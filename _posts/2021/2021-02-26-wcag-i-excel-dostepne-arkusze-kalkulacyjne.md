---
id: 2101
title: 'WCAG i Excel &#8211; dostępne arkusze kalkulacyjne'
date: '2021-02-26T14:45:43+01:00'
excerpt: 'Na specjalne zamówienie - przymiarka do wytycznych dla dostępnego arkusza kalkulacyjnego'
layout: post
guid: 'http://informaton.blog/?p=2101'
permalink: /2021/02/26/wcag-i-excel-dostepne-arkusze-kalkulacyjne/
timeline_notification:
    - '1614347144'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - Calc
    - etykiety
    - EXcel
    - formularz
    - kontrast
    - numbers
    - tabele
    - WCAG
---

Dostępny czwartek ponownie postawił przede mną wyzwanie. Padło kilka trudnych pytań na temat zapewnienia dostępności arkuszy kalkulacyjnych. W tytule jest Excel, ale dotyczy to w równym stopniu każdego innego arkusza kalkulacyjnego. Przyłóżmy zatem do arkuszy naszą ulubioną miarę, czyli WCAG.

Nadaję temu tekstowi numer wersji 0.1.

## Założenia wstępne

Na początek ustalmy, do czego powinno się używać arkusza kalkulacyjnego. Jest to narzędzie do prezentacji i przetwarzania danych, w szczególności liczbowych. Nie jest to edytor tekstu lub ramka do prezentacji. Jeżeli ktoś używa arkusza niezgodnie z przeznaczeniem, to niech sam się martwi o jego dostępność.

Poniżej moje prywatne rekomendacje przygotowane na podstawie 13 wytycznych zawartych w WCAG. Jeżeli coś pominąłem to jedynie moja wina i zachęcam do słusznej i konstruktywnej krytyki w komentarzach. Świadomie pomijam też rozwiązania istniejące tylko w części arkuszy, na przykład kontrolki ActiveX, ponieważ nie każdy ma do dyspozycji Excel i może korzystać z Libre Calc lub Apple Numbers.

## Wytyczna 1.1 Alternatywa tekstowa

- Umieszczanie grafiki w arkuszu kalkulacyjnym jest złym rozwiązaniem. Jedyny wyjątek można zrobić dla wykresów, dla których dane znajdują się jawnie w tym samym arkuszu. One stanowią alternatywę tekstową dla wykresu.

## Wytyczna 1.2 Multimedia

- Jeżeli – z niezrozumiałego powodu – ktoś umieści w arkuszu kalkulacyjnym filmy, animacje lub podcast, to niech sam się martwi. Tam na takie elementy nie ma miejsca.

## Wytyczna 1.3 Możliwość adaptacji

Tutaj wreszcie mamy o czym pisać. Na początek – arkusz kalkulacyjny to taka naprawdę wielka tabela. Ma setki kolumn i tysiące wierszy. Nic zatem dziwnego, że użytkownik widzi tylko jej wycinek. Dodatkowo – jest to struktura dwuwymiarowa i można przemieszczać się po niej w pionie i poziomie. Nawigacja po arkuszu jest znacznie trudniejsza, niż po dokumencie tekstowym i trzeba to wziąć pod uwagę. Dla niewidomych i słabowidzących użytkowników jest to jeszcze trudniejsze, bo nie widzą otoczenia danej komórki. Osoby niewidome dlatego, że mają dostęp tylko do treści jednej komórki, a słabowidzący – bo widzą ich zaledwie kilka. Zadaniem twórcy arkusza jest zatem ułatwienie w zorientowaniu się w arkuszu. Proponuję zatem następujące zalecenia:

- Zaczynaj tabelę od lewego górnego rogu, czyli od komórki A1. Użytkownik nie będzie musiał szukać początku treści.
- Unikaj zbędnego łączenia komórek w wierszu i kolumnie. Poruszając się klawiaturą użytkownik będzie się przenosił z pojedynczej komórki rozciągniętej na kilka w wierszu, a dalej będzie miał zupełnie inne dane. Unikanie nie oznacza całkowitego zakazu, a stosowanie z namysłem i tylko w niezbędnych sytuacjach.
- Stosuj wiersze i kolumny nagłówkowe i to możliwie blisko początku, czyli góry i lewego krańca.
- Unikaj umieszczania kilku tabel w jednym arkuszu. Lepiej dodaj kolejny w tym samym skoroszycie.
- Unikaj instrukcji skierowanych do odbiorcy opartych o kolor, wielkość lub orientację, czyli na przykład „w prawym górnym rogu”, „w kolumnie zaznaczonej na czerwono”, „zapisane mniejszą czcionką”. Za to zawsze jasne będzie poinformowanie podanie koordynat komórki.

