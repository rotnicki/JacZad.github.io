---
id: 773
title: 'Okno modalne wykorzystujące ARIA'
date: '2013-08-21T12:03:49+02:00'
layout: post
guid: 'http://informaton.pl/?p=773'
permalink: /2013/08/21/okno-modalne-wykorzystujace-aria/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - fokus
    - formularze
    - interfejs
    - klawiatura
    - okna
---

Okna modalne pozwalają na budowanie interfejsów webowych o znacznym podobieństwie do aplikacji instalowanych na komputerach. Programiści nie zawsze dbają o to, by takie elementy były dostępne, a jedynie starają się, by **wyglądały** podobnie do znanych skądinąd. Tymczasem takie okienka mogą być w pełni dostępne. Tutaj ciekawy [przykład zbudowania takiego okienka](http://accessibility.oit.ncsu.edu/training/aria/modal-window/), które jest w pełni dostępne.

Rozwiązanie korzysta ze standardowych rozwiązań zaproponowanych w technologii ARIA, na przykład DESCRIBEDBY i ALERT. Ciekawostką jest ingerowanie w obsługę klawiatury, by ograniczyć dostęp za pomocą klawiatury do elementów spoza okna. Klawisz Esc wyłącza okienko i pozwala powrócić do przeglądania strony.

Przy tej okazji autorzy wskazali na niedoskonałości interpretacji ARIA w różnych przeglądarkach. Jednak żadna z nich nie dyskwalifikuje rozwiązania, bo są to uchybienia stosunkowo niewielkie i o marginalnym znaczeniu. Podobne okna można wykorzystywać wszędzie tam, gdzie użytkownik operuje na niewielkich fragmentach strony, na przykład nanosząc na nie uwagi. Rozwiązanie bardzo mi się podoba i jest pełniejsze, niż zaproponowane kiedyś przeze mnie.