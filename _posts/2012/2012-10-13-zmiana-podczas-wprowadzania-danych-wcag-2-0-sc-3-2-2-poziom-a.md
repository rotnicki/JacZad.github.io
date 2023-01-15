---
id: 311
title: 'Zmiana podczas wprowadzania danych (WCAG 2.0 SC 3.2.2, poziom A)'
date: '2012-10-13T08:06:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=311'
permalink: /2012/10/13/zmiana-podczas-wprowadzania-danych-wcag-2-0-sc-3-2-2-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - bezpieczeństwo
    - fokus
    - formularze
    - klawiatura
    - nawigacja
---

Prawdziwą zmorą dla wielu użytkowników są interaktywne, czy wręcz “inteligentne” formularze. Podczas wprowadzania danych w polach edycyjnych, zaznaczania pól wyboru lub opcji, wybierania pozycji z listy lub innych czynności, na stronie dzieją się przeróżne rzeczy. Często dzieją się poza kontrolą i świadomością użytkownika, chociaż w założeniu miały mu pomagać. Warto zatem przemyśleć sposób skonstruowania formularzy i zabrać im nieco tej wątpliwej inteligencji.

Kryterium sukcesu 3.2.2 zobowiązuje projektantów serwisów internetowych, by podczas wprowadzania danych w formularzach użytkownik nie był zaskakiwany zmianą kontekstu, chyba że zostanie o tym uprzedzony przed wprowadzeniem danych. Zmiana kontekstu oznacza między innymi uruchomienie innej aplikacji, otwarcie innej strony, zmianę sposobu prezentacji treści lub sensu dokumentu. Skorzystają na tym:

- użytkownicy niewidomi i słabowidzący,
- użytkownicy klawiatur,
- użytkownicy z ograniczeniami kognitywistycznymi,
- seniorzy.

Projektowanie formularzy, jako elementu nawigacjiw serwisie, wymaga sporej staranności i przemyślenia konsekwencji. Zdarzają się serwisy, gdzie z rozwijanej listy należy wybrać swój kraj, by przejść na stronę lokalnego dystrybutora. Nie ma w tym rozwiązaniu nic złego, o ile to użytkownik zdecyduje, kiedy już dokonał wyboru, a kiedy zaznaczył jakiś kraj przez pomyłkę lub nie miał innego wyboru. Jeżeli bowiem zaraz po zaznaczeniu kraju na liście zostanie przeniesiony, to może być zmuszony do powrotu i wybierania po raz kolejny. Najgorzej w takim wypadku mają użytkownicy klawiatur, którzy **muszą** przejść przez wszystkie kraje po kolei, zanim trafią na ten którego potrzebują. Po każdym przekierowaniu muszą wracać na stronę z listą wyboru i przesunąć kursor o jedną pozycję w dół i znowu zostaną przeniesieni na złą stronę i tak czasem bardzo wiele razy. A najgorzej jest wtedy, gdy po powrocie fokus znajduje się ponownie na pierwszej pozycji, bo to oznacza pętlę bez wyjścia. A wystarczy, by oprócz listy dać użytkownikowi przycisk “wybierz”, by mógł on spokojnie dokonać wyboru.

Podobnie irytujące są rozwiązania, gdy po zaznaczeniu pola wyboru lub opcji wyskakuje nam okno z przeglądarką plików PDF wczytującą w locie jakiś dokument z sieci. Mniej doświadczony użytkownik może być mocno zdezorientowany, o ile nie zostanie o tym uprzedzony. W zasadzie każdą zautomatyzowaną akcję wykonywaną przy zmianie danych w formularzu należy dobrze przemyśleć, by była ona faktycznie przydatna użytkownikowi.

Jednak najbardziej niebezpiecznym zjawiskiem, jakie wiąże się z tzw. “inteligentnymi” formularzami jest zmiana sensu formularza. Użytkownik, który nie ogarnia całości strony, a jedynie niewielki jej fragment, może być wprowadzony w błąd. Załóżmy, że wypełnia formularz zamówienia na usługę telefoniczną i w pewnym momencie zaznacza pole wyboru “klient indywidualny” i cały formularz się zmienia, w tym dobierane są inne parametry abonamentu. Jednak użytkownik o tym nie wie, bo wprowadza swoje dane osobowe, a koszt i warunki abonamentu sprawdził wcześniej i odpowiadały mu. W ten sposób może zawrzeć umowę na warunkach niekorzystnych dla siebie tylko dlatego, że dane zmieniły się podczas ich wprowadzania. Takie działanie formularza jest dopuszczalne, o ile użytkownik zostanie o takiej zmianie poinformowany, na przykład przez komunikat w rodzaju “klient indywidualny – zaznaczenie tego pola może spowodować zmiany w taryfach wybranych wcześniej”.