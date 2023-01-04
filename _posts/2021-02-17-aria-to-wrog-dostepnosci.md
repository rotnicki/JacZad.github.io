---
id: 2097
title: 'ARIA to wróg dostępności'
date: '2021-02-17T16:32:52+01:00'
layout: post
guid: 'http://informaton.blog/?p=2097'
permalink: /2021/02/17/aria-to-wrog-dostepnosci/
timeline_notification:
    - '1613575973'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - ARIA
    - badania
    - eskrzynka
    - Virtualo
    - WAVE
    - WebAIM
---

Twórcy technologii [ARIA (Accessible Rich Internet Application)](https://www.w3.org/TR/wai-aria-1.2/) na pewno nie spodziewali się, że tak się stanie ARIA miały być odpowiedzią na niekompletność HTML i rozbuchaną pomysłowość programistów. Miały być łatami na dziurawe pod względem dostępności strony internetowe. Tymczasem stały się często przyczyną braku dostępności.

ARIA stały się magicznymi zaklęciami, zamieniającymi niedostępny kod w kod wysokiej dostępności. Tak przynajmniej sądzi wielu projektantów, przeklejających kod z innych projektów. A czasem wstawiają atrybuty ARIA niszcząc dostępność. Tak było swego czasu w księgarni Virtualo, a teraz na stronie usługi [eSkrzynka Poczty Polskiej](https://eskrzynka.poczta-polska.pl/#/). W obu przypadkach chodzi o atrybut ARIA-HIDDEN, który ukrywa element przed technologiami asystującymi, czyli na przykład czytnikami ekranu. Efekt jest taki, że niewidomy użytkownik nawet nie wie o istnieniu przycisku, bo czytnik ekranu go ignoruje. Jaki cel miał programista stosując ten atrybut?

Okazuje się, że problem jest znacznie szerszy i nie dotyczy tylko polskich stron. Firma WebAIM przeprowadziła doroczne badanie miliona stron internetowych swoim narzędziem do automatycznego wykrywania błędów dostępności Wave. Wyniki badania są smutne, bo wynika z nich, że strony internetowe aż roją się od błędów dostępności, ale też że ich przybywa. Cały [raport](https://webaim.org/projects/million/) jest bardzo ciekawy, ale warto zwrócić uwagę na część poświęconą właśnie technologii ARIA. Używa jej 2/3 stron internetowych. I na stronach używających ARIA pojawia się o ponad 60% błędów dostępności więcej, niż na stronach bez tej technologii! Prościej – jak jest ARIA, to błędów dostępności jest więcej.

Główną zasadą stosowania ARIA, jest by jej nie stosować bez bardzo ważnego powodu. Powód stosowania akurat ARIA-HIDDEN musi zaś być szczególnie dobry, bo jest to atrybut wysokiego ryzyka. O ile z wieloma błędami dostępności można sobie poradzić, to tego ominąć się nie da. No dobrze… Można to zrobić narzędziami deweloperskimi, ale to wyższa szkoła jazdy.

Zaczyna pojawiać się potrzeba, by w czytnikach ekranu umiejscowić opcję wyłączenia obsługi ARIA. A to już bardzo poważny sygnał, że technologia mająca służyć dostępności, może ją niszczyć. Wielka szkoda, bo czasem naprawdę się przydaje.