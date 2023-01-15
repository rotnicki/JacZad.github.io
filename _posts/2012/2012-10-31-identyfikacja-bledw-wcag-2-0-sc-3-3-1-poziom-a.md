---
id: 335
title: 'Identyfikacja błędów (WCAG 2.0 SC 3.3.1, poziom A)'
date: '2012-10-31T12:28:54+01:00'
layout: post
guid: 'http://informaton.pl/?p=335'
permalink: /2012/10/31/identyfikacja-bledw-wcag-2-0-sc-3-3-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - błędy
    - formularze
    - kolor
    - kontrast
    - tekst
    - wsparcie
---

Interakcja użytkownika z serwisem internetowym to często wprowadzanie danych. Użytkownik ma prawo do popełniania błędów, a system powiniengo wspomagać w ich poprawianiu. Na przykład przez jasną identyfikację.

Kryterium sukcesu 3.3.1 zobowiązuje do projektowania systemów do wprowadzania danych (formularzy) w taki sposób, by wykrywane w sposób automatyczny błędy były prezentowane użytkownikowi w postaci tekstowej. Skorzystają na tym:

- użytkownicy niewidomi,
- daltoniści,
- seniorzy,
- użytkownicy z małym doświadczeniem,
- użytkownicy z ograniczeniami kognitywnymi.

Zasada jest dosyć prosta: jeżeli system wykryje błąd we wprowadzonych przez użytkownika danych, to powinien go wskazać. Tak się dzieje bardzo często, ale nie zawsze. Czasem formularz zwraca komunikat w rodzaju “popraw dane”, bez wskazania miejsca, w którym błąd został popełniony. To bardzo utrudnia odnalezienie i poprawienie błędnie podanej informacji.

Warunkiem dodatkowym jest, by informacja o błędzie była zaprezentowana w formie tekstowej. Tutaj błędy popełniane są znacznie częściej, na przykład w postaci komunikatów “popraw dane zaznaczone na czerwono”. Wyróżnianie istotnych informacji kolorem jest ryzykownym zachowaniem i WCAG piętnuje to jako błąd dostępności. Można błędy oznaczyć kolorem czerwonym, ale przede wszystkim trzeba je wskazać słownie, na przykład “błędny numer PESEL”.

Oba błędy zawierał swego czasu formularz do rejestracji konta Apple ID. Po wprowadzeniu wszystkich danych osobowych niezbędnych do rejestracji otrzymywałem komunikat, by poprawić błędy zaznaczone na czerwono. Po konsultacji z osobą widzącą dowiedziałem się, że na czerwono zaznaczone jest moje nazwisko, ale co się nie podobało systemowi – tego już nie wiedziałem. Po pewnym czasie wpadłem na pomysł, by zastąpić literę “ż” literą “z” i teraz procedura poszła do przodu. Jednak gdyby nie wsparcie innych osób i pewna doza uporu, to pewnie konta bym nie założył.