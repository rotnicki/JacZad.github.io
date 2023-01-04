---
id: 328
title: 'Brak nieoczekiwanych zmian kontekstu (WCAG 2.0 SC 3.2.5, poziom AAA)'
date: '2012-10-24T13:29:47+02:00'
layout: post
guid: 'http://informaton.pl/?p=328'
permalink: /2012/10/24/brak-nieoczekiwanych-zmian-kontekstu-wcag-2-0-sc-3-2-5-poziom-aaa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - Ajax
    - formularze
    - JavaScript
    - klawiatura
    - nawigacja
---

Na wyższych poziomach dostępności WCAG ogranicza niektóre wyjątki, jakie są dopuszczalne na poziomach niższych. O ile zatem na poziomie A wymagane było przynajmniej ostrzeżenie użytkownika o nieprzewidywalnych zachowaniach, by były nieco bardziej przewidywalne. Na wyższym poziomie trzeba zrezygnować z takich rozwiązań w ogóle lub zaproponować alternatywne rozwiązanie.

Kryterium sukcesu 3.2.2 zobowiązuje projektantów serwisów internetowych, by podczas wprowadzania danych w formularzach użytkownik nie był zaskakiwany zmianą kontekstu. Zmiana kontekstu oznacza między innymi uruchomienie innej aplikacji, otwarcie innej strony, zmianę sposobu prezentacji treści lub sensu dokumentu. Skorzystają na tym:

- użytkownicy niewidomi i słabowidzący,
- użytkownicy klawiatur,
- użytkownicy z ograniczeniami kognitywnymi,
- seniorzy.

Stosowanie tej zasady właściwie uniemożliwia stosowanie tzw. interaktywnych formularzy, co może wzburzyć niektórych projektantów. Jednak po chwili zastanowienia dojdą do wniosku, że to się da zrobić. Można przecież stosować kreatory, gdzie kolejne wyświetlone okno zależy od tego, jakie dane były wprowadzone wcześniej. Zaś samą zmianę kontekstu trzeba pozostawić użytkownikowi w postaci przycisku “dalej” lub “przejdź”. Można zrobić także dwie wersje formularza – jedną interaktywną i drugą – statyczną, by użytkownik mógł sobie wybrać, ale to raczej sztuka dla sztuki. Na pocieszenie dodam, że tak wymuszona statyczność formularzy może pozytywnie wpłynąć na ich logikę.