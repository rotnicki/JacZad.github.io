---
id: 931
title: 'Dostępność dla blogerów'
date: '2014-01-19T15:00:24+01:00'
layout: post
guid: 'http://informaton.pl/?p=931'
permalink: /2014/01/19/dostepnosc-dla-blogerw/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - blogi
    - klawiatura
    - kontrast
    - multimedia
    - napisy
    - PSBV
    - tekst
    - 'WCAG 2.0'
---

Ponieważ pojawiło się na rynku zupełnie nowe [Polskie Stowarzyszenie Blogerów i Vlogerów](http://psbv.pl/), to w prezencie przygotowałem dla nich listę porad. Mają one pomóc w tworzeniu bardziej dostępnej blogosfery, bo obecnie woła ona o pomstę do nieba. Braki tekstów alternatywnych, napisów do filmów, pisanie hermetycznym językiem i stosowanie przedziwnych rozszerzeń sprawia, że blogi i całe serwisy oparte o podobne mechanizmy są mało dostępne. Może zatem ktoś skorzysta dla dobra społecznego.

1. Dodając multimedia do bloga pamiętaj, by przypisać do nich tekst alternatywny. Odpowiednie pole edycyjne znajdziesz w edycji pliku w galerii plików. Tekst alternatywny ma dokładnie przekazywać informacje na temat dołączonego pliku. Pamiętaj, że tekst alternatywny to nie podpis! Ma on **\*opisać\*** niewidomemu użytkownikowi to, co widać na ekranie, a niesłyszącemu to, co słychać z głośników.
2. Dodając podcast lub inne medium zawierające tylko dźwięk dodaj także jego pełną transkrypcję w postaci tekstu. W ten sposób zapoznają się z nim osoby niesłyszące.
3. Publikując film, na przykład w YouTube lub na Vimeo od razu dodaj do niego napisy. Oba serwisy na to pozwalają, a w ten sposób zadbasz o dostęp dla osób niesłyszących.
4. Publikując filmy postaraj się, by z dialogów i komentarzy z offu wynikało to, co dzieje się na ekranie. Jeżeli to nie wystarcza, dodaj ścieżkę audiodeskrypcji. To pomoże zrozumieć informacje użytkownikom niewidomym.
5. Nie stosuj zabezpieczeń typu CAPTCHA, szczególnie polegających na odczytywaniu znaków ze zniekształconego obrazka. Jest to utrudnienie dla wszystkich użytkowników, a dla niewidomych jest nie do przejścia. Uwierz też, że kod dźwiękowy nie rozwiązuje sprawy.
6. Do prezentacji tabel używaj odpowiednich narzędzi (znaczników), a nie wklejaj zrzutów ekranu.
7. Unikaj informowania użytkownika za pomocą pojęć związanych z kształtem (okrągły przycisk), rozmiaru (mała ikona), wzrokowa lokalizacja (w menu po lewej stronie), orientacji w przestrzeni (pionowy pasek) lub dźwięk (po usłyszeniu klaksonu). Tego rodzaju instrukcje są bezużyteczne dla osób niewidomych, a w przypadku dźwięku – dla niesłyszących.
8. Istotne informacje mogą być wyróżniane kolorem, ale powinny być wyróżnione także na inny sposób, na przykład przez pogrubienie.
9. Dźwięk, w tym także w filmach, nie powinien być odtwarzany automatycznie po wejściu na stronę. Może to utrudnić lub uniemożliwić korzystanie ze strony osobom używającym syntezatorów mowy.
10. Pomiędzy tekstem a tłem należy zachować odpowiednio duży kontrast, wynoszący przynajmniej 4,5:1 lub lepiej 7:1.
11. Sprawdź, czy za pomocą przeglądarki można powiększyć tekst na stronie przynajmniej dwukrotnie. Służy do tego najczęściej skrót Ctrl “+”.
12. Prezentując informacje tekstowe nigdy nie rób tego za pomocą grafiki. Takiego tekstu nie można powiększyć, zmienić kolorystyki lub krojów czcionek.
13. Wszystkie elementy interfejsu (linki, przyciski, pola formularzy) muszą być dostępne z poziomu klawiatury.
14. Unikaj elementów, które ograniczają czasowo użytkownika. Pojawiająca się i znikająca, przewijająca się informacja może nie zostać zauważona przez część użytkowników. Wygasające sesje, odświeżające się elementy mogą sprawić, że użytkownik się nie wyrobi w określonym czasie.
15. Unikaj treści, które mogą wywołać atak padaczki. Treści migające częściej niż trzy razy na sekundę oraz zawierające dużo koloru czerwonego są szczególnie niebezpieczne.
16. Zapewnij mechanizm pozwalający na pominięcie bloków stałych na stronie, na przykład menu i wyszukiwarki. Służą do tego skiplinki, landmarki i nagłówki. Skiplinki to linki umieszczane na początku strony przenoszące fokus w odpowiednie miejsce. Jeżeli ich nie masz, a używasz WordPressa, możesz skorzystać z wtyczki WP Accessibility.
17. Każda podstrona serwisu powinna mieć unikalny tytuł wyświetlany na belce tytułowej przeglądarki. WordPress posiada taką funkcjonalność od początku, chociaż można ją zepsuć przez użycie wtyczek lub nieporadne grzebanie w kodzie źródłowym.
18. Dłuższe teksty dziel na mniejsze części i każdemu fragmentowi nadawaj tytuł w nagłówku odpowiedniego poziomu. W ogóle stosuj nagłówki do opisywania treści na stronie, co pomoże w nawigacji i zrozumieniu treści.
19. Fokus przemieszczany za pomocą klawiatury powinien przemieszczać się w sposób logiczny i oczekiwany. Służy do tego klawisz Tab, więc możesz to sprawdzić samodzielnie. Pamiętaj też, że ten fokus powinien być zawsze widoczny, a jego ukrywanie za pomocą stylów jest błędem.
20. Cel, do którego prowadzą używane w serwisie linki, powinien wynikać z ich treści lub najbliższego otoczenia. Dlatego unikaj linków w rodzaju “tutaj”, “kliknij”, “pobierz” i podobnych, które nie mają znaczenia poza kontekstem.
21. Daj użytkownikowi wiele możliwości odnalezienia informacji stosując hierarchiczne menu, kategorie, tagi, wpisy sugerowane, wyszukiwarkę.
22. Język tekstu na stronie powinien być zawsze zdefiniowany. W wypadku języka polskiego w kodzie powinien znaleźć się atrybut LANG=”pl” przy znaczniku HTML. Jeżeli w treści znajdą się wstawki w innych językach, to należy je także zdefiniować. Można to zrobić w kodzie otaczając je znacznikiem SPAN: &lt;span lang=”en”&gt;…&lt;/span&gt;. Dzięki temu syntezatory mowy będą się przełączać na właściwy język.
23. Treść nie powinna się zmieniać automatycznie podczas wprowadzania danych lub przeniesieniu fokusa na jakiś element. Dotyczy to także automatycznego otwierania nowej strony, nowej karty, zewnętrznej aplikacji, zmiany języka i innych zachowań, których użytkownik może się nie spodziewać.
24. Stosuj konsekwentną nawigację i identyfikację wizualną na każdej podstronie serwisu. Niech menu są zawsze w tym samym miejscu i pozycje w menu nie przemieszczają się bez wyraźnego żądania użytkownika.
25. Jeżeli użytkownik ma możliwość wprowadzania danych, na przykład wpisywania komentarza, to wykryty automatycznie błąd popełniony przez niego,powinien być mu zakomunikowany w postaci informacji tekstowej. Samo zaznaczenie kolorem nie wystarczy.
26. Wszystkie pola formularzy powinny być zaopatrzone w etykiety powiązane z danym polem oraz instrukcje wyjaśniające sposób wprowadzania danych. Nie licz na to, że każdy użytkownik sam się domyśli, co ma wpisać.
27. Postaraj się, by Twój serwis dawał się parsować w walidatorze. Chodzi o to, by był zgodny ze standardami internetowymi takimi jak HTML, HTML5, CSS, RSS i innymi.