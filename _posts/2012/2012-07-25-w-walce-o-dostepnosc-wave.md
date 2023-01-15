---
id: 21
title: 'WAVE &#8211; narzędzie do walidacji i prezentacji'
date: '2012-07-25T09:26:55+02:00'
layout: post
guid: 'http://informaton.pl/?p=21'
permalink: /2012/07/25/w-walce-o-dostepnosc-wave/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - narzędzie
    - prezentacja
    - walidacja
---

![Logo Wave](https://i0.wp.com/wave.webaim.org/media/wavelogo.png?w=160)Dzisiaj moje ulubione narzędzie do walidacji dostępności stron internetowych. Nadaje się zarówno do wspomagania testowania, jak i na prezentacje.

Aplikacja nosi nazwę WAVE, co jest akronimem Web Accessibility Evaluation Tool, a dostępna jest pod adresem <http://wave.webaim.org/> Tamże można wpisać w pole edycyjne adres strony do sprawdzenia i uzyskania wyniku testu. Jest to jednak mało wygodne i polecam tutaj użycie wtyczki do przeglądarki Firefox dostępnej na podstronie [Toolbar](http://wave.webaim.org/toolbar/). Po zainstalowaniu dostajemy w przeglądarce wygodne narzędzie, które pokrótce opiszę.

### Błędy, ostrzeżenia i sztuczki

[![Zrzut ekranu z wyświetloną oryginalną stroną www.scon.waw.pl](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-1-300x168.jpg?resize=300%2C168 "Zrzut ekranu oryginalnej strony www.scon.waw.pl")](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-1.jpg)Wtyczki w zasadzie nie trzeba konfigurować, bo w opcjach znajdziemy wyłącznie ustawienia dla interfejsu użytkownika. Zatem otwieramy interesującą nas stronę internetową , którą w tym wypadku jest serwis internetowy Stołecznego Centrum Osób Niepełnosprawnych (SCON) i wybieramy z narzędzi to najważniejsze, czyli "Errors, features and alerts" i naszym oczom lub uszom ukazuje się strona w zupełnie innym świetle – upstrzona kolorowymi ikonkami informującymi o tym, z czego do tej pory nie zdawaliśmy sobie sprawy. W ten sposób można zwizualizować błędy i problemy na stronach internetowych.

[![Zrzut ekranu serwisu www.scon.waw.pl po użyciu narzędzia do wyświetlania błędów. Widoczne są kolorowe ikonki.](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-errors-1-300x168.jpg?resize=300%2C168 "Strona z ikonami błędów i ostrzeżeń")](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-errors-1.jpg)Ikony są w czterech kolorach i każdy z nich ma swoje znaczenie:

- czerwone oznaczają błąd dostępności, który koniecznie należy poprawić,
- żółte oznaczają ostrzeżenie, że w tym miejscu jest coś podejrzanego, co potencjalnie może generować błąd, ale program nie umie tego z pewnością stwierdzić,
- zielone oznaczają, że tutaj sprytny webmaster zastosował odpowiednie rozwiązanie, na przykład tekst alternatywny,
- niebieskie oznaczają, że webmaster był porządny i kodował stronę semantycznie.

A zatem – im więcej czerwonego i żółtego – tym gorzej. Kolory zielony i niebieski zaś to ordery przypinane do piersi webmastera. Od tego momentu jego misją życiową może stać się tępienie czerwonych i żółtych z równoczesnym mnożeniem zielonych i niebieskich. Troszkę tu zajechało rasizmem, ale to czysty przypadek.

Oczywiście nie tylko kolor jest ważny, bo to byłoby za mało informacji. Po wybraniu narzędzia "Icons key" otrzymujemy pełną listę wszystkich ikonek używanych w programie z objaśnieniem, co też one oznaczają. Krótką informację można uzyskać w dymku po najechaniu na ikonę już na stronie testowanej, ale komunikaty niekoniecznie muszą być dla wszystkich jasne. Tutaj można przeczytać dokładniej, do czego program się przyczepił, a zatem wiadome też będzie, jak się problemu pozbyć.

### Struktura dokumentu

Kolejne narzędzie pod nazwą "Structure/order" pozwala spojrzeć na stronę od strony kolejności elementów w niej zawartych. Kodując stronę opartą na stylach często można zapomnieć, że pod spodem jest kod semantyczny, który ma określoną kolejność. Układając z niemal dowolną swobodą elementy graficzne interfejsu warto czasem sprawdzić, jaką mają kolejność i czy ta kolejność ma sens. Tą ścieżkę można prześledzić dzięki wyświetlanym na stronie numerom kolejnym. Jeżeli wszystko wygląda z sensem, to w porządku. Program za nas nie sprawdzi logiki i trzeba to zrobić na własną rękę.

### Tryb tekstowy

[![Zrzut ekranu strony www.scon.waw.pl po użyciu narzędzia "tylko tekst". Tak odczytają tą stronę użytkownicy niewidomi.](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-text-1-300x168.jpg?resize=300%2C168 "www.scon.waw.pl w trybie tekstowym")](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/wawe-text-1.jpg)Wspomniałem już, że ta wtyczka nadaje się na prezentacje o dostępności, a to dzięki kolejnemu narzędziu – "Text-only". Po włączeniu można zobaczyć, jak wygląda strona w przeglądarce tekstowej lub jak jest słyszana przez niewidomego użytkownika. Taki widok potrafi wyrwać głośne westchnienie wśród zebranych na pokazie, bo znajoma do tej pory strona zamienia się w potwora ohydnego, a informacje znikają gdzieś jak kamfora. Jednak w wypadku stron dostępnych wrażenie jest dużo mniejsze, a funkcjonalność strony pozostaje bez zmian.

Podobnie można sobie obejrzeć stronę z wyłączonymi stylami, do czego służy narzędzie "Disable styles". Wciąż bowiem można spotkać przeglądarki, które słabo interpretują CSS, więc warto wiedzieć, czy strona nadal będzie użyteczna. Dodatkowym, choć moim zdaniem mało przydatnym narzędziem jest "Outline". Jest to coś podobnego do konspektu w edytorach tekstu, gdy zamiast całego dokumentu możemy obejrzeć jego strukturę. Jest to raczej narzędzie pomocnicze, uzupełniające komplet, niż samodzielne rozwiązanie testujące.

### Zastrzeżenie

Trzeba mieć świadomość, że żadne automatyczne narzędzie nie dokona pełnej analizy strony internetowej pod kątem dostępności. Jednak wyeliminowanie błędów i uważne przyjrzenie się ostrzeżeniom może rozwiązać większość problemów. Należy też zauważyć, że WAVE nie jest prymitywnym analizatorem kodu. Potrafi na przykład zwrócić uwagę na linki, które formalnie mają opis alternatywny, ale jest on podejrzany. Polecam wypróbowanie i przekonanie się osobiście.