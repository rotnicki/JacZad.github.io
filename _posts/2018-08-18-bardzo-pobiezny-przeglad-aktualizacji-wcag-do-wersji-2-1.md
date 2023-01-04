---
id: 1864
title: 'Bardzo pobieżny przegląd aktualizacji WCAG do wersji 2.1'
date: '2018-08-18T14:48:17+02:00'
layout: post
guid: 'http://informaton.pl/?p=1864'
permalink: /2018/08/18/bardzo-pobiezny-przeglad-aktualizacji-wcag-do-wersji-2-1/
restapi_import_id:
    - 5ca8405547793
publicize_twitter_user:
    - jaczad
categories:
    - artykuły
tags:
    - ARIA
    - kontrast
    - mobilne
    - standard
    - 'technologie asystujące'
    - 'WCAG 2.0'
    - 'WCAG 2.1'
---

Aktualizacja standardu WCAG 2.0 do wersji 2.1 przyniosła 17 nowych kryteriów sukcesu i zupełnie nową wytyczną. Zmiany podyktowane były koniecznością uwzględnienia trzech obszarów, do tej pory mało obecnych:

1. Aplikacje i strony mobilne.
2. Osoby słabowidzące.
3. Osoby z ograniczeniami poznawczymi.

Poniżej streszczam te 17 nowych kryteriów sukcesu, jak je rozumiem i jak sam umiem wyjaśnić. Tłumaczenia są bardzo kulawe, bo na szybko trudno znaleźć zgrabne polskie odpowiedniki, a i sam dokument pisany jest bez refleksji nad problemami z tłumaczeniami. Jeżeli zatem ktoś wpadnie na lepsze tłumaczenie, to ja z otwartymi ramionami przyjmę. Podkreślam też, że to nie jest tłumaczenie, a raczej przegląd i wyjaśnienie nowelizacji. Treść dodanych elementów można znaleźć w [tym dokumencie](https://www.w3.org/WAI/standards-guidelines/wcag/new-in-21/).

1. Kryterium sukcesu 1.3.4 – orientacja: pozwól na wyświetlanie treści zarówno w układzie poziomym, jak i pionowym (poziom AA). To ewidentnie kryterium związane z urządzeniami mobilnymi, które dostosowują sposób wyświetlania informacji w zależności od tego, jak urządzenie trzyma użytkownik. Czasem jednak nie może go obrócić i pojawia się problem, gdy aplikacja wymusza układ pionowy, a urządzenie jest ułożone poziomo.
2. Kryterium sukcesu 1.3.5: określ prawidłową wartość (poziom AA). Lepiej tego na razie nie umiem przetłumaczyć. Chodzi tu zaś o to, by system – o ile to możliwe – podpowiadał użytkownikowi prawidłowe wartości już podczas wprowadzania danych, na przykład przez autouzupełnianie. Wygodne dla wszystkich, ale szczególnie docenią to osoby z dysleksjami.
3. Kryterium sukcesu 1.3.6: określ znaczenie (poziom AAA). W tym kryterium chodzi o to, by do komponentów interfejsu, szczególnie graficznych, dodawać ich znaczenie. Wydaje się to dosyć podobne do dodawania ról, ale jednak na bardziej szczegółowym poziomie. Przychodzi mi do głowy przykład z ikonką drukarki, do której dołączona jest semantycznieinformacja, że ta konkretna ikonka oznacza drukowanie, a sąsiednia – wysłanie pocztą email. Nie znam oprogramowania, o którym wspomina WCAG 2.1, ale pozwala ono na podmianę nieznanych ikonek na standardowe, co ułatwi życie osobom z ograniczeniami poznawczymi.
4. Kryterium sukcesu 1.4.10: zawijanie tekstu (poziom AA). W tym kryterium uwzględnia się potrzeby osób bardzo słabo widzących, które wymagają dużych powiększeń. Tekst powinno dać się powiększyć tak, by nie wymagało to przewijania w poziomie lub pionie. Jest to zatem funkcja “reflow” z różnych czytników dokumentów tekstowych, na przykład Adobe Acrobat.
5. Kryterium sukcesu 1.4.11: kontrast dla treści nie będących tekstem (poziom AA). Jest to spora zmiana w stosunku do WCAG 2.0, które wymagały kontrastu tylko dla tekstu. Teraz wymagany jest kontrast także dla elementów interfejsu i grafik pozwalających na zrozumienie treści. Na przykład wcześniej w formularzu badany był tylko kontrast dla etykietki tekstowej dla pola wyboru, a teraz badać się będzie także samo pole wyboru.
6. Kryterium sukcesu 1.4.12: światło w tekście (poziom AA). Tu ponownie ukłon w stronę osób mających problemy z czytaniem (dysleksja, słaby wzrok) i możliwość ustawienia optymalnych dla siebie odstępów pomiędzy liniami, akapitami, znakami i wyrazami. Oczywiście te zmiany nie mogą spowodować utraty treści!
7. Kryterium sukcesu 1.4.13: treści spod fokusa (poziom AA). Tutaj kryterium rozprawia się z treściami wyświetlanymi automatycznie po najechaniu kursorem na jakiś element. Z jednej strony – użytkownikom programów powiększających może to przesłaniać widok, a z drugiej – dla użytkowników z zaburzoną motoryką może być trudno zapanować nad kursorem.
8. Kryterium 2.1.4: jednoliterowe skróty klawiszowe (poziom A). Jeżeli w aplikacjach stosowane są skróty jednoznakowe, czyli bez klawiszy modyfikujących, to trzeba dać możliwość ich wyłączenia lub mogą działać tylko na element, na którym znajduje się fokus. W aplikacji webowej Gmail klawisz “c” tworzy nową wiadomość i jest to bardzo wygodne. Jednak czasem fokus może gdzieś uciec i podczas pisania użyjemy klawisza do archiwizacji lub wręcz kasowania i robi się problem. Akurat w Gmail można te skróty wyłączyć.
9. Kryterium 2.2.6: koniec czasu (poziom AAA). Użytkownik powinien być ostrzeżony, że może utracić dane po określonym czasie braku aktywności.
10. Kryterium sukcesu 2.3.3: animacje podczas działań (poziom AAA). Efektowne animacje, zwłaszcza w aplikacjach mobilnych, mogą być dezorientujące dla niektórych użytkowników. Trzeba zatem dać im możliwość ich wyłączenia. Wydaje się też, że będzie to z pożytkiem dla wydajności tych aplikacji.
11. Kryterium sukcesu 2.5.1: gesty punktowe (poziom A). Jeżeli w aplikacji wykorzystywane są gesty wielopalcowe lub wymagające przesuwania w określony sposób, to istnieje też możliwość by daną funkcję zrealizować za pomocą pojedynczego dotknięcia. W materiale źródłowym podano dobry przykład, gdy mapę powiększa się rozszerzając palcami, ale można też kliknąć na przyciski zwiększania i zmniejszania.
12. Kryterium sukcesu 2.5.2: anulowanie kliknięcia (poziom A). To kryterium dotyczy możliwości wycofania się z przypadkowego kliknięcia myszą lub dotknięcia palcem. Oczywiście nie chodzi o to, by każde kliknięcie potwierdzać w otwartym oknie. Chodzi o to, by można było palec przesunąć poza przycisk, by funkcja się nie aktywowała. Doskonale zrobione jest w klawiaturze wirtualnej na iOS.
13. Kryterium sukcesu 2.5.3: etykieta w nazwie (poziom A). Należy zachować zgodność nazwy komponentu z jego etykietą. Na przykład przycisk do wyszukiwania powinien mieć nazwę “szukaj” jeżeli taki napis jest na nim wyświetlony. Ciekawe, jak to będzie działać z polskimi literkami oraz elementami tłumaczonymi w locie. Mogą pojawić się problemy, a poziom dostępności to pojedyncze A.
14. Kryterium sukcesu 2.5.4: aktywowanie ruchem (poziom A). To kryterium dotyczy urządzeń mobilnych wyposażonych w akcelerometry, kompasy i inne sensory. Ich użycie jest bardzo wygodne, ale powinno dać się możliwość używania aplikacji bez nich, to znaczy za pomocą standardowego interfejsu.
15. Kryterium sukcesu 2.5.5: wielkość kontrolki (poziom AAA). Wielkość obiektu, który trzeba dotknąć lub kliknąć myszą musi być na tyle duża, by użytkownik mógł łatwo trafić palcem lub kursorem myszy. Tutaj wielkość określono na przynajmniej 44 punktów CSS.
16. Kryterium sukcesu 2.5.6: konkurencyjne metody wprowadzania danych (poziom AAA). Użytkownik powinien mieć możliwość wybrania, z jakiej metody wprowadzania danych skorzysta. Podłączenie myszy nie może wyłączać dostępu za pomocą klawiatury, a podłączenie klawiatury fizycznej nie powinno blokować możliwości używania klawiatury wirtualnej. Całkiem dobry pomysł, chociaż mam wrażenie, że raczej jest to robione domyślnie.
17. Kryterium sukcesu 4.1.3: komunikaty o stanie (poziom AA). Tutaj chodzi o to, by komunikaty systemowe przekazywane były za pośrednictwem technologii asystujących. W poczcie Gmail po wysłaniu wiadomości, czytnik ekranu informuje “wiadomość wysłana” bez przenoszenia fokusu do miejsca, gdzie pojawił się ten komunikat. Tu aż się prosi o aria-live z parametrem “polite” lub “assertive”. Jestem za, chociaż spotkałem też rozwiązania okropnie upierdliwe, na przykład na YouTube przy wysyłaniu filmu na serwer.

Jak widać – pojawiła się nowa, trzynasta wytyczna z numerem 2.5. Dotyczy ona różnych trybów (sposobów) na wprowadzanie danych. Pojawiają się tu gesty, poruszanie urządzeniem, obsługa za pomocą mowy, rysika itp. Innymi słowy – pojawiły się urządzenia inne, niż komputer.

Teraz czekam aż ktoś porządnie przetłumaczy to wszystko na język polski. A potem włączy w przepisy prawne i proces kształcenia programistów i projektantów. Zauważcie też, że żadne z nowych kryteriów nie jest kierowane do twórców i redaktorów treści. Wszystkie dotyczą osób technicznie zajmujących się interfejsami