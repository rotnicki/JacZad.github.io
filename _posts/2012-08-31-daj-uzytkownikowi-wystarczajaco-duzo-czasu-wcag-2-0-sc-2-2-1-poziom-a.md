---
id: 206
title: 'Daj użytkownikowi wystarczająco dużo czasu (WCAG 2.0 SC 2.2.1, poziom A)'
date: '2012-08-31T09:13:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=206'
permalink: /2012/08/31/daj-uzytkownikowi-wystarczajaco-duzo-czasu-wcag-2-0-sc-2-2-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - czas
    - formularze
    - klawiatura
    - sesja
    - testy
---

Użytkownicy pracują w różnym tempie – jedni są bardziej doświadczeni lub sprawni manualnie od innych, chociaż czasem zależy to od samego urządzenia lub oprogramowania. Warto uwzględnić te różnice przy projektowaniu stron internetowych, by każdy miał równy dostęp do treści.

Kryterium sukcesu 2.2.1 dotyczy serwisów internetowych, wktórych upływający czas może spowodować, że treść lub funkcje zmienią się bez interwencji użytkownika. W takiej sytuacji trzeba dać mu możliwość zatrzymania upływu czasu, przedłużenia go przynajmniej dziesięciokrotnie lub ostrzec przed końcem na przynajmniej 20 sekund, by mógł w prosty sposób zareagować, na przykład przez naciśnięcie klawisza. Od tych zasad uczyniono trzy odstępstwa:

 &lt;liGdy czas dotyczy wydarzeń realnych, na przykład zakończenia aukcji lub transmisji na żywo. 2. Gdy upływający czas stanowi kluczową wartość, na przykład w wypadku zadań wykonywanych na czas.
3. Gdy czas został określony na co najmniej 20 godzin.

Na stosowaniu tej zasady skorzystają:

- użytkownicy mający problem z obsługą klawiatury i myszki,
- seniorzy,
- użytkownicy niewidomi i słabowidzący,
- nowicjusze w Internecie,
- użytkownicy przypadkowego sprzętu i oprogramowania.

Problem dynamicznie zmieniających się stron internetowych dotyczy wielu grup użytkowników. Nie każdy jest w stanie odpowiednio szybko odczytać informację, przetworzyć i zareagować. Ograniczony czas jest często stosowany jako element zabezpieczenia danych użytkownika, na przykład w transakcjach finansowych. A zatem trzeba pogodzić dwa, pozornie sprzeczne ze sobą, cele: bezpieczeństwo i dostępność. Można to zrobić w dosyć prosty sposób.

Użytkownik powinien mieć świadomość, że upływający czas ma swoje znaczenie i odejście od komputera podczas wykonywania operacji może spowodować na przykład wylogowanie z systemu. Jednak w wypadku niektórych użytkowników brak reakcji może wynikać z ich ograniczeń fizycznych, które uniemożliwiają im szybkie nawigowanie po stronie. Najlepiej dać wówczas możliwość wyłączenia upływu czasu w ogóle, by mogli z pełnym spokojem realizować zadanie, bez presji upływającego czasu. Nieco gorszym rozwiązaniem jest zaproponowanie wydłużenia dostępnego czasu przez użytkownika, przy czym to wydłużenie musi wynosić przynajmniej dziesięciokrotność czasu domślnie ustalonego, na przykład z 1 minuty do 10 minut. Najmniej korzystnym rozwiązaniem jest ostrzeżenie użytkownika o końcu upływającego czasu na przynajmniej 20 sekund przed jego upłynięciem. Takie ostrzeżenie może być zrealizowane przez wyskakujące okno alertu, a użytkownik powinien mieć możliwość zareagowania w możliwie prosty sposób, na przykład naciśnięcie spacji. Natomiast niedopuszczalne jest, by taka reakcja wymuszała użycie kursora myszy (kliknięcie), ponieważ naruszałoby to [kryterium sukcesu 2.1.1](http://informaton.pl/?p=184).

Są jednak sytuacje, gdy dowolne regulowanie czasu nie jest możliwe i wtedy stosowanie powyższych zasad nie jest obowiązujące. Dotyczy to dwóch sytuacji: gdy czas jest realny lub gdy jest kluczowy. Czas jest realny, gdy dotyczy faktycznych zdarzeń lub interakcji z innymi ludźmi. Nie da się wydłużyć dowolnie czasu, gdy dotyczy on momentu zakończenia aukcji, złożenia zlecenia na zakup akcji i podobnych sytuacji. Trudno też go sobie wyobrazić podczas wspólnej gry z innymi użytkownikami w <abbr title="Multi User Dungeon">MUD</abbr> lub synchronicznego edytowania dokumentów.

Drugie odstępstwo dotyczy sytuacji, gdy czas trwania operacji jest kluczowy dla oceny i dotyczy przede wszystkim wszelkiego rodzaju testów. Jeżeli na rozwiązanie danego testu przeznaczony jest określony czas, to użytkownik nie może go sobie dowolnie wydłużać lub zatrzymywać. Jednak w takich sytuacjach trzeba wziąć pod uwagę ograniczenia dotykające osoby z różnymi rodzajami niepełnosprawności i dla wyrównania szans należy im zaproponować określony, chociaż wydłużony czas na zaliczenie testu. Na uczelniach wyższych i podczas matur zazwyczaj przyjmuje się przedłużenie czasu o połowę, czyli na przykład trzy godziny zamiast dwóch. Jest to jednak czas bezwzględnie przestrzegany i nie powinien być już modyfikowany przez użytkownika.

W sytuacji, gdy czas wygaśnięcia sesji lub inny wyznaczony upływ określono na co najmniej 20 godzin, w ogóle nie należy stosować opisywanej zasady. W takiej sytuacji można przyjąć, że czas nie jest ograniczony i kryterium sukcesu jest automatycznie spełnione.