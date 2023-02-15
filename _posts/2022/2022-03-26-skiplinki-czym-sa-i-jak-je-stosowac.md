---
id: 2681
title: 'Czym są skiplinki i jak je stosować?'
date: '2022-03-26T14:25:00+01:00'
author: 'Jacek Zadrożny'
layout: post
categories:
    - artykuły
tags:
    - 'fokus klawiatury'
    - klawiatura
    - 'WCAG'
    - 'skiplink'
excerpt: Poradnik na temat prawidłowego stosowania skiplinków na stronach internetowych.
---

WCAG rekomendują stosowanie skiplinków w kryterium sukcesu 2.4.1: możliwość pominięcia bloków. Ostatnio zaciekawiło mnie bogactwo rodzajów i sposobów wdrażania skiplinków. Postaram się zatem trochę podpowiedzieć, żeby unikać pewnych rozwiązań. Zatem do dzieła!

## Dla kogo są skiplinki?

Skiplinki są przeznaczone dla osób, które nawigują po stronie internetowej za pomocą klawiatury. Takie osoby nie mogą lub nie chcą korzystać z myszy, trackballa lub innego urządzenia wskazującego. Za to korzystają z tabulatora, który przenosi fokus pomiędzy aktywnymi elementami, na przykład łączami.

Taki użytkownik jest zatem postawiony w mało komfortowej sytuacji, ponieważ musi użyć tabulatora wiele razy, zanim dotrze do interesującego go miejsca. Takim problematycznym miejscem jest najczęściej system nawigacji – menu w różnych smakach, wyszukiwarka itp. Innym miejscem mogą być osadzone na stronie zewnętrzne elementy. Ostatnio policzyłem aktywne elementy w osadzonym feedzie Twittera. Było ich 168, co oznacza że tyle razy trzeba nacisnąć tabulator, żeby się przedrzeć za ten widżet.

## Jak powinny wyglądać i działać skiplinki?

Skiplink powinien być pierwszym elementem, na jaki natrafia fokus klawiatury po wczytaniu strony internetowej. Dopuszczalne jest jego ukrycie wizualne i wyświetlanie go w momencie otrzymania fokusu klawiatury. Jednak osobiście radzę, by był on widoczny przez cały czas. “Widoczny” oznacza także, że fokus umieszczony na nim musi być dobrze widoczny. Fokus jest zazwyczaj ramką otaczającą aktywny element, chociaż można go wyróżniać na inne sposoby. Jeżeli jest tojednak ramka, to pamiętaj o odpowiednim kontraście i grbości.

## Etykieta i cel

Wydawałoby się, że najlepszą etykietą dla skiplinku będzie “pomiń nawigację”, co jest zgodne z zapisami WCAG. Jednak już się przyjęło, że etykieta nie informuje, co można pominąć, lecz dokąd można fokus przenieść. Dlatego optymalnym jest etykieta w rodzaju “przeskocz do treści”. Etykieta powinna być możliwie krótka, więc odradzam taką w rodzaju “przenieś fokus do głównej cześci strony internetowej”.

Treść etykiety powinna pasować do celu, do którego prowadzi skiplink. Zdecydowanie najczęściej powinien prowadzić do obszaru, któremu można nadać rolę “main”. W innych przypadkach musisz samodzielnie zdecydować, który obszar jest tym najważniejszym.

## Ile tych skiplinków?

WCAG wymaga tylko tego jednego skiplinku. Jednak często spotykam całe zestawy, prowadzące do menu bocznego, wyszukiwarki, stopki i jeszcze w inne miejsca. To nie jest błąd, o ile zachowasz w tym umiar.

Duża liczba skiplinków może całkowicie zanegować ich sens. One same stają się dodatkowym systemem nawigacji, który trzeba jakoś pominąć. A zatem należałoby dodać jeszcze skiplink do pomijania skiplinków. To byłby jednak już absurd.

## Podsumowanie

- Skiplink owinien być na każdej podstronie strony internetowej.
- Skiplink powinien być pierwszym elementem przechwytującym fokus klawiatury.
- Skiplink może być ukryty wizualnie, ale lepiej by zawsze był widoczny.
- Skiplink powinien kierować do najważniejszego obszaru podstrony.
- Jeden skiplink jest obowiązkowy. Więcej skiplinków wymaga namysłu, a jeżeli nie masz pewności – odpuść.