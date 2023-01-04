---
id: 2349
title: 'Mity cyfrowej dostępności &#8211; łącza'
date: '2021-06-05T18:48:21+02:00'
excerpt: 'Dzisiaj próbuję rozprawić się z kolejnym mitem krążącym w środowisku rzemiosła dostępnościowego. Piszę o wyższości jednych łączy nad drugimi, a raczej o braku takiej wyższości.'
layout: post
guid: 'http://informaton.blog/?p=2349'
permalink: /2021/06/05/mity-cyfrowej-dostepnosci-acza/
publicize_linkedin_url:
    - ''
timeline_notification:
    - '1622911705'
publicize_twitter_user:
    - jaczad
categories:
    - artykuły
tags:
    - automaty
    - łącza
    - tekst
    - Utilitia
    - WCAG
---

Co jakiś czas dowiaduję się z różnych źródeł, że pewien rodzaj łączy jest niedostępny lub niezgodny z WCAG, Jeżeli znam źródło, to staram się dopytać, dlaczego tak uważa. Nigdy nie dostałem satysfakcjonującej odpowiedzi. Dlatego poniżej opiszę, dlaczego nie uważam, by to był błąd dostępności.

Chodzi zaś o łącza, w których elementem klikalnym jest adres do zasobu w sieci, czyli na przykład <https://informaton.blog/2015/01/09/tajemniczy-wskaznik-dostepnosci-utilitii-czyli-o-ograniczonym-zaufaniu-do-automatow/>. W tym podlinkowanym artykule publicznie pytam, na czym polega błąd dostępności i wciąż nie znam odpowiedzi. Zdaniem części specjalistów to łącze może wyglądać tylko tak: [TAJEMNICZY WSKAŹNIK DOSTĘPNOŚCI UTILITII, CZYLI O OGRANICZONYM ZAUFANIU DO AUTOMATÓW](https://informaton.blog/2015/01/09/tajemniczy-wskaznik-dostepnosci-utilitii-czyli-o-ograniczonym-zaufaniu-do-automatow/). Ewentualnie może to być inny tekst, ale nie adres URI.

W WCAG mamy takie odniesienie do łączy:

> Kryterium sukcesu 2.4.4 Cel łącza (w kontekście)
> 
> Cel każdego łącza może wynikać z samej treści łącza lub z treści tekstu powiązanego z kontekstem łącza określonym programowo , poza tymi przypadkami, kiedy cel łącza i tak byłby niejasny dla użytkowników.

Jest jeszcze kryterium sukcesu 2.4.9, różniące się od poprzedniego tylko tym, że nie musi być w kontekście, czyli jego sens musi być jasny samoistnie. Więcej na ten temat nie znalazłem.

Nie wiem, skąd pojawiła się ta teza o wyższości łączy maskowanych nad jawnymi i to na dodatek jako błąd dostępności. Z WCAG nie mogę tego wyczytać. Od biedy zrozumiałbym, gdyby na końcu nie było zastrzeżenia „poza tymi przypadkami, kiedy cel łącza i tak byłby niejasny dla użytkowników.” Ja to rozumiem tak, że łącze nie musi być dostępniejsze dla użytkownika z niepełnosprawnością, niż dla innych. Oczywiście gdyby uznać, że z takim łączem jest coś nie tak.

Łącze ma funkcję taką samą od powstania Internetu: trzeba w nie kliknąć, by wywołać jakiś zasób, najczęściej inną stronę internetową. To działa doskonale. Może zatem chodzi o to, że adres jest trudny do czytania?.. Trudno dociec, a za to mogę wskazać wadę takiego maskowania łączy.

Taką wadą jest zaginięcie informacji o adresie w przypadku niektórych przekształceń. Na straży stoi tu wytyczna:

> Wytyczna 1.3 Możliwość adaptacji
> 
> Twórz treści, które mogą być prezentowane na różne sposoby bez utraty informacji czy struktury.

Tutaj informacja zaginie, jeżeli zostanie przekształcona do wydruku na papierze, po wykonaniu zrzutu ekranu, skopiowaniu tekstu z przeglądarki lub dokumentu i pewnie także w innych sytuacjach. Patrząc od tej strony, można uznać że to właśnie markowane adresy są niedostępne, a jawne – są dostępne i przetwarzalne. Nie będę się jednak o to bił.

To jest kolejne miejsce, gdzie zachować należy zdrowy rozsądek. Maskowane łącza wyglądają ładniej, bo adres URI to ciąg różnych znaków, często bez żadnej sensownej treści. Z kolei należy pamiętać, że dokumenty mające dużą szansę na wyplucie z drukarki powinny mieć te adresy raczej jawne. Dlatego uważam, że oba podejścia mają swoje wady i zalety, ale żadne też nie powinno być traktowane jako błąd.