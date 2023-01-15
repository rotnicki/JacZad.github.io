---
id: 1041
title: 'Dostępność niejedno ma imie'
date: '2014-05-09T12:59:10+02:00'
layout: post
guid: 'http://informaton.pl/?p=1041'
permalink: /2014/05/09/dostepnosc-niejedno-ma-imie/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - audyt
    - klawiatura
    - multimedia
    - 'WCAG 2.0'
---

Do napisania tych kilku refleksji zmobilizowała mnie dyskusja na liście osób niewidomych. Zaczęła się od alarmistycznego wezwania do interwencji w sprawie nowej wersji elektronicznego rozkładu jazdy pociągów PKP. Po kilkudziesięciu postach dyskusja – jak często się zdarza – skręciła w stronę prywatnych wycieczek. Jednak wcześniej pojawiło się kilka wątków związanych z dostępnością, które zamierzam opisać i dodać do nich własny komentarz.

### Dostępne czy niedostępne?

Największa dyskusja wybuchła wokół samego stwierdzenia, czy rozkład jest dostępny, czy też nie. Jak się okazało – samo pojęcie dostępności jest znane, ale rozumiane już na najróżniejsze sposoby. Jeden z dyskutantów uznał, że skoro jest w stanie coś zrobić, to znaczy że mechanizm jest dostępny. Argumenty przeciwne były bardzo liczne. Jedne dotyczyły efektywności, bo przecież niewidomy użytkownik musi zrobić o wiele więcej czynności, niż widzący. Inne dotyczyły technologii, bo mechanizm działał różnie w różnych przeglądarkach i z różnymi czytnikami ekranu. Wreszcie argumenty kompetencyjne, bo przecież trzeba umieć posługiwać się technologiami asystującymi.

Dla mnie zupełnie oczywiste jest, że dostępności nie można potwierdzić tylko na tej podstawie, że **ja coś mogę zrobić**. Jest to dostępność co najwyżej subiektywna i niepewna. Jest to też dostępność dla osoby z konkretnym rodzajem niepełnosprawności, konkretną technologią i konkretnymi kompetencjami, a nie obiektywna.

### Dostępność obiektywna nie istnieje

Tak naprawdę jednak nie ma czegoś takiego, jak dostępność obiektywna, w pełni weryfikowalna i pewna. To znaczy – można zrobić stronę internetową zgodną z wymaganiami, ale jest to pewnego rodzaju abstrakt, który w rzeczywistości nie istnieje. Kiedy rozmawiamy o istniejącym serwisie, w którym zasady dostępności nie były fundamentem założycielskim, zawsze będziemy mieli wątpliwości. A przynajmniej ja będę miał wątpliwości.

Załóżmy, że przyglądamy się nowemu kalendarzowi służącemu do wybierania daty wyjazdu. Dzień wybierany jest za pomocą kliknięcia myszą, ale nie są to linki ani żadne inne elementy dostępne z poziomu klawiatury. Jednak czytniki ekranu wykrywają akcje onClick i dają możliwość wybrania za pomocą klawiatury. Ta funkcjonalność nie wynika jednak z budowy serwisu, ale ze specjalnego oprogramowania, z którego korzysta niewidomy użytkownik. Czy zatem wytyczna 2.1 WCAG jest spełniona, czy też nie? Oczywiście nie jest, chociaż akurat ten użytkownik może spacją wybrać dany dzień.

Teraz zaczyna się to jeszcze trudniejsze – decyzja o tym, co zrobić, by ten kalendarz był dostępny. Można dodać rolę BUTTON i odpowiedni TABINDEX do każdego obiektu z dniem i zatrzeć ręce, że jest w porządku. No i wtedy ja mam zgryz decyzyjny, bo rzeczywiście – z punktu widzenia WCAG jest już w porządku. Tylko nie każdy ma przeglądarkę i czytnik ekranu obsługujące technologię ARIA, a zatem dla niego nic się nie zmieni. Moja sugestia do zmiany będzie w tej sytuacji następująca – zamiana na znacznik BUTTON, a nie dodawanie innym obiektom roli BUTTON, tylko jaką mam stosować przy tym argumentację?

### Niewidomy nie jest dobrym audytorem dostępności

Jeżeli ktoś kiedyś zaproponuje sprawdzenie dostępności strony internetowej przez osobę niewidomą – nie korzystajcie. Osoba niewidoma nie jest dobrym audytorem dostępności i nigdy nie będzie. Powodem fundamentalnym jest to, że nie wie, co znajduje się na stronie internetowej i jak ona działa. Paradoksalnym jest, że może stwierdzić niedostępność czegoś, co dostępne jest przynajmniej w stopniu minimalnym. Za to elementy zupełnie niedostępne zwyczajnie umykają technologiom asystującym. Jakiś czas temu miałem taki problem w sklepie [Home.pl](http://home.pl), gdy chciałem kupić kolejną domenę. Elementy odpowiedzialne za realizację procesu zakupu były albo zupełnie niedostępne, albo nie były elementami aktywnymi. Nie poradziłem sobie z tym zakupem sam i musiałem poprosić kogoś widzącego. Tyle że ja **wiedziałem**, że tam muszą być takie elementy, więc ich intensywnie szukałem. A gdybym nie szukał, to zwyczajnie bym je przeoczył.

Osoba niewidoma jest złym audytorem także z innego powodu – bo z zewnątrz może wyglądać na kompetentną w tym zakresie. Na dostępności stron internetowych najbardziej korzystają właśnie niewidomi użytkownicy, więc często stawia się znak równości pomiędzy dostępnością i dostępnością dla osób niewidomych. To oczywiście jest bzdura, ale bzdura dosyć powszechnie akceptowana. Jest ona rozpowszechniona także wśród osób niewidomych, bo w końcu oni też są częścią społeczeństwa. Wystarczy jednak zadać jedno proste pytanie – jak sprawdzisz obecność napisów w filmie, kontrast kolorów, migotanie treści? I nagle okazuje się, że taki audyt można sobie wsadzić… między bajki. Wykonywanie testów lub audytów wymaga znajomości tematu, a nie wyczucia. Wszyscy mówimy po polsku, ale nie każdy jest redaktorem, korektorem lub pisarzem.

Jednak jest tu też druga strona – osoba niewidoma może być jednocześnie najlepszym audytorem, gdy pracuje w zespole. Dla webmasterów, programistów, projektantów dostępność jest czymś dosyć obcym, z czym nie mają do czynienia na codzień. Jest to dla nich język obcy, więc warto podeprzeć się wsparciem <span lang="en">“native speakerów”</span>, czyli właśnie osób niewidomych. Dla nich oczywistościami są struktura i semantyka informacji, bo korzystają z niej na codzień. Bez problemu wskażą miejsca, gdzie informacja opiera się tylko na wzroku, a zatem nie jest uniwersalna. dopadną i rozszarpią braki w opisach alternatywnych lub multimediach. A kiedy poznają zasady dostępności, mogą spokojnie kierować zespołami audytorskimi. Przedtem muszą jednak wiele się nauczyć, by wiedzieć, gdzie tkwią ich słabości i niemożności.

### Dostępność efektywna

Warto jeszcze zwrócić uwagę na wątek efektywności w dostępności. Serwis internetowy może być bowiem zgodny z wymaganiami WCAG 2.0 (przynajmniej formalnie) i audytor nie może się za bardzo przyczepić. A jednocześnie może być tak nieefektywny w używaniu, że ta dostępność nie ma żadnego znaczenia. Z drugiej strony – tu padnie herezja – serwis może być na bakier z wieloma zasadami dostępności, a jednocześnie być “używalny”, a praca z nim może być wygodna i szybka. Chyba wiem skąd to się bierze, a przyszło mi do głowy po przeczytaniu książki [UX Storytellers](http://www.hci.org.pl/uxs/), czyli wyznań specjalistów z dziedziny UX. Miałem poczucie, że to jest kolejna grupa specjalistów dziedziny tak wąskiej, że nie zahacza nawet o inne dziedziny. UX, czyli <span lang="en">user experience to coś innego niż użyteczność lub dostępność. A to przecież wcale nie jest tak. UX to coś wynikającego z użyteczności i dostępności, a do tego branych razem. Jest to jeden konglomerat pojęciowy, który trzeba brać łącznie, a nie rozdzielnie. W całej książce znalazłem zaledwie jedno odniesienie do dostępności, dotyczące upraszczania formularzy, by były bardziej zrozumiałe. To jest właśnie dostępność, chociaż autor pewnie w ogóle tak nie pomyślał.</span>

Już dawno zauważyłem, że użyteczność i dostępność mają wiele punktów wspólnych. Tak naprawdę, to jest to to samo, tylko w innym ujęciu. Może ktoś młodszy i z bardziej otwartym umysłem zrobiłby kompilację tych dwóch obszarów i to pokazał. Potem UX będzie wychodzić już samo.

Pozostawiam te rozważania do przemyślenia, także osobom niewidomym uważającym się za ekspertów od dostępności stron internetowych. Mogą zrobić prosty test: przejrzeć specyfikację [WCAG 2.0](http://fdc.org.pl/wcag2/) i zaznaczyć sobie kryteria  
 sukcesu, które mogą sami sprawdzić. To może być dobra lekcja pokory. Jest to też powód, dla którego tak niechętnie podejmuję się robienia audytów dostępności – zawsze muszę znaleźć kogoś, kto mi w tym pomoże, a jednocześnie muszę go wdrożyć w dostępność. Jeżeli zaś kiedyś zajmę się tym na poważnie, znajdę kogoś na stałe do zespołu. I na pewno nie będzie to osoba niewidoma.