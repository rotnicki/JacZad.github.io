---
id: 401
title: 'Poprawność techniczna (WCAG 2.0 SC 4.1.1, poziom A)'
date: '2012-11-23T09:33:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=401'
permalink: /2012/11/23/poprawnosc-techniczna-wcag-2-0-sc-4-1-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - błędy
    - semantyka
    - walidacja
---

Treści publikowane w Internecie powinny dawać się parsować i walidować, a zatem powinny być poprawne technicznie, zgodne ze specyfikacjami technicznymi. Poprawny kod HTML wydaje się czymś oczywistym i stosunkowo łatwym do zaprogramowania, a przecież tak mało jest serwisów internetowych poprawnych technicznie.

Kryterium sukcesu 4.1.1 zobowiązuje do tworzenia prawidłowego kodu w wypadku stosowania technologii opartych o znaczniki. Znaczniki powinny być prawidłowo otwarte, zamknięte, zagnieżdżone w odpowiedniej kolejności i nie posiadać powtarzających się argumentów. Skorzystają na tym:

- użytkownicy korzystający z technologii asystujących,
- roboty sieciowe, które agregują i analizują treści,
- deweloperzy integrujący różne systemy,
- administratorzy serwisów.

Wydawałoby się, że stosowanie poprawnego kodu stron internetowych jest oczywistością. Jednak serwisy powstają w wyniku montażu wielu różnych elementów, technologii, gotowych bibliotek, edytorów wizualnych i źródłowych. Bardziej skomplikowana usługa jest właściwie aplikacją uruchamianą w przeglądarce, a jej objętość utrudnia zadbanie o kod.

W sukurs programistom przychodzą walidatory kodu, jak ten oferowany przez World Wide Web Consortium pod adresem[validator.w3c.org](http://validator.w3c.org) lub Tidy. Pozwalają one na odnalezienie błędów przez wskazanie miejsca, gdzie takowy błąd się znajduje. Dzięki temu można go stosunkowo łatwo usunąć.

Czasem pada pytanie, czy to jest naprawdę takie ważne, skoro strona się wyświetla. Otóż strona się wyświetla w przeglądarce, bo tak się projektuje przeglądarki, by wyświetlały nieprawidłowy kod. Jednakże fakt, że strona “jakoś”się wyświetla, nie powinien przesłaniać nam problemu, jaki może generować dla programów mniej odpornych na błędy. Należą do nich technologie wspomagające, na przykład czytniki ekranu, które korzystają z interfejsów pośredniczących, jak MS Active Accessibility czy też AT-SPI. Jeżeli przeglądarka nie wie, co ma przekazać do tych interfejsów, to może nie przekazać nic lub wykonać operację błędnie. Podobny problem mają roboty sieciowe, które usiłują analizować zawartość stron internetowych, jak choćby wyszukiwarki internetowe. Jeżeli kod jest generowany w locie przez JavaScript, to nawet jeżeli jest poprawny, to nie da się analizować. Jednak niepoprawny kod sprawia, że informacja może być źle zaindeksowana, co wpływa na pozycję strony w wyszukiwarce.

Wreszcie dla mnie poprawność kodu to ważny element rzemiosła, jakim jest tworzenie stron internetowych. Programista tworzący wadliwy kod jest jak pisarz piszący z błędami ortograficznymi. Na dodatek ten rodzaj błędów najłatwiej jest wykryć w sposób obiektywny, co naraża programistę na zażenowanie. Dlatego warto dbać o poprawność językową HTML czy XML.