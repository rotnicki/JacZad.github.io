---
id: 862
title: 'Ostrożnie z ukrywaniem treści, czyli o dylematach w dostępności'
date: '2013-10-13T11:10:49+02:00'
layout: post
guid: 'http://informaton.pl/?p=862'
permalink: /2013/10/13/ostroznie-z-ukrywaniem-tresci-czyli-o-dylematach-w-dostepnosci/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - audyt
    - etykiety
    - formularze
    - HTML5
    - walidator
    - 'WCAG 2.0'
---

Sprawdzając niedawno dostępność jednego z serwisów internetowych, odkryłem ciekawą właściwość czytników ekranu i walidatorów dostępności. Mogą podawać sprzeczne informacje, gdy projektant wykaże się odpowiednią gimnastyką w pisaniu kodu. A problem pojawił się przy okazji ukrywania treści przed użytkownikami.

Stosowałem swoje zwyczajowe narzędzia do testowania, to znaczy [czytnik ekranu NVDA](http://informaton.pl/?p=352)i [pasek narzędzi WAVE](http://informaton.pl/?p=21). Zgrzyt pojawił się przy polu wyszukiwarki. WAVE nie informował o braku etykiety dla pola edycyjnego, a nawet o jego istnieniu. Tymczasem NVDA nie oznajmiał etykiety, ani w trybie przeglądania, ani w trybie formularzy. Było to na tyle niezwykle, że zerknąłem do kodu strony i znalazłem tam coś takiego:

```
<label for="search" style="display: none;">wyszukaj</label>
<input type="text" id="search" name="search">

```

A zatem programista dodał etykietę do pola formularza, a potem ją ukrył za pomocą stylów. Dlatego walidator nie wykrył problemu, chociaż ten ewidentnie występuje. To pokazuje, że nie wolno ufać walidatorom, bo zbyt łatwo je oszukać. Pogadałem na ten temat z Dominikiem Paszkiewiczem, a potem zacząłem myśleć nad sposobem rozwiązania problemu.

### Poszukiwanie rozwiązania

Cel do osiągnięcia jest następujący: dodać etykietę do pola wyszukiwarki, a jednocześnie ukryć ją przed użytkownikami. Pomijam, że to w zasadzie jest sprzeczne z wymaganiami dostępności, bo etykieta powinna być widoczna dla wszystkich, ale sam problem jest ciekawy. Na początek warto dodać troszkę semantyki.

```
<input type="search" id="search" name="search">

```

Powyższe rozwiązanie można zastosować, jeżeli strona jest wykonana w standardzie HTML5. Pozwala on na korzystanie z [nowych typów pól](http://informaton.pl/?p=497)wskazujących wprost, jakie dane należy tam wprowadzić. Jeżeli jednak nie jest to HTML5 lub jeżeli chcemy tenże HTML5 uzupełnić, to warto skorzystać z technik ARIA:

```
<form role="search">
<input type="search" id="search" name="search" aria-label="Wyszukaj">
<input type="submit" id="searchbutton" value="Szukaj!">
</form>

```

W ten sposób oznaczyliśmy punkt orientacyjny (landmark) dla wyszukiwarki i dodaliśmy do pola wyszukiwania etykietkę. Przykład można użyć w HTML5, a we wcześniejszych wersjach tego języka atrybut TYPE trzeba ustawić na TEXT. Jeżeli ktoś ma zamiar tu skończyć, to oczywiście może, ale warto zwrócić uwagę na kilka dodatkowych problemów

### Dylematy dostępności

Powyższe rozwiązanie jest wystarczające, o ile użytkownik ma nowoczesną przeglądarkę i nowoczesny czytnik ekranu. Pierwsze jest stosunkowo proste, chociaż wielu niewidomych użytkowników trwa przy przeglądarce Internet Explorer, a system Windows XP uwięził ich na wersji numer 8. A zatem nie skorzystają z większości dobrodziejstw ARIA. Jeszcze gorzej jest z czytnikami ekranu, bo są to programy bardzo drogie, a obsługa nowszych przeglądarek i ARIA wymaga kosztownej aktualizacji. Jest co prawda NVDA, ale wciąż za mało rozpowszechniony, a i przyzwyczajenie do czytnika ekranu robi swoje. Jest zatem potencjalnie duża grupa użytkowników,nie będących w stanie dotrzeć do informacji o etykiecie.

Z drugiej strony – zasady dostępności mówią, że etykieta powinna być dostępna dla wszystkich, a zatem samo jej ukrywanie jest naruszeniem wymagań WCAG 2.0. Etykiety nie służą tylko niewidomym użytkownikom, lecz także osobom mniej doświadczonym i mającym problemy z rozumieniem treści i nawigacji. Z tego punktu widzenia kod powinien wyglądać następująco:

```
<form role="search">
<label for="search">
<input type="search" id="search" name="search" aria-label="Wyszukaj">
<input type="submit" id="searchbutton" value="Szukaj!">
</form>

```

To rozwiązanie **nie ukrywa etykiety**, jak to miał w planie projektant. Wydaje się, że w tym przypadku dostępność ma wpływ na wygląd i nie da się tego ominąć. Opisywana sytuacja pokazuje też, że trzeba z ostrożnością przyjmować raporty z automatycznych walidatorów. Te narzędzia nie mogą uwzględniać wszystkich pomysłów projektantów, a zatem mogą być mylące. Okazuje się, że testów dostępności nie da się zautomatyzować, a przynajmniej nie da się tego zrobić w tym momencie.