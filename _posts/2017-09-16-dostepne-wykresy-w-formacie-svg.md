---
id: 1746
title: 'Dostępne wykresy w formacie SVG'
date: '2017-09-16T11:00:12+02:00'
layout: post
guid: 'http://informaton.pl/?p=1746'
permalink: /2017/09/16/dostepne-wykresy-w-formacie-svg/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - SVG
    - tabele
    - wykresy
---

Dostępność treści cyfrowych to wciąż dosyć hermetyczny obszar. Dzisiaj jednak zamierzam podlinkować coś jeszcze bardziej hermetycznego, chociaż przydatnego. Jest to artykuł *[Accessible SVG line graphs – Tink](https://tink.uk/accessible-svg-line-graphs/)*Format SVG (Scalable Vector Graphic) jest jednym z formatów opracowanych przez W3C i stał się standardem w tworzeniu grafiki wektorowej, jak JPG i PNG stały się standardem dla grafiki rastrowej. Mimo to jest on wciąż dosyć rzadko stosowany, być może z powodu zbyt małej liczby narzędzi. Ponieważ jednak jest on aplikacją XML, to można źródło uzupełnić o atrybuty ARIA i w ten sposób zaprojektować dostępny wykres, co właśnie opisuje artykuł. Metoda jest prosta: pod wykresem kryje się tabela z danymi, w której zdefiniowano wiersze i komórki. Coś podobnego można zrobić także w HTML, co swego czasu [opisałem](http://informaton.pl/artykuly/tworzenie-opisw-alternatywnych-grafiki-na-stronach-internetowych/). Zaletą opisywanego rozwiązania jest jednak fakt, że wszystkie dane zawarte są w samym pliku SVG, który można swobodnie przenosić i osadzać w innych miejscach, bez utraty dostępności.