---
id: 1211
title: 'Tajemniczy wskaźnik dostępności Utilitii, czyli o ograniczonym zaufaniu do automatów'
date: '2015-01-09T14:26:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=1211'
permalink: /2015/01/09/tajemniczy-wskaznik-dostepnosci-utilitii-czyli-o-ograniczonym-zaufaniu-do-automatow/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - narzędzia
    - Utilitia
    - 'WCAG 2.0'
---

Coraz bardziej utwierdzam się w przekonaniu, że należy zamknąć dostęp do narzędzi automatycznie badających dostępność dla ignorantów. Ludzie są zbyt leniwi, by temat zgłębić, a automaty dają odpowiedzi zbyt proste i niepewne. Opiszę to na przykładzie [Utilitii](https://walidator.utilitia.pl/), której jestem wyrodnym ojcem. Jest to właśnie automat, do którego ignorant wrzuca adres strony internetowej i wyciąga tylko wskaźnik dostępności, którym potem wali na lewo i prawo. A zagłębić się w temat to nie łaska?!

Utilitia jest ciekawym narzędziem internetowym i to opracowanym w Polsce. Pozwala na wykonywanie automatycznych testów dostępności stron internetowych. Sęków zaś jest w tym kilka.

Testy badają tylko część dostępności i to wcale nie tak wielką. Nie ma automatu i pewnie długo jeszcze nie będzie, który pozwoliłby na pełne i pewne zbadanie dostępności, bo jest to po prostu zbyt trudne. Trzeba byłoby zaprząc do tego sztuczną inteligencję i symulatory użytkowników. A zatem wynik otrzymany z Utilitii w postaci raportu jest prawdziwy, ale nie jest pełny. Dlatego nawet serwis mający wskaźnik maksymalny, czyli 10.0 może nie być dostępny.

Algorytm oceniający został przygotowany przez ludzi, a ci też mogą się mylić. Ja uważam, że w tym algorytmie są błędy, bo sprawdziłem to na swoim własnym serwisie. Otóż otrzymał on ocenę 7.2, czyli stosunkowo niską. Nie twierdzę, że jest idealny pod względem dostępności, ale nie jest też z nim tak źle, więc sprawdziłem szczegóły. Wygenerowałem raport, w którym chciałem obejrzeć tylko błędy. I co się okazało? Otóż Utilitia wskazuje jako błędy miejsca, które błędami wcale nie są. Można od biedy uznać, że należy tam ostrzec przed możliwością wystąpienia błędu, ale tylko tyle.

Aby nie być gołosłownym, w raporcie znalazłem następujące błędy dostępności:

- Obecność bloku informującego o lokalizacji w obrębie strony (okruszki): Nie znaleziono bloku”. Okruszki nie są jedynym sposobem na wskazanie użytkownikowi miejsca w serwisie. Ich brak nie może być zatem traktowany jako błąd. A zresztą – to jest wymaganie z poziomu AAA WCAG 2.0.
- Prymitywne formatowanie: Akapit jest pusty. W ogóle nie mam pojecia, które kryterium sukcesu jest tu złamane. Jest to z pewnością niedoróbka programistyczna, ale błąd dostępności…
- Prymitywne formatowanie: Tabela nie ma nagłówków. To byłby błąd, gdyby takie nagłówki były w tabeli potrzebne. W tabeli w moim serwisie nie są potrzebne, bo jest to element layoutu.
- Linki: Treść linku nie jest tożsama z innymi, prowadzącymi do tego samego miejsca. Wydaje się, że nie musi być tożsama. Problematyczna jest inna sytuacja, gdy link o tej samej etykiecie (np. “Kontakt”) prowadzi w różne miejsca. Ja w każdym razie tego błędu nie uznaję.
- Linki: Treść linku stanowi fragment adresu URL. A nie może? Nie potrafię wymyślić, które z kryteriów sukcesu WCAG 2.0 zostało tu naruszone.

Utilitia pozwoliła mi na znalezienie kilku błędów dostępności, to znaczy brak etykiety do pola wyszukiwania, zbyt mały kontrast w dwóch miejscach oraz błędy w kodzie HTML, które pochodzą z wtyczek. Z ponad 250 wygenerowanych błędów jest to zaledwie kilkanaście prawdziwych, a zatem wynik 7.2 jest nieprawdziwy. Ja potrafię zinterpretować wyniki raportu, ale niektórzy wezmą bezkrytycznie dwie cyferki rozdzielone kropką i użyją ich bez wahania i refleksji. Może zatem lepiej zrezygnować z tego wskaźnika, skoro niczego nie pokazuje… Swoją drogą – ciekawe ile punktów miałby mój serwis, gdyby nie wliczać w to wątpliwych błędów. Sprawdziłem i wyszło 8.0, co nadal jest dosyć słabe. Szewc jednak często chodzi bez butów.

Wiertarka sama nie wierci otworów, aparat fotograficzny nie robi sam zdjęć, nawet z samowyzwalaczem. Utilitia i inne narzędzia służą ludziom, ale ludzie muszą umieć się nimi posłużyć. Oferma nie zrobi dobrego zdjęcia nawet najlepszym aparatem, chyba że przypadkiem. I odwrotnie – mistrz fotografii nie zrobi konkursowej fotki za pomocą dziecięcej zabawki dołączanej do czasopisma. Dopiero dobre narzędzie w rękach fachowca może pokazać swoją siłę. Nad Utilitią trzeba nadal pracować, a jej użytkownicy powinni się uczyć o dostępności trochę więcej, niż odczytywanie ułamka dziesiętnego. Inaczej dostępnego Internetu nie zbudujemy.