---
id: 184
title: 'Dostęp za pomocą klawiatury (WCAG 2.0 SC 2.1.1, poziom A)'
date: '2012-08-26T08:53:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=184'
permalink: /2012/08/26/dostep-za-pomoca-klawiatury-wcag-2-0-sc-2-1-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - interfejs
    - klawiatura
    - myszka
    - niewidomi
---

Wydawałoby się, że w czasach urządzeń dotykowych każdy zdaje sobie sprawę, że nie każdy używa myszki. A przecież jeszcze dwie dekady temu i myszka była niezbyt często spotykana. Dlaczego zatem tak wielu programistów uważa, że wystarczy stosować jeden interfejs dostępowy?

Kryterium sukcesu 2.1.1 zobowiązuje do zapewnienia dostępu do każdej treści i funkcji za pomocą klawiatury. Czyniony jest jednak jeden wyjątek dla sposobu wprowadzania danych, gdzie oprócz określenia punktu początkowego i koncowego, ważna jest także droga pomiędzy nimi. Dosyć to zawiłe, więc za chwilę wyjaśnię, a z rozwiązania takiego skorzystają:

- użytkownicy z niedowładami rąk,
- użytkownicy terminali wyposażonych tylko w klawiaturę,
- użytkownicy niewidomi.

W zasadzie należy to kryterium rozumieć jako bezwzględny obowiązek projektowania serwisów internetowych w sposób umożliwiający pełną obsługę za pomocą klawiatury. Zatem niedopuszczalne jest, by zastosować technikę “przeciągnij i upuść” i zapomnieć o alternatywnym rozwiązaniu dostępnym z klawiatury, na przykład “kopiuj i wklej”. Należy też zapomnieć o elementach reagujących tylko na kursor myszy, jako o potencjalnie niedostępnych dla klawiatury.

Czas teraz na wytłumaczenie tego zawiłego zastrzeżenia. Otóż czasem – oprócz punktu początkowego i końcowego operacji – ważna jest także ścieżka dotarcia lub czas trwania. Pociągnięcie pędzlem to nie jest proste połączenie dwóch punktów, ale dosyć skomplikowana kombinacja kształtu, siły nacisku pędzla i szybkości malowania. W takim przypadku jest to nawet ważniejsze od samych punktów krańcowych. Podobnie – sterując modelem samochodu jadącego po ulicach miasta nie da się wyznaczyć po prostu dwóch punktów i wyrysować trasy przejazdu. To są przykładowe sytuacje dopuszczające rezygnację z pełnej dostępności za pomocą klawiatury.

Jednak to wyłączenie nie upoważnia projektantów do naciągania zasad i tworzenia dziwolągów programistycznych w rodzaju puzzli przesuwanych myszką, z których należy ułożyć hasło dostępu do konta. Jeżeli funkcję można zrealizować za pomocą interfejsu klawiaturowego, to tak powinno to być zrobione. To jednak wcale nie wyklucza stosowania także innych rozwiązań, w tym wykorzystujących myszkę, ale jako rozwiązania równoległe.

Powszechnie stosowany CMS [WordPress](http://www.wordpress.org) ma zaimplementowane układanie widgetów za pomocą myszki (przeciągnij i upuść). Jednak można włączyć w tym samym miejscu tryb ułatwionej dostępności i to samo zadanie można wykonać za pomocą klawiatury. To jest wzorcowe rozwiązanie problemu, chociaż zapomniano o zrealizowaniu go w innym miejscu, a mianowicie w sekcji udostępniania (share). Warto jednak zajrzeć do panelu administracyjnego WordPressa, by zobaczyć, jak to może wyglądać.