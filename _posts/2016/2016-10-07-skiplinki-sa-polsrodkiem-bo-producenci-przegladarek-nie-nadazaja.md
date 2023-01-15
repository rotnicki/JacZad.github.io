---
id: 1564
title: 'skiplinki są półśrodkiem, bo producenci przeglądarek nie nadążają'
date: '2016-10-07T12:06:24+02:00'
layout: post
guid: 'http://informaton.pl/?p=1564'
permalink: /2016/10/07/skiplinki-sa-polsrodkiem-bo-producenci-przegladarek-nie-nadazaja/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - HTML5
    - landmarki
    - nawigacja
    - skiplinki
---

Jednym z kryteriów sukcesu w specyfikacji WCAG 2.0 jest to wymagające zaimplementowania sposobu na pominięcie stałych elementów strony. Chodzi o to, by użytkownik korzystający ze strony w sposób sekwencyjny miał szybszy dostęp do głównej treści. Takimi osobami są użytkownicy niewidomi, niesprawni manualnie oraz część użytkowników urządzeń mobilnych.

Rozwiązania są cztery: skiplinki, landmarki, znaczniki struktury z HTML5 i nagłówki. Ja jestem ogromnym zwolennikiem stosowania landmarków i elementów semantycznych zaprojektowanych w HTML5. Skiplinki zawsze wydawały mi się pewnego rodzaju obejściem problemu, a nagłówki służą tylko osobom niewidomym. Nagłówki są co prawda częścią semantyki dokumentu, ale nie mogą z nich skorzystać inni użytkownicy. Jak wspomniałem – skiplinki od zawsze budziły moje podejrzenia, ale nie wiedziałem dlaczego. Dzisiaj przeczytałem [artykuł na ten temat](https://www.epinova.no/en/blog/save-us-from-skip-links/) i olśniło mnie. Autor wykłada to bardzo prosto, a jednocześnie wskazuje winnego.

Według niego skiplinki są hackowaniem, a nie rozwiązaniem problemu. Prawdziwym rozwiązaniem powinna być semantyka strony, czyli znaczniki MAIN i inne opisane w HTML5. A jeżeli się nie da – stosowanie landmarków. Być może dałoby się stosować obie techniki jednocześnie. Odpowiednie mechanizmy zaszyte w przeglądarkach powinny pozwalać na przechodzenie pomiędzy obszarami semantycznymi lub landmarkami, a wtedy skiplinki w ogóle przestają być potrzebne. No i tu pojawiają się winni braku takich rozwiązań – producenci przeglądarek. Nie implementują oni skrótów klawiaturowych pozwalających na pomijanie treści, więc użytkownicy nie mają z czego korzystać. I dopóki ta sytuacja się nie zmieni, skiplinki będą musiały nadal być stosowane.