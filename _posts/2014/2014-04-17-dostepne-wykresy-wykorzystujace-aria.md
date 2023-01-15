---
id: 1020
title: 'Dostępne wykresy wykorzystujące ARIA'
date: '2014-04-17T11:59:53+02:00'
layout: post
guid: 'http://informaton.pl/?p=1020'
permalink: /2014/04/17/dostepne-wykresy-wykorzystujace-aria/
enclosure:
    - "http://paypal.github.io/amcharts-accessibility-plugin/media/SR_amChartsAccessibility.mov\n7002112\nvideo/quicktime\n"
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - JavaScript
    - klawiatura
    - wykresy
---

Swego czasu opisywałem w jaki sposób można osadzać na stronach [dostępne wykresy](http://informaton.pl/?p=88). Jednak moja metoda – chociaż skuteczna – jest biedniutka w porównaniu z rozwiązaniem, które niedawno odkryłem. Jest to [amCharts Accessibility Plugin](http://paypal.github.io/amcharts-accessibility-plugin/), czyli rozszerzenie dla komercyjnego narzędzia do tworzenia wykresów na żywo [AmCharts](http://www.amcharts.com/). Sądząc po liście firm – jest to narzędzie dobre i popularne, a wykresy są generowane na żywo za pomocą biblioteki JavaScript.

Na czym polega moc tkwiąca w AAP? Na dodaniu ról ARIA i obsługi za pomocą klawiatury. Statyczny obrazek wykresu zamienia się wtedy w interaktywnyobiekt, po którym można się przemieszczać za pomocą klawiatury. Oczywiście działa to tylko z czytnikiem ekranu, na przykład NVDA, bo i rozszerzenie przeznaczone jest przede wszystkim dla niewidomych użytkowników. [Wersja demonstracyjna takiego wykresu](http://paypal.github.io/amcharts-accessibility-plugin/demo.html)pozwala obejrzeć, jak to działa. Można też obejrzeć dołączony do opisu [screencast](http://paypal.github.io/amcharts-accessibility-plugin/media/SR_amChartsAccessibility.mov). Szkoda jedynie, że sama podstawowa biblioteka jest komercyjna, bo chętnie bym poeksperymentował.