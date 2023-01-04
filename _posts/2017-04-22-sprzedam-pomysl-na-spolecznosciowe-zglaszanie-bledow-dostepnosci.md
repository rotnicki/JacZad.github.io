---
id: 1650
title: 'Sprzedam pomysł na społecznościowe zgłaszanie błędów dostępności'
date: '2017-04-22T14:19:26+02:00'
layout: post
guid: 'http://informaton.pl/?p=1650'
permalink: /2017/04/22/sprzedam-pomysl-na-spolecznosciowe-zglaszanie-bledow-dostepnosci/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - błę
    - Chrome
    - Firefox
    - 'open source'
    - wtyczka
---

Chodzi za mną ten pomysł już kilka lat i jakoś sam go nie umiałem zrealizować. Podjąłem nawet z góry przegraną próbę, by zrealizować go samodzielnie, co wymagało uczenia się zupełnie nowych dla mnie technologii. Poddałem się i postanowiłem pomysł opisać, by zrealizował go ktoś posiadający wiedzę lub determinację większą od mojej.

Ponieważ nie jestem programistą, to mogę spokojnie napisać, że pomysł jest łatwy do zrealizowania. Polega na przygotowaniu wtyczki do przeglądarki internetowej (Firefox lub Chrome) zbierającej zgłoszenia o błędach dostępności na stronach internetowych. Zgłoszenia mają być wysyłane do serwera agregującego dane, a tam aplikacja zajmie się prezentacją danych w postaci raportów gotowych do wysłania. Prawda, że proste!

Wtyczka powinna być możliwie prosta w użyciu. Użytkownik wybiera z menu kontekstowego lub przez kliknięcie na ikonkę wtyczkę i zaznacza znalezione problemy. Zestaw musi być prosty i stosunkowo krótki, by nie zanudzić odniesieniami do WCAG 2.0. Na przykład “kod obrazkowy CAPTCHA”, “brak obsługi klawiaturą”, “zbyt mały kontrast”, “zbyt małe czcionki”, “automatycznie uruchamiany dźwięk” itd. Wtyczka powinna też zabrać sobie adres URL zgłaszanej strony oraz identyfikator użytkownika. Ten identyfikator powinien być unikalny, a służyć będzie tylko do tego, by zgłaszający mógł podejrzeć, co dzieje się ze zgłoszeniem.

Wszystko to ląduje na serwerze zbierającym zgłoszenia i przetwarzającym je odpowiednio. Po pierwsze – według domeny segreguje zgłoszenia na te dotyczące konkretnego serwisu. Po drugie – tworzy raporty na temat zgłaszanych błędów. Po trzecie – tworzy wiadomość do właściciela serwisu z informacją o problemach i sugestią, by się ogarnął. Po czwarte – pokazuje zasoby w wygodny dla czytelnika sposób, a więc często zgłaszane serwisy, często pojawiające się błędy, najaktywniejsi zgłaszający itp.

Zdaję sobie sprawę, że procesu nie da się do końca zautomatyzować. Jednak automatyczne walidatory nie rozwiązują problemu, a audyty na zamówienie odbywają się tylko wtedy, gdy ktoś je zamówi. To oznacza poprawę sytuacji w wielkich serwisach administracji publicznej i zupełny marazm w mniejszych. Poza tym jakoś mam przeczucie, że ludzie korzystają z zupełnie innych serwisów, niż się wydaje urzędnikom. System może być podatny na trolling i to też trzeba przewidzieć. Mam już w głowie pewne rozwiązania, którymi chętnie i bezpłatnie podzielę się z chętnymi do wdrożenia. Tu tylko szepnę, że pomysł opiera się o renomę.

Może pomysł weźmie jakaś organizacja pozarządowa albo firma komercyjna. A może uczelnia wyższa lub wręcz jakiś student szukający tematu na pracę inżynierską. A może jakaś grupa fanatyków <span lang="en">open source zaparkuje jako otwarty projekt. Ja chętnie zgłaszam się do współpracy i będę się ścigał z innymi na znajdowanie błędów. Podoba się Wam pomysł? Jeżeli tak, to szerujcie, lajkujcie i co tam jeszcze robi się w tych internetach.</span>