## Wytyczna 1.4 Rozróżnialność

Tutaj zastosowanie ma kilka elementów WCAG, czyli kryteriów sukcesu. Wydaje się, że tylko następujące:

- Informacja nie może być wyróżniona tylko kolorem, bo może nie dotrzeć do wielu ludzi. Stosuj też pogrubienie lub inne wyróżnienia.
- Pamiętaj o odpowiednim kontraście między tłem i tekstem. Niektóre wzory tabel mają różnobarwne tła, co może generować problemy z kontrastem.
- Nie wkładaj pod tekst obrazków, choćby nawet ładnie wyglądały. Każdemu będzie trudniej odczytać tekst.
- Jeżeli masz w arkuszu wykresy, wybierz taki wzór, w którym zachowany jest odpowiedni kontrast.

## Wytyczna 2.1 Dostępność z klawiatury

Zasadniczo twórca nie ma wpływu na tą wytyczną. Wyjątkiem są wbudowane kontrolki, na przykład rozwijane listy. To zawsze jest ryzykowny element, więc upewnij się, że można z listy wybrać wartość. Oczywiście bez użycia myszy.

## Wytyczna 2.2 Wystarczający czas

Tu problemy mogą się pojawić tylko wówczas, gdy arkusz pobiera dane z zewnątrz i te dane się zmieniają. Trudno jest wyłączyć ten efekt. Na szczęście jest dość rzadko używany.

## Wytyczna 2.3 Ataki padaczki

- Nie stosuj tekstu migającego, szczególnie w kolorze czerwonym.

## Wytyczna 2.4 Możliwość nawigacji

- Nadawaj arkuszom zrozumiałe tytuły.
- Pamiętaj o nagłówkach kolumn i wierszy.

## Wytyczna 2.5 Metody obsługi

Nie dostrzegam zastosowania. O wszystko dba klient (edytor) arkuszy kalkulacyjnych.

## Wytyczna 3.1 Możliwość odczytania

- Etykiety, w tym nagłówki kolumn i wierszy, powinny być zrozumiałe. Jeżeli są tam pojęcia mało znane lub używane są skróty, trzeba je wyjaśnić.

## Wytyczna 3.2 Przewidywalność

- Jeżeli w arkuszy dokonywane są operacje zmieniające wartości w komórkach – uprzedź o tym użytkownika. Na przykład w pierwszym wierszu arkusza.
- Jeżeli skoroszyt zawiera arkusze z podobnymi arkuszami, na przykład prezentującymi analogiczne dane z różnych lat, powinny zawsze mieć taki sam układ.

## Wytyczna 3.3 Pomoc przy wprowadzaniu informacji

Często arkusz służy do wprowadzania danych, czyli jest swego rodzaju formularzem. Dobre przygotowanie takiego arkusza nie jest proste, bo nie jest zaprojektowany do takich zadań. Trzeba jednak zadbać także o taką pomoc przy wypełnianiu.

- Jeżeli arkusz wykrywa i wskazuje błędy, to powinien to robić w zauważalny sposób, na przykład za pomocą komunikatu tekstowego wyświetlanego na ekranie.
- Jeżeli w jakieś pole dane ma wpisać użytkownik, musisz dostarczyć mu etykietę. Nie wystarczy napis w komórce obok, bo nie zawsze jest oczywiste, w które pole wpisać dane: powyżej, poniżej, a może po prawej. Dlatego zdecyduj się na coś i stosuj to konsekwentnie, a na początku arkusza poinformuj o tym wyborze użytkownika. Na przykład „Dane wpisuj zawsze w komórce na prawo od etykiety”.
- Podpowiadaj użytkownikowi, w jaki sposób wpisać dane, jeżeli format jest określony. Na przykład „wpisz numer NIP w postaci 10 cyfr, bez innych znaków lub odstępów”.

## Wytyczna 4.1 Kompatybilność

Tu wszystko załatwia edytor arkuszy, który powinien generować poprawny format wyjściowy.

Na razie zostawiam materiał w tej formie, ale będę go uzupełniał. Stosowanie tych podpowiedzi pozwoli na zapewnienie dostępności standardowym arkuszom kalkulacyjnym.

## Inne źródła

- <https://support.microsoft.com/en-us/office/make-your-excel-documents-accessible-to-people-with-disabilities-6cc05fc5-1314-48b5-8eb3-683e49b3e593>

<http://dostepny.joomla.pl/warsztat/dobre-praktyki/dostepne-dokumenty-cyfrowe/206-tworzenie-dostepnych-arkuszy-kalkulacyjnych-w-microsoft-excel-2016-windows-i-2011-mac>