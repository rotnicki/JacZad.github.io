---
id: 988
title: 'Wykrywanie czytników ekranu &#8211; dobro czy zło?'
date: '2014-03-15T16:42:57+01:00'
layout: post
guid: 'http://informaton.pl/?p=988'
permalink: /2014/03/15/wykrywanie-czytnikw-ekranu-dobro-czy-zlo/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - badania
    - przeglądarki
    - RWD
    - TL-DR
    - WebAIM
---

Niedawno zakończyło się [badanie użytkowników czytników ekranu](http://informaton.pl/?p=966). Zadano w nim dwa pytania na temat wykrywania przez serwisy internetowe sytuacji, gdy użytkownik korzysta z czytnika ekranu. Pierwsze dotyczyło komfortu, a drugie – akceptacji tej sytuacji, gdyby miała pozytywnie wpłynąć na dostępność serwisu. No i rozpętała się krótka, ale burzliwa dyskusja.

Prawie 4/5 respondentów czułaby się mniej lub bardziej komfortowo wiedząc, że po drugiej stronie ktoś wie o tym, że używają czytników ekranu. Aż 7/8 odczuwa to, jeżeli miałoby to pozytywny wpływ na dostępność serwisu. Ja też jestem w tej grupie, chociaż teraz wiem, że popełniłem błąd zaznaczając te opcje. Po prostu nie do końca przemyślałem decyzję, a dokładniej – okazałem się naiwniakiem.

### Usprawiedliwiam się z decyzji

Przez te wszystkie lata zajmowania się dostępnością narzekałem na brak danych statystycznych. Na pytania o liczbę użytkowników niewidomych, słabowidzących, głuchych, niesprawnych manualnie i z innymi niesprawnościami odpowiadałem danymi pośrednimi. Może to kogoś zdziwi, ale nie ma pewnych danych na temat liczby osób niewidomych w Polsce. Ja w takiej sytuacji podaję liczbę 145 tysięcy, która wynika z badania stanu zdrowia ludności Polski, a jednocześnie dosyć dobrze pokrywa się z szacunkami Światowej Organizacji Zdrowia. Informacje zebrane z w sposób automatyczny byłyby dobrym argumentem w dyskusji. Jednak ten medal ma drugą stronę, której nie zauważyłem.

### Dwa powody, by nie zbierać tego typu danych

W dyskusjach na temat zbierania informacji o użytkownikach czytników ekranu powtarzały się dwa argumenty: prywatność i jakość serwisów internetowych. Pierwszy można streścić w stwierdzeniu, że nie powinno się zbierać informacji wrażliwych, a takimi są informacje o używaniu technologii wspomagających. Oznacza to bowiem, że po drugiej stronie Internetu jest w tym wypadku osoba niewidoma. W połączeniu z serwisami, gdzie podajemy dane osobiste (imie, nazwisko, adres email, numer telefonu) jest to faktycznie niebezpieczne.

Drugi argument jest innej natury. Jeżeli wykrywanie czytników ekranu ma doprowadzić do podniesienia dostępności serwisu internetowego, to w jaki sposób? Możliwe są dwie ścieżki. Po pierwsze – właściciel serwisu dowiaduje się o takich użytkownikach i dostępności, a na skutek wewnętrznej przemiany każe poprawić serwis. Po drugie – programista dodaje skrypt, który wykrywa czytnik ekranu i przenosi użytkownika na “specjalną wersję strony dla niepełnosprawnych”. Niestety – doświadczenie podpowiada raczej to drugie rozwiązanie. Jednak najbardziej niebezpieczne jest połączenie obu ścieżek polegające na przekształceniu serwisu do innej wersji za pomocą odpowiedniego skryptu. Oznacza to pojawienie się **kolejnej wersji dostosowanej**. Czy coś Wam to przypomina?

### Psucie standardów

Wyobraźcie sobie teraz skrypt, który wykrywa rodzaj przeglądarki i czytnik ekranu i na tej podstawie generujący atrybuty ARIA i inne elementy wspomagające dostępność. Kolejne potężne i wciąż puchnące biblioteki programistyczne, których jedynym zadaniem jest wyświetlanie **tak samo tych samych elementów** w różnych przeglądarkach. Teraz spuchną od kolejnych wariantów wyświetlania czcionek, obrysów, fokusów, landmarków i całej reszty. Zamiast uniwersalnie zaprojektowanego serwisu będziemy mieli setki wariantów dla różnych kombinacji system operacyjny / przeglądarka / wersja przeglądarki / czytnik ekranu / rozdzielczość. Po co producenci przeglądarek mają się martwić stosowaniem standardów, skoro programista może zrobić kolejną wersję. A jak nie zrobi, to jego problem. Ktoś powie, że to jest przecież sedno projektowania responsywnego, które dopasowuje się do klienta. Ja jednak obawiam się czegoś innego – w pewnym momencie te wszystkie frameworki, biblioteki, skórki będą tak skomplikowane i rozbudowane, że nikt ich nie ogarnie. Wtedy zacznie się zewnętrzne łatanie, jak to ma już miejsce w wypadku [Bootstrap](http://informaton.pl/?p=949). A producenci przeglądarek ten problem też zrzucą na barki programistów.

Może trochę przesadzam i nie będzie tak źle. Jednak oczami wyobraźni widzę już komunikaty wyświetlane na stronie internetowej <q>Przeglądanie strony wymaga przeglądarki Internet Explorer w wersji 22 lub wyższej, czytnika ekranu Jaws for Windows w wersji 19 SP 2 i syntezatora mowy Speecher. Uaktualnij swoje oprogramowanie i wróć do nas.</q>. Brrr… Dlatego biję się w pierś, że zgrzeszyłem zaznaczając niewłaściwą opcję w badaniu i na przyszłość będę bardziej uważał. Szkoda, że głosu nie można cofnąć.