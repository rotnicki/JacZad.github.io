---
title: 'Dostępny bank internetowy &#8211; na co zwrócić szczególną uwagę?'
date: '2014-08-28T14:54:32+02:00'
layout: post
categories:
    - artykuły
tags:
    - 'Android'
    - banki
    - formularze
    - iOS
    - klawiatura
    - 'aplikacje mobilne'
    - pieniądze
---

Ostatnio czytałem i komentowałem dokument przygotowany przez Związek Banków Polskich traktujący o dobrych praktykach w obsłudze niepełnosprawnych klientów. Jest to druga wersja wytycznych, która została gruntownie poprawiona i poważnie rozszerzona o temat dostępności w Internecie i bankowości mobilnej. Oczywiście dostępność banku elektronicznego jest tą samą dostępnością, co sklepu, portalu, czy edytora online. Jednak jest tu też pewna specyfika, na którą warto zwrócić szczególną uwagę, bo wiąże się z bezpieczeństwem pieniędzy.

### Logowanie do systemu transakcyjnego

Wykonywanie operacji bankowej zaczynamy od zalogowania się. Zazwyczaj klient dysponuje loginem, na przykład numerem klienta i hasłem. Oba pola tekstowe powinny być wykonane za pomocą standardowych kontrolek lub ostatecznie – muszą być odpowiednio oprogramowane, by takie kontrolki udawać. Nie wystarczy, że wyglądają na pola edycyjne, ale muszą być polami tego typu w sensie semantycznym. Oczywiście przy każdym należy umieścić dowiązaną etykietkę oraz przynajmniej podstawową instrukcję wprowadzania danych. Kilkukrotne błędne wprowadzenie danych może skutkować zablokowaniem konta.

Problem pojawia się, gdy projektanci postanowią zadbać dodatkowo o bezpieczeństwo. Znajdują wówczas jakiś sposób na utrudnienie wprowadzania hasła, na przykład oczekując wprowadzenia tylko znaków o konkretnych numerach. Takie rozwiązanie może być dostępne w sensie technicznym, bo przecież to tylko kolejny formularz, ale warto pamiętać, że osoba niewidoma musi odliczać znaki w pamięci lub ostatecznie wydrukowane w brajlu. Drukowania hasła się zdecydowanie nie zaleca, więc pozostaje zawodna pamięć. Do tego zdarza się, że numer pozycji znaku w haśle wyświetlany jest w postaci obrazka bez tekstu alternatywnego. Wtedy to już zupełnie jest źle.

Nie potrafię ocenić, czy opisywane powyżej rozwiązanie zwiększa znacząco bezpieczeństwo. Zakładam tu utrudnienie dla keyloggerów (złośliwego oprogramowania przechwytującego naciśnięcia klawiszy). Jednak trzeba mieć na uwadze, że nie każdy poradzi sobie z tego rodzaju zabezpieczeniem.

Pola edycyjne i przycisk do zalogowania powinny być dostępne z poziomu klawiatury i zawsze powinien być widoczny fokus na elemencie interfejsu.

### Wykonywanie operacji

Po zalogowaniu mamy dostęp do panelu administracyjnego, który pozwala na wykonywanie różnorodnych operacji, na przykład sprawdzanie salda, przygotowywanie przelewów itp. Najważniejszymi elementami są zatem nawigacja i formularze. Można przedstawić następującą listę szczegółowych zaleceń:

