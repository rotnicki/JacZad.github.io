---
id: 1630
title: 'Automatyczne walidatory dostępności działają za słabo, by na nich polegać'
date: '2017-03-02T12:42:36+01:00'
layout: post
guid: 'http://informaton.pl/?p=1630'
permalink: /2017/03/02/automatyczne-walidatory-dostepnosci-dzialaja-za-slabo-by-na-nich-polegac/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - automaty
    - badania
    - Google
    - Tenon
    - walidator
    - WAVE
---

Badania dostępności stron nie da się zautomatyzować. Piszę o tym od czasu do czasu przypominając, że walidatory są tylko omylnymi narzędziami i człowiek z odpowiednią wiedzą musi im pomagać. Czasem zastanawiałem się też, jaka jest efektywność narzędzi w rodzaju Wave czy Tenon. No i wreszcie mam na to odpowiedź.

> We recently conducted an audit of automated accessibility testing tools. We built a website full of accessibility failures to test them on. We’ve published our findings here.In this blog post we

Źródło: *[What we found when we tested tools on the world’s least-accessible webpage | Accessibility](https://accessibility.blog.gov.uk/2017/02/24/what-we-found-when-we-tested-tools-on-the-worlds-least-accessible-webpage/)*

Autorzy tego eksperymentu stworzyli “najmniej dostępną stronę w internecie”, by przetestować 10 narzędzi do automatycznej walidacji. Z tą “najmniej dostępną”, to trochę przesadzili, bo ja spotykam na codzień o wiele gorsze. Jednak potrzebna im była do testów. Wsadzili więc do niej prawie półtorej setki błędów i zapuścili narzędzia walidujące. Efekt był do przewidzenia – nie da się automatycznie badać dostępności.

Automaty były wrażliwe na mniej niż 30% błędów, a uwzględniając też ostrzeżenia – mniej niż 40%. Co więcej – ponad 40% błędów nie zostało zgłoszonych przez żadne z narzędzi! Zatem nie ma narzędzi, nawet zaprzęgniętych razem do roboty, które mogłyby dokonać rzetelnej oceny dostępności. Efektywność waha się w przedziale 17-29%, co nie wygląda zbyt dobrze. Trudno też uznać, że coś może się w niedalekiej przyszłości poprawić. Nadal trzeba polegać na ludziach – ekspertach i użytkownikach.