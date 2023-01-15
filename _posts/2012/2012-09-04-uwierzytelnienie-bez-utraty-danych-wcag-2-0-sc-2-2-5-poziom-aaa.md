---
id: 215
title: 'Uwierzytelnienie bez utraty danych (WCAG 2.0 SC 2.2.5, poziom AAA)'
date: '2012-09-04T09:18:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=215'
permalink: /2012/09/04/uwierzytelnienie-bez-utraty-danych-wcag-2-0-sc-2-2-5-poziom-aaa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - bezpieczeństwo
    - czas
    - formularze
    - logowanie
    - sesja
---

Chociaż coraz rzadziej, ale wciąż zdarzają się serwisy internetowe, w których użytkownik musi po kilka razy wprowadzać te same dane. Dzieje się tak zazwyczaj wtedy, gdy wygaśnie sesja lub system z innego powodu nabierze wątpliwości co do autentyczności użytkownika.

Kryterium sukcesu 2.2.5 zobowiązuje do projektowania systemów transakcyjnych (sprzedażowych, usługowych, bankowych) w taki sposób, by po ewentualnym wygaśnięciu sesji użytkownik mógł potwierdzić swoją tożsamość (zalogować się) i kontynuować pracę **bez utraty danych**. Na przestrzeganiu tej zasady skorzystają:

- wszyscy użytkownicy serwisu,
- w szczególności osoby pracujące w wolniejszym tempie lub korzystający z technologii asystujących.

Jest to jedna z zasad na pograniczu dostępności i bezpieczeństwa. Jednak przyjrzawszy się jej bliżej, widać że nie stoją w sprzeczności. Chodzi tu w skrócie o rozwiązanie, dzięki któremu pracowicie wprowadzone dane nie znikną po wygaśnięciu sesji. Takie wygaśnięcie może wystąpić po upłynięciu określonego czasu, po określonym czasie bezczynności użytkownika lub po zalogowaniu się do tej samej usługi za pomocą innego urządzenia, na przykład telefonu komórkowego. System może zarządać potwierdzenia tożsamości przez podanie hasła, ale ta autoryzacja nie może spowodować wykasowania danych.