1. Każdy element interfejsu (linki, kontrolki formularzy, przyciski) musi być dostępny z poziomu klawiatury, a przemieszczanie się po nich musi być logiczne (prawidłowa kolejność). Fokus przemieszczany za pomocą klawiatury musi być zawsze dobrze widoczny. Jeżeli w systemie są elementy dynamiczne rozwijane za pomocą myszki, to muszą działać tak samo przy użyciu klawiatury.
2. Należy unikać elementów interfejsu, które zmieniają się bez wiedzy użytkownika. Tzw. “inteligentne” interfejsy próbują domyślić się, co zamierza zrobić użytkownik i podsuwają mu gotowe rozwiązania. To może być pomocne dla doświadczonych użytkowników, ale mniej doświadczonych i niepełnosprawnych może wprawić w konsternację. Oni oczekują stałego interfejsu, stałej kolejności pozycji w menu i wyraźnej reakcji systemu na działania użytkownika. Jeżeli system będzie robił coś za nich – poczują się zagubieni.
3. Informacje w panelu powinny być prawidłowo opisane semantycznie. Szczególnie dotyczy to informacji o charakterze tabelarycznym, na przykład listy operacji.
4. Staranne wykonanie formularzy jest kluczowe dla dostępności panelu transakcyjnego. Każdy element powinien być zaopatrzony w etykietę oraz stosowną instrukcję wypełniania. Jeżeli w polu wymagany jest konkretny format danych lub niedopuszczalne są pewne znaki, to trzeba to wyraźnie napisać użytkownikowi. Interfejs musi też dawać możliwość kopiowania informacji, na przykład z dokumentu tekstowego lub emaila oraz edytowania zawartości. Takie możliwości dają przede wszystkim natywne kontrolki HTML, więc warto je stosować.
5. Błędy wykryte podczas sprawdzania przez system muszą być prezentowane w postaci tekstu. Oznaczanie błędnych danych kolorem jest dopuszczalne, ale nie może to być jedyny sposób. Błąd należy też jakoś wyjaśnić użytkownikowi. “Błędny numer konta” to trochę zbyt lakoniczne wyjaśnienie, ale już “W numerze konta jest za mało cyfr – brakuje jednej” lub “Popraw numer konta. Suma kontrolna pokazuje, że jest nieprawidłowy.” dają już odpowiednią informację. Analogicznie warto podawać informacje o błędach w formacie danych lub o nie wystarczających środkach na koncie. Komunikaty o błędach warto osadzać w [aktywnych regionach,](http://informaton.pl/?p=499)aby nie uszły uwagi niewidomym klientom.
6. Następnym krokiem jest danie możliwości sprawdzenia poprawności danych. Jest to standardowe rozwiązanie spotykane w bankach i sklepach internetowych, polegające na wyświetleniu podsumowania operacji. Użytkownik może na spokojnie przejrzeć wprowadzone dane i zatwierdzić operację. Jeżeli odkryje błąd – powinien mieć możliwość poprawienia w tym jednym miejscu, a nie należy go zmuszać do wypełniania całego formularza od początku.
7. Prawdziwą zmorą mogą być wygasające sesje, które mają chronić użytkownika przed pozostawieniem w publicznym miejscu komputera z uruchomionym i działającym systemem transakcyjnym. To jest potrzebne zabezpieczenie, ale koniecznie należy zadbać, by użytkownik został ostrzeżony onadchodzącym momencie wygaśnięcia sesji, by mógł jakoś zareagować. A jak mu ta sesja nawet wygaśnie i system go wyloguje, powinien dać możliwość ponownego zalogowania i dokończenia pracy w miejscu, gdzie została przerwana bez utraty danych.

### Potwierdzanie operacji

Potwierdzanie operacji jednorazowymi kodami jest standardową procedurą w niemal każdym banku Internetowym. Banki mają wiele sposobów na zaopatrywanie klientów w takie kody, a najważniejsze wymieniam poniżej.

1. Kody drukowane na papierowych zdrapkach. To jeden z najstarszych sposobów, polegający na wysłaniu do klienta kartki z wydrukowanymi kodami jednorazowymi o przypisanych im numerach. System transakcyjny podaje numer kodu, a użytkownik odnajduje kod i przepisuje go w formularzu. Rozwiązanie niedostępne dla osób niewidomych i częściowo niedostępne dla słabowidzących.
2. Kody drukowane brajlem. Nie wiem, czy jeszcze są stosowane, ale kilka lat temu banki oferowały takie listy kodów dla niewidomych klientów. Były dostępne dla osób niewidomych, ale pod warunkiem, że znały brajla. A to wcale nie jest tak powszechna umiejętność.
3. Kody przesyłane przez SMS. Ten rodzaj kodów zastąpił kody papierowe i jest najbardziej optymalnym rozwiązaniem. Dzięki oprogramowaniu czytającemu ekran i powiększającemu ekran telefonu lub smartfona – jest to rozwiązanie dostępne dla osób niepełnosprawnych wzrokowo. Wymaga jednak posiadania telefonu z odpowiednim oprogramowaniem.
4. Elektroniczne tokeny generujące kody. Nie wiem, czy są jeszcze w użyciu, ale kiedyś z kontem bankowym dostarczano klientowi urządzenie elektroniczne. Jego jedynym zadaniem było generowanie jednorazowego ciągu cyfr, którym można było potwierdzić transakcję. Były oczywiście zupełnie niedostępne dla osób niewidomych i częściowo dla słabowidzących.

Jak widać – jedynym w miarę pewnym mechanizmem autoryzacji są kody przesyłane przez SMS. Przynajmniej w wypadku bankowości internetowej, a nie aplikacji mobilnych.

### Aplikacje mobilne

Coraz więcej banków oferuje aplikacje mobilne na smartfony, głównie iPhone, Android i Windows Phone. Dzięki temu klient może mieć wygodny dostęp do swojego konta w  
każdym miejscu, pod warunkiem dostępu do Internetu. Korzystanie ze smartfona ma dodatkową zaletę, jaką jest możliwość powiązania konta z konkretnym urządzeniem, co ogranicza konieczność zabezpieczania operacji jednorazowymi kodami. Dodatkowe funkcjonalności mogą wykorzystywać odbiornik GPS, na przykład wskazując najbliższe placówki bankowe lub bankomaty.

Aplikacje mobilne należy także projektować z troską o dostępność. Zarówno system iOS, jak i Android oddają w ręce deweloperów obszerne dokumentacje poświęcone budowaniu dostępnych interfejsów. Warto w tym miejscu przypomnieć także o istnieniu rewelacyjnego dokumentu przygotowanego przez BBC pod tytułem [Mobile Accessibility Guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile_access.shtml). Polecam to opracowanie, bo nader często zdarza się, że aplikacja pozbawiona jest tak podstawowych funkcjonalności, jak możliwość zalogowania się. Za wzór można stawiać starą wersję aplikacji mobilnej mBanku, BZ WBK oraz Millenium. Proszę się jednak do tych rekomendacji nie przywiązywać, bo z każdą aktualizacją sytuacja może się zmienić.
