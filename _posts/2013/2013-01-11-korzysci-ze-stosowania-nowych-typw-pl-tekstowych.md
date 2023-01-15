---
id: 497
title: 'Korzyści ze stosowania nowych typów pól tekstowych'
date: '2013-01-11T18:47:18+01:00'
layout: post
guid: 'http://informaton.pl/?p=497'
permalink: /2013/01/11/korzysci-ze-stosowania-nowych-typw-pl-tekstowych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - formularze
    - 'HTML 5'
    - klawiatura
    - mobilne
    - semantyka
---

Specyfikacja HTML 5 wprowadza sporo nowych typów pól formularzy, które są mocno wyspecjalizowane. Odpowiednio użyte mogą być ułatwieniem dla webmasterów i użytkowników, chociaż ich implementacja wciąż nie jest kompletna. Ja jednak chciałbym zachęcić do ich stosowania na przykładzie pola typu EMAIL.

Stosowanie nowych typów pól jest banalnie proste i polega na podania ich jako wartości atrybutu TYPE. Można to zrobić chociażby tak:

```
<form>
<label for="login">Użytkownik: </label>
<input type="email" placeholder="wpisz adres email" name="login" id="login">
</form>

```

## Walidacja typów pól

Można zapytać – po co takie rozwiązanie, skoro i tak trzeba oprogramować takie pole. Trzeba dodać skrypt, który sprawdzi, czy tekst jest adresem poczty elektronicznej. Do tego wystarczy pole typu TEXT i zapewni się w ten sposób całkowitą zgodność. To jest prawda, ale tylko częściowa. Niektóre przeglądarki, na przykład Firefox, potrafią już sprawdzić wprowadzony tekst i wyświetlić odpowiednie ostrzeżenie. Jednak faktycznie – na razie bez skryptu obejść się nie da. Warto jednak wprawiać się w stosowaniu nowych standardów. W starych przeglądarkach pole nieznanego typu wyrenderowane zostanie jako pole typu TEXT i zgodność zostanie zachowana.

## Klawiatury mobilne

Jest przynajmniej jeden dobry powód, by stosować pole typu EMAIL. Takie pole zostanie prawidłowo zinterpretowane przez większość mobilnych przeglądarek internetowych i do wprowadzania danych system może zaproponować bardziej dostosowaną klawiaturę. W systemie iOS po napotkaniu na pole tego typu, system zaproponuje klawiaturę z dodatkowymi znakami “@” i “.”. To niewielkie udogodnienie sprawia, że wprowadzając adres jacek.zadrozny@hotmail.com nie muszę przełączać się sześciokrotnie pomiędzy klawiaturami. Podobnie jest w innych przeglądarkach mobilnych i na innych systemach. Rozwiązanie to działa także w wypadku wykorzystywania HTML 5 do budowania interfejsów aplikacji, w tym oczywiście webowych. Podobnie działać będzie stosowanie typu URL, kiedy to dostaniemy znaki w rodzaju “/” i “:”.

## Semantyka kodu

Ostatnim powodem dla stosowania tych nowych typów jest dbałość o semantykę kodu. Specyfikacje HTML oferują szeroki wachlarz znaczników i atrybutów pozwalających na precyzyjne opisywanie rodzaju treści.Im bardziej semantycznie zaprojektowany jest serwis internetowy, tym lepiej poradzą sobie z nim różne narzędzia: agregatory treści, technologie asystujące i wyszukiwarki. To chyba też dobry argument.