---
id: 330
title: 'Pisanie tekstu w zgodzie z WCAG 2.0'
date: '2012-10-27T15:54:03+02:00'
layout: post
guid: 'http://informaton.pl/?p=330'
permalink: /2012/10/27/pisanie-tekstu-w-zgodzie-z-wcag-2-0/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - czcionka
    - easy-to-read
    - kolor
    - kontrast
    - nagłówki
    - tekst
---

W poniższym artykule zebrałem wskazówki, które mogą być pomocne podczas pisania tekstów (artykułów, instrukcji, zawiadomień). Wskazówki pochodzą z WCAG 2.0 i przy każdej w nawiasie znajduje się odpowiednie kryterium sukcesu. Odnoszą się do tekstów pisanych zarówno na stronie internetowej, w edytorze MS Word jak i w programie do składu. Trzeba jedynie czasem poszukać odpowiedniego rozwiązania technicznego.

Wskazówki podzieliłem na trzy części, zgodnie z poziomami dostępności. Najniższy powinni stosować absolutnie wszyscy, średni – wszyscy kierujący informację do nieokreślonego odbiorcy, a najwyższy – dbający o najwyższy standard.

### Poziom A

1. Jeżeli w artykule używasz obrazów, grafik, animacji, filmów lub innych treści nie tekstowych – zaopatrz je w tekst alternatywny (SC 1.1.1).
2. Struktura informacji (rozdziały, listy) powinny być zdefiniowane programowo, a nie tylko wizualnie (SC 1.3.1). W wypadku stron internetowych oznacza to stosowanie prawidłowych znaczników, a nie formatowanie wyłącznie wizualne, a w edytorach tekstu – odpowiednich stylów.
3. Jeżeli wygląd treści ma wpływ na kolejność odczytu (kolumny, tabele) to kolejność powinna być odpowiednio zdefiniowana (SC 1.3.2). W praktyce oznacza to, że kolejność odczytu informacji maszynowo jest zgodna z kolejnością odczytu wzrokiem.
4. Unikaj stosowania pojęć odnoszących się do kształtu (kwadratowy, okrągły), wielkości (mały, duży), lokalizacji (w prawym górnym rogu) i orientacji (poziomy, pionowy) przekazując informację użytkownikowi (SC 1.3.3). Jeżeli użytkownik nie widzi lub informacja jest przekształcona w inny sposób, to te informacje mogą być nieaktualne.
5. Kolor nie może być jedynym wyróżnikiem ważnych informacji (SC 1.4.1). Ten rodzaj informacji zniknie jako pierwszy po wydrukowaniu w czerni i bieli.
6. Nadawaj dokumentom tytuły, które określają ich treść (SC 2.4.2). W szczególności chodzi tu o tytuł zawarty w metainformacjach dokumentu.
7. Jeżeli w tekście pojawiają się łącza, to ich treść powinna być zrozumiała w kontekście otoczenia ściśle z nim związanego (SC 2.4.4).
8. Zawsze określaj główny język dokumentu (SC 3.1.1).
9. Sprawdź, czy tekst po opublikowaniu przechodzi proces walidacji (SC 4.1.1).

### Poziom AA

1. Minimalny kontrast dla czcionek i tła powinien wynosić przynajmniej 4,5:1, a w wypadku dużych czcionek – 3:1 (SC 1.4.3).
2. Rozmiar czcionek można zwiększyć dwukrotnie bez użycia technologii asystujących, na przykład używając narzędzi w przeglądarce internetowej (SC 1.4.4).
3. Używaj tekstu, a nie obrazu tekstu (SC 1.4.5). Obrazem tekstu są na przykład skany umieszczone w kontenerze PDF lub DOC. Wyjątkowo można zastosować rozwiązanie graficzne, jeżeli użytkownik może dostosować sobie sposób wyświetlania treści, ale należy tego unikać.
4. Nagłówki i etykiety powinny opisywać zawartość (SC 2.4.6).
5. Określaj język fragmentów tekstów, jeżeli jest inny od języka całego dokumentu (SC 3.1.2).

### Poziom AAA

1. Kontrast pomiędzy tekstem a tłem powinien wynosić przynajmniej 7:1, a w wypadku dużych czcionek – 4,5:1 (SC 1.4.6).
2. Tekst można zaprezentować z uwzględnieniem następujących kryteriów: 1) użytkownik może ustawić sobie kolor tła i tekstu; 2) w linii jest najwyżej 80 znaków; 3) tekst nie jest wyjustowany; 4) interlinia wynosi przynajmniej 1,5 wiersza, a odstęp pomiędzy akapitami 1,5 interlinii; 5) rozmiar tekstu można powiększyć dwukrotnie bez konieczności przewijania treści w poziomie (SC 1.4.8).
3. Obraz tekstu jest stosowany wyłącznie do celów dekoracyjnych lub wówczas, gdy układ stanowi esencję informacji (SC 1.4.9).
4. Jeżeli w tekście znajduje się łącze, to jego znaczenie powinno być zrozumiałe także po wyjęciu go z kontekstu otoczenia (SC 2.4.9). Niedopuszczalne są zatem łącza o treści “dalej”, “kliknij”,, “więcej”, ponieważ samoistnie nic nie znaczą.
5. Używaj nagłówków do dzielenia treści na logiczne fragmenty (SC 2.4.10). Podzielenie tekstu na mniejsze części i nadanie im tytułów pozwoli na ich łatwiejsze czytanie.
6. Wyjaśniaj mało znane pojęcia i wyrazy, w tym żargonowe (SC 3.1.3).
7. Rozwijaj i wyjaśniaj stosowane w tekście skróty (SC 3.1.4).
8. Jeżeli tekst wymaga wykształcenia wyższego, niż gimnazjalne, zaproponuj jego prostszą wersję dostosowaną do tego poziomu (SC 3.1.5).
9. Jeżeli w tekście znajdują się słowa, których znaczenie zależy od wymowy, to zapewniona jest ta wymowa (SC 3.1.6) W wypadku języka polskiego taka sytuacja praktycznie się nie zdarza, ale warto zwrócić uwagę na wstawki w innych językach, szczególnie azjatyckich..