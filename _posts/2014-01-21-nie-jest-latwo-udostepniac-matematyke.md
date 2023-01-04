---
id: 934
title: 'Nie jest łatwo udostępniać matematykę'
date: '2014-01-21T14:40:29+01:00'
layout: post
guid: 'http://informaton.pl/?p=934'
permalink: /2014/01/21/nie-jest-latwo-udostepniac-matematyke/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - e-podręcznik
    - LaTeX
    - matematyka
    - MathML
    - MEN
    - ORE
---

Podczas prac nad e-podręcznikiem prowadzonymi przez Ośrodek Rozwoju Edukacji, jednym z największych wyzwań okazało się udostępnienie matematyki. Podręczniki do tego przedmiotu zawierają wzory, wykresy, matryce i wiele innych elementów, które mają charakter grafiki, mimo że często korzystają ze znaków alfanumerycznych. Jak zaprezentować taką informację niewidomym uczniom? Są na to różne sposoby.

### MathML – język opisu matematyki zupełnie nieczytelny

Pierwszym narzucającym się sposobem znalezienia rozwiązania jest sięgnięcie do standardów sieciowych. Chwila poszukiwań i na stronach <span lang="en">World Wide Web Consortium</span> znajdujemy język opisu wzorów matematycznych za pomocą znaczników o nazwie [MathML](http://www.w3.org/Math/). Bardzo dobrze, ale co nam z tego? Wiele przeglądarek prawidłowo wyświetla wzory zapisane w MathML, ale jak je udostępnić niewidomemu uczniowi? Przecież kod złożony ze znaczników jest dla normalnego człowieka trudny do przetworzenia i zrozumienia. Zobacz [“prosty przykład” kodu w MathML opublikowany w Wikipedii](http://pl.wikipedia.org/wiki/MathML).

Jeszcze chwila poszukiwań i pojawia się nam [MathPlayer](http://www.dessci.com/en/products/mathplayer/) – wtyczka do przeglądarki MS Internet Explorer. Jej podstawowym zadaniem jest przekazanie w ludzkim języku zapisu wzoru przygotowanego w MathML. Niestety “ludzki” oznacza w tym wypadku język angielski. Wydaje się, że dla ucznia byłoby sporym wyzwaniem zrozumienie skomplikowanego wzoru w obcym języku. Do tego rozszerzenie jest tylko dla jednej przeglądarki, a zatem nie jest w najmniejszym stopniu uniwersalne. Może być jakoś tam pomocne, ale do wdrożenia się nie nadaje.

### Opowiedz mi o wzorze

A może podejść do wzorów tak, jak do zwykłej grafiki, do której można dodać tekst alternatywny… MathPlayer robi to automatycznie na podstawie MathML, ale czy człowiek nie da sobie z tym rady? Oczywiście że sobie da radę! Pojawiają się jednak różnorodne problemy. Po pierwsze – jest dosyć głupim rozwiązaniem, gdy człowiek przetwarza informację cyfrową na inną informację cyfrową, gdy powinien to robić komputer. Po drugie – łatwo tu o pomyłkę, którą z kolei trudno jest odnaleźć. Po trzecie wreszcie – należy przyjąć wspólny dla wszystkich wzorów algorytm kodowania informacji. Ten sam wzór można opowiedzieć na różne sposoby, a sposób powinien być jeden. Nawet odczytywanie konkretnego znaku musi być jednolite. Spróbujmy jednak.

> Duże E równa się małe m razy małe c do kwadratu

A może raczej…

> e równa się m c kwadrat

Albo…

> Duże E równe jest iloczynowi m i c podniesionemu do drugiej potęgi

A mamy tu zaledwie pięć znaków i bardzo prosty wzór. Jednoznaczność jest tutaj absolutnie niezbędna, a takiej nie zapewni nam żywy człowiek, choćby nie wiem jak staranny. Proces musi być zautomatyzowany.

### Jak się to robi w Wikipedii…

Sprytnie rozwiązano problem wyświetlania wzorów matematycznych w Wikipedii. Jeżeli zachodzi potrzeba, by takowy zaprezentować, w kodzie używany jest [LaTeX](http://www.latex-project.org/), czyli specjalnie zaprojektowany język do składu dokumentów. A że wymyślił go amerykański matematyk Donald Knuth, któremu nie podobał się sposób składania jego publikacji przez wydawnictwo, to i LaTeX został doprowadzony do perfekcji w tym właśnie zastosowaniu. No dobrze… Puryści mnie poprawią, że Knuth wymyślił TeX, a LaTeX jest jedynie nakładką, ale matematykę zapisuje się tak samo.

Kod LaTeXowy przetwarzany jest przez specjalny skrypt, który generuje czarno-biały obrazek w formacie PNG. Więcej o tym mechanizmie można przeczytać na [dedykowanej stronie Wikipedii po angielsku.](http://meta.wikimedia.org/wiki/Help:Formula#TeX) Jednak sam TeX nie ginie i jest wstawiany jako tekst alternatywny dla obrazka, który można zobaczyć najeżdżając kursorem myszy na obrazek. Może przyjąć postać:

> $E=mc^{2}$

Albo – po usunięciu zbędnych w tym momencie znaków dolara:

> E=mc^{2}

Wydaje się, że znaleźliśmy idealne rozwiązanie. Wzór jest pięknie wyświetlony, tekst alternatywny jest jednoznaczny, a zarazem stosunkowo prosty do zrozumienia. Jest jednak mały haczyk…

### Nie wszystkim da się dogodzić

Plik PNG jest domyślnie generowany z białym tłem i czarnym wzorem. Kontrast wynosi 21:1, czyli większego się nie da. Mamy zatem spełnienie wymagań WCAG 2.0 na poziomie AA. Jednak są użytkownicy, którym to nie wystarczy. To ci, którzy – z powodu chorób siatkówki – korzystają z tzw. trybu wysokiego kontrastu. Polega o najczęściej na zmianie kolorystyki, by tło było ciemne, a tekst jasny. Jeżeli oprogramowanie zamieni kolory po prostu w sposób negatywowy, jak to robią OS X i iOS – problemu nie będzie. Jeżeli jednak tekst i tło się zmienią, a obrazek – nie, a dzieje się tak w systemie Windows, to efekt nie będzie ciekawy. Na ciemnej, najczęściej czarnej stronie, po oczach będzie bił biały prostokąt obrazka z wzorem, którego nie da się odczytać. Włączenie przeźroczystości dla koloru białego w pliku PNG niewiele da. Co prawda biały prostokąt nie będzie już raził, ale czarny wzór na czarnym tle będzie równie widoczny, jak biały niedźwiedź na śniegu.

Nie umiem na szybko zaproponować rozwiązania tego problemu. Może jakiś skrypt wykrywający TWK generujący pliki w innej kolorystyce. Albo zamiast pliku PNG wektorowa grafika SVG z kontrolkami do zmiany kolorów… W każdym razie wszystkich i na szybko zadowolić się nie da. A przed nami jeszcze wykresy, macierze i inne urocze elementy podręczników do matematyki. No cóż, nikt nie mówił, że będzie łatwo.