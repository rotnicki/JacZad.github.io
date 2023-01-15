---
id: 371
title: 'Sugerowanie poprawnych wartości (WCAG 2.0 SC 3.3.3, poziom AA)'
date: '2012-11-14T09:36:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=371'
permalink: /2012/11/14/sugerowanie-poprawnych-wartosci-wcag-2-0-sc-3-3-3-poziom-aa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - bezpieczeństwo
    - błędy
    - dysleksja
    - formularze
    - pomoc
---

Wprowadzanie danych w formularzach może być zajęciem frustrującym, gdy użytkownik nie do końca jest pewien, jak ma to zrobić. Czasem nie wystarczą odpowiednie etykiety, objaśnienia i wskazywanie miejsc, w których system odnalazł błąd. Wtedy trzeba spróbować czegoś jeszcze – zasugerowania użytkownikowi prawidłowej wartości.

Kryterium sukcesu 3.3.3 zaleca projektantom serwisów internetowych, by projektowali formularze w taki sposób, by potrafiły zasugerować użytkownikowi prawidłową wartość w miejsce wykrytego błędu. Nie dotyczy to sytuacji, gdy zagrażałoby to bezpieczeństwu użytkownika. Skorzystają na tym:

- użytkownicy z małym doświadczeniem,
- seniorzy,
- osoby z ograniczeniami kognitywnymi,
- dyslektycy.

Odpowiednio zaprojektowany system potrafi przewidywać wartości wprowadzane przez użytkownika, a szczególnie wtedy, gdy potrafi wykrywać błędy. Jeżeli jest to możliwe, to powinien zasugerować prawidłową wartość lub upewnić się co do intencji. Użytkownik wprowadzający datę urodzenia może popełnić wiele różnych błędów: przestawić znaki, podać dane w złym formacie, wpisać literę “O” zamiast cyfry “0”. System zazwyczaj potrafi rozpoznać, że użytkownik się pomylił i powinien o tym poinformować. Może jednak zrobić coś więcej, jak to robi chociażby wyszukiwarka Google: może zasugerować wartość prawidłową. Może zatem zapytać “Czy na pewno urodziłeś się 12 marca 1870 roku? To by oznaczało, że masz 143 lata, a to bardzo dużo. Może raczej urodziłeś się w 1970 lub 1987 roku.” Zakładamy przy tym, że system ma wątpliwości wyłącznie do roku urodzenia i pozwala na kliknięcie w link z dobrym rocznikiem.

Wykrywanie błędów przez samego użytkownika może być trudne z kilku powodów. Dyslektycy często zamieniają kolejność znaków i nie widzą różnicy pomiędzy “1987” i “1897”. Są też użytkownicy, dla których wygląd znaków jest tożsamy z ich znaczeniem i stosują literę “O” zamiast cyfry “0” jak w maszynach do pisania. Powodów może być zresztą znacznie więcej i trzeba pamiętać, by użytkownikowi ułatwić życie.

Takie ułatwienie nie dotyczy sytuacji związanych z bezpieczeństwem w sieci. Najlepszym przykładem jest wpisywanie hasła, gdzie nawet dyslektykowi nie wolno podpowiedzieć prawidłowego. Tutaj muszą wystarczyć sugestie w rodzaju “Upewnij się, że nie masz włączonego klawisza CapsLock” lub “liczba gwiazdek powinna odpowiadać liczbie znaków w haśle” czy wreszcie “W haśle rozróżnia się wielkość liter”.