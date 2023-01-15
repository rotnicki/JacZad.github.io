---
id: 247
title: 'Nawigacja fokusa (WCAG 2.0 SC 2.4.3, poziom A)'
date: '2012-09-16T08:52:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=247'
permalink: /2012/09/16/nawigacja-fokusa-wcag-2-0-sc-2-4-3-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - fokus
    - formularze
    - klawiatura
    - narzędzia
    - nawigacja
    - semantyka
    - WAVE
---

Fokus to miejsce, w którym w konkretnym momencie skoncentrowana jest uwaga systemu operacyjnego lub aplikacji. Podkreślam – nie użytkownika, który może przyglądać się akurat zupełnie innemu miejscu. I jest to miejsce wyróżnione podświetleniem, ramką lub w inny sposób. Tego właśnie miejsca (fokusa) dotyczą wszelkiego rodzaju czynności kontekstowe.

Kryterium sukcesu 2.4.3 zobowiązuje, by fokus przemieszczany był w sposób sensowny z punktu widzenia logiki strony. Przemieszczanie fokusa odbywa się za pomocą klawiatury przy użycia klawisza Tab. Skorzystają na tym:

- użytkownicy niewidomi,
- użytkownicy nie używający myszy (na przykład w telefonie komórkowym),
- użytkownicy z niedowładami rąk.

Problemów z fokusem nie mają użytkownicy myszy, bo jest on automatycznie przenoszony do obiektu, na którym użytkownik wykonuje akcję, na przykład klika. Jednak wielu użytkowników nie korzysta z myszy, ale z klawiatury i wtedy kolejność nawigacji fokusa jest ważna, bo może ułatwić lub utrudnić korzystanie ze strony. Informacje o kolejności pobierane są ze źródła dokumentu i nie mają nic wspólnego z wyglądem, który można przecież niemal dowolnie zmieniać za pomocą stylów. Jeżeli jednak taka rozbieżność się pojawi, to kolejność nawigacji można zaprogramować za pomocą atrybutu TABINDEX z parametrem którym są kolejne numery.

Sprawa bardzo się komplikuje, gdy dokument jest generowany dynamicznie po stronie klienta. Programiści stosują rozwiązania oparte o JavaScript lub Ajax, które mogą dodawać i usuwać elementy dokumentu, zaburzając jego strukturę. Tak się dzieje na przykład z “inteligentnymi formularzami”, gdzie wybranie lub zmiana wartości w jednej kontrolce powoduje zmiany w całym formularzu. Samo w sobie nie musi to generować problemów, ale trzeba zadbać o to, by pozmianie kolejność nadal była sensowna. Przy czym “sensowna” oznacza “zgodna z logiką formularza i oczekiwaniami projektanta”. Sprawdzić kolejność można zaś za pomocą narzędzia [WAVE](http://informaton.pl/?p=21) wybierając narzędzie “Structure/Order”