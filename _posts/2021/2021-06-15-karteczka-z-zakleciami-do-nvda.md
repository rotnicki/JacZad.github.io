---
title: 'Karteczka z zaklęciami do NVDA'
date: '2021-06-15T15:21:25+02:00'
excerpt: 'Jeżeli ktoś potrzebuje, to może skorzystać z żółtej karteczki ze skrótami do NVDA.'
layout: post
categories:
    - artykuły
tags:
    - NVDA
    - 'skróty klawiszowe'
    - webinarium
---

Tydzień temu odbył się webinar na temat korzystania z czytnika ekranu NVDA. Tempo było chyba zbyt duże, bo uczestnicy nie wszystko zapamiętali lub zapisali. Poniżej zatem przypominajki.

## Instalacja i wstępna konfiguracja

Czytnik ekranu NVDA można pobrać ze strony [NV Access](https://www.nvaccess.org/). Jest to program bezpłatny, o otwartym kodzie i można go spokojnie instalować na dowolnym komputerze z Windows.

Po zainstalowaniu warto go skonfigurować. Ustawienia można wywołać klikając myszką na ikonę w zasobniku lub skrótem klawiszowym Insert n.

1. W zakładce “Ogólne” odznacz wszystkie opcje.
2. W zakładce “Klawiatura” wybierz układ klawiatury “laptop” i klawisz modyfikujący CapsLock.
3. W zakładce “Tryb czytania” wyłącz opcję “Użyj układu ekranu, o ile to możliwe”.

## Podstawowa obsługa

Czytnika ekranu używaj tylko za pomocą klawiatury. Najlepiej odłącz myszkę i touchpad.

Klawisz NVDA to specjalny klawisz do wprowadzania poleceń NVDA. Domyślnie jest to klawisz Insert, a dodatkowo – po włączeniu – Capslock.

Nvda możesz uruchomić skrótem Ctrl + Alt + d. Zamknąć zaś możesz skrótem NVDA q.

## Systemowe skróty klawiszowe

W systemie Windows można korzystać z aplikacji za pomocą klawiatury. Poniżej znajdziesz listę najważniejszych skrótów.

1. Tab – przemieszcza fokus na kolejny element.
2. Shift + Tab przemieszcza fokus na poprzedni element.
3. Alt lub F10 przenosi fokus na menu górne aplikacji.
4. Shift + F10 rozwija menu kontekstowe.
5. Strzałki w lewo, prawo, górę i dół przemieszczają fokus między różnymi elementami, na przykład pozycjami w menu, ikonami itp.
6. Enter aktywuje element, na przykład przycisk, łącze.
7. Spacja zaznacza pola wyboru, pola opcji, aktywuje przyciski.
8. Alt + Tab przełącza między dwoma ostatnio otwartymi aplikacjami.
9. Windows – Tab otwiera okno widoku zadań, gdzie można wybrać dowolną aplikację.
10. Ctrl + Tab przełącza pomiędzy zakładkami, o ile są obecne.
11. Esc pozwala zamknąć menu, okno itp.

## Skróty klawiszowe NVDA

Czytnik ekranu NVDA ma bardzo dużo własnych skrótów klawiszowych. Poniżej znajdziesz tylko najbardziej potrzebne. Wszystkie skróty znajdziesz w menu Pomoc – Wykaz skrótów poleceń.

1. NVDA + Tab odczytuje element, na którym znajduje się fokus.
2. NVDA + Spacja przełącza NVDA między trybem formularza i czytania.
3. NVDA + Ctrl + k wyświetla ustawienia klawiatury.
4. NVDA + Ctrl + d wyświetla okno ustawień formatowania dokumentów.
5. NVDA + Ctrl + v wyświetla ustawienia mowy.
6. NVDA + p zmienia poziom interpunkcji, czyli odczytywania znaków innych niż litery i cyfry.
7. NVDA + t odczytuje tytuł okna.
8. NVDA + n otwiera menu NVDA.

## Tryby pracy NVDA

Nvda może pracować w jednym z dwóch trybów. Różnią się one pod względem funkcji i obsługi klawiaturą. Do przełączania się pomiędzy trybami służy skrót NVDA + Spacja. Każdy z trybów sygnalizowany jest innym dźwiękiem podczas przełączania. W NVDA istnieje jeszcze jeden, dość specjalny tryb nawigowania po obiektach. Jednak tutaj go nie omówię.

### Tryb formularzy

Jest to podstawowy tryb pracy z aplikacjami. Zastosowanie mają skróty klawiszowe opisane w sekcji o systemowych skrótach klawiszowych. W tym trybie NVDA odczytuje tylko te elementy, które przyjmują fokus klawiatury oraz elementy ściśle z nimi powiązane. NVDA odczyta zatem informację, że znajduje się na przycisku oraz etykietę tekstową, o ile jakaś jest powiązana z przyciskiem. Czytnik ekranu nie ma dostępu do treści, na których nie można umieścić fokusu.

### Tryb czytania

Jest to specjalny tryb pracy czytnika ekranu, pozwalający na dotarcie do elementów, które nie przyjmują fokusa. Jest on szczególnie istotny na stronach internetowych, w aplikacjach wykorzystujących kontrolki webowe (na przykład MS Teams). Można go użyć także w edytorze Word i Adobe Reader.

W trybie czytania funkcje klawiszy zmieniają się. Klawisze strzałek pozwalają przemieszczać się po dokumencie podobnie jak w edytorze tekstu. Za to nie zmieniają wartości w kontrolkach. W trybie czytania nie da się edytować treści.

W trybie czytania wykorzystywane są jednoznakowe skróty. Pozwalają na szybką nawigację po elementach charakterystycznych dla stron internetowych. Oto kilka wybranych, które przemieszczają fokus do przodu. Dodanie klawisza Shift sprawi, że fokus będzie się przemieszczał do tyłu.

- h – przemieszczanie między nagłówkami;
- g – przemieszczanie między grafikami;
- t – przemieszczanie między tabelami;
- d – przemieszczanie między punktami orientacyjnymi;
- l – przemieszczanie między listami;
- e przemieszczanie między polami edycyjnymi;
- x przemieszczanie między polami wyboru;
- b przemieszczanie między przyciskami.

## Dodatkowe narzędzia

Skrót klawiszowy NVDA + F7 wyświetla na stronie internetowej wykaz elementów. Są tam łącza, przyciski, nagłówki. Dzięki temu możesz przyjrzeć się strukturze swojej strony.

W menu NVDA w Narzędziach znajdziesz takie, które nazywa się

“Podgląd mowy”. Po uruchomieniu możesz oglądać w oddzielnym okienku to, co wypowiada syntezator mowy.

A skoro mowa o syntezatorze mowy, to ustawienia wywołać możesz skrótem NVDA + Ctrl + v i skonfigurować do swoich potrzeb. Wybierz przycisk “Zmień”, aby wybrać silnik syntezy mowy. Domyślnie są tam SAPI, Espeak i mobilne głosy od Microsoft. Wybierz taki, który najbardziej Ci odpowiada.

## Do zapamiętania

Na koniec rzeczy, które koniecznie musisz zapamiętać:

1. Z NVDA należy pracować klawiaturą, by zrozumieć jego działanie i skutecznie testować.
2. Używanie NVDA wymaga przełączania się między trybem formularza i trybem czytania.
3. Niewidomy użytkownik ma sekwencyjny dostęp do informacji, a skróty klawiszowe tylko trochę to ułatwiają.
4. Struktura strony jest bardzo istotnym elementem dostępności cyfrowej.
