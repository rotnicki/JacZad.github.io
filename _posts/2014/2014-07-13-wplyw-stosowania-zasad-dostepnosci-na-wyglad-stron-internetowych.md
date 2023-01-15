---
id: 1083
title: 'Wpływ stosowania zasad dostępności na wygląd stron internetowych'
date: '2014-07-13T10:57:47+02:00'
layout: post
guid: 'http://informaton.pl/?p=1083'
permalink: /2014/07/13/wplyw-stosowania-zasad-dostepnosci-na-wyglad-stron-internetowych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audiodeskrypcja
    - estetyka
    - formularze
    - klawiatura
    - kolor
    - napisy
    - semantyka
    - 'WCAG 2.0'
    - wygląd
---

Co jakiś czas słyszę narzekania, że stosowanie wytycznych dostępności ma negatywny wpływ na wygląd serwisu internetowego. Zawsze staram się przekonać rozmówcę, że tak nie jest i obiecuję sobie w duchu przygotowanie zestawienia kryteriów sukcesu z opisem ich wpływu na wygląd. Wreszcie się zmobilizowałem i przedstawiam pierwszą część, kryteria na poziomie A.

Przez “wygląd” będę rozumiał w tym zestawieniu nie tylko odbiór wzrokowy, ale też słuchowy. Czynię to zastrzeżenie, bo nie umiem znaleźć odpowiedniejszego słowa na odbiór zmysłowy informacji płynących ze strony internetowej, które byłoby proste. A zatem poniżej zestawienie.

### Kryteria sukcesu WCAG 2.0 na poziomie A i ich wpływ na wygląd strony internetowej

1. **1.1.1 Treść nietekstowa** Spełnienie tego kryterium nie wpływa na wygląd strony internetowej, bo teksty alternatywne są ukryte pod elementami nie tekstowymi. Jeżeli projektant stosuje inną technikę, na przykład podpisy do ikon, to czyni to na własną odpowiedzialność, a wygląd też się nie zmienia.
2. **1.2.1 Tylko audio lub tylko wideo (nagranie)** Najprostszym sposobem zapewnienia zgodności jest dostarczenie transkrypcji tekstowej dla dźwięku lub obrazu (zależnie od rodzaju medium) jako oddzielnego dokumentu. Wymaga to dodania linku lub przycisku wyświetlającego taką transkrypcję, co może wpływać na wygląd strony.
3. **1.2.2 Napisy rozszerzone (nagranie)** Dodanie do filmów napisów dla osób niesłyszących nie ma wpływu na wygląd, o ile są to napisy zamknięte, czyli włączane i wyłączane przez użytkownika. Jedynym elementem wpływającym na wygląd jest w tym przypadku konieczność dodania przycisku do aktywowania napisów, jak to ma miejsce na przykład w YouTube. Jeżeli są to napisy otwarte, to mają wpływ na wygląd, chociaż użytkownicy są raczej do tego rozwiązania przyzwyczajeni w kinach i przy oglądaniu filmów w innych sytuacjach.
4. **1.2.3 Audiodeskrypcja lub alternatywa dla mediów (nagranie)** Dodanie transkrypcji tekstowej zmienia wygląd o tyle, że wymaga dodania przycisku lub linku do oddzielnego dokumentu tekstowego lub nagrania. Korzystając z audiodeskrypcji pojawia się taki sam wybór, jak w wypadku napisów – audiodeskrypcja zamknięta lub otwarta. Zamknięta wymaga dodania kolejnego przycisku lub linku do jej aktywowania, więc wpływ na wygląd jest niewielki. Większy problem jest z audiodeskrypcją otwartą, bo irytuje widzących użytkowników.
5. **1.3.1 Informacje i relacje** Wszystko powinno odbywać się na poziomie semantycznym, to znaczy kodu strony, co nie ma, a raczej – nie powinno mieć wpływu na wygląd.
6. **1.3.2 Zrozumiała kolejność** Podobnie jak relacje, także kolejność oparta jest o semantykę dokumentu. Strona zrobiona porządnie spełni to kryterium i nie będzie to miało wpływu na wygląd.
7. **1.3.3 Właściwości zmysłowe** Spełnienie kryterium nie wpływa w najmniejszym stopniu na wygląd, ponieważ dotyczy tylko sformułowań zawartych w informacjach tekstowych.
8. **1.4.1 Użycie koloru** Spełnienie tego kryterium może mieć wpływ na wygląd strony, szczególnie przy oznaczaniu istotnych informacji.
9. **1.4.2 Kontrola odtwarzania dźwięku** Spełnienie kryterium może mieć wpływ na wygląd strony, o ile korzysta ona z rozwiązania w postaci automatycznie odtwarzanego dźwięku. Dotyczy to także dźwięku w nagraniach audiowideo, na przykład reklam.
10. **2.1.1 Klawiatura** Spełnienie kryterium nie ma żadnego wpływu na wygląd, bo realizowane jest na niższym poziomie.
11. **2.1.2 Brak pułapki na klawiaturę** Podobnie jak poprzednie, także to kryterium nie wpływa na wygląd, bo realizowane jest na niższym poziomie.
12. **2.2.1 Możliwość dostosowania czasu** Spełnienie tego kryterium może wpływać na wygląd tylko przez konieczność dodania przycisku pozwalającego na sterowanie czasem.
13. **2.2.2: Wstrzymywanie (pauza), zatrzymywanie, ukrywanie** Kryterium to pozwala na stosowanie ruchomych elementów, ale zobowiązuje do zapewnienia możliwości zatrzymania, wstrzymania lub ukrycia. Zatem wpływ na wygląd będzie podobny, jak w poprzednim wypadku, przez konieczność dodania przycisku realizującego taką funkcję.
14. **2.3.1 Trzy błyski lub wartości poniżej progu** Spełnienie tego kryterium wpływa na wygląd strony internetowej, bo wprost zabrania stosowania na niej pewnego rodzaju elementów.
15. **2.4.1 Możliwość pominięcia bloków** Dodanie skiplinków z całą pewnością wpływa na wygląd strony internetowej, a jest to zalecana technika. Tym bardziej, że nie wolno ich ukrywać za pomocą stylów lub w inny sposób.
16. **2.4.2 Tytuły stron** To kryterium nie wpływa na wygląd strony internetowej, chociaż wpływa na wygląd przeglądarki. Tytuł strony jest bowiem wyświetlany na jej pasku tytułu, obok nazwy samej przeglądarki.
17. **2.4.3 Kolejność fokusa** Spełnienie tego kryterium nie wpływa na wygląd strony, ponieważ realizowane jest na poziomie semantycznym.
18. **2.4.4 Cel linku (w kontekście)** Spełnienie tego kryterium może mieć wpływ na wygląd strony internetowej, ponieważ może wymusić jej przebudowę. Najczęściej dotyczy to łączy umieszczonych w tabelach lub w inny sposób rozmieszczonych w przestrzeni. Samo umieszczenie w tabeli jeszcze nie narusza tego kryterium, o ile równocześnie spełnione jest kryterium 1.3.1, ale często robione jest to bardziej po bałaganiarsku.
19. **3.1.1 Język strony** Deklaracja języka nie ma żadnego wpływu na wygląd strony internetowej.
20. **3.2.1 Po oznaczeniu fokusem** Spełnienie tego kryterium może mieć wpływ na wygląd strony internetowej przez zmianę w sposobie jej działania. Może na przykład wymusić pojawienie się dodatkowych informacji tekstowych lub kontrolek.
21. **3.2.2 Podczas wprowadzania danych** Tutaj sytuacja ma się podobnie, jak w wypadku poprzedniego kryterium.
22. **3.3.1 Identyfikacja błędu** Kryterium wymusza stosowanie komunikatów tekstowych o błędach, a zatem może mieć wpływ na wygląd strony internetowej.
23. **3.3.2 Etykiety lub instrukcje** To kryterium ma wpływ na wygląd formularzy, bo nakazuje wyświetlanie etykiet i instrukcji, które bywają czasem ukrywane ze względów estetycznych.
24. **4.1.1 Parsowanie** Kryterium nie wpływa na wygląd strony internetowej, bo zobowiązuje do stosowania poprawnego kodu. Wątpliwości może budzić jedynie stosowanie prefiksowanych elementów stylów, na przykład eksperymentalnych rozwiązań Mozilli lub Opery, bo ich obecność może generować błędy parsowania, a brak – wpłynąć na wygląd.
25. **4.1.2 Nazwa, rola, wartość** Spełnienie tego kryterium odbywa się na poziomie semantycznym i nie ma wpływu na wygląd strony internetowej.

### Podsumowanie

Po gruntownym przyjrzeniu się temu zestawieniu można zauważyć pewne grupy kryteriów:

- nie wpływające w żaden sposób na wygląd strony;
- wpływające przez konieczność dodania elementów sterujących, które można ładnie wkomponować w stronę,
- wpływające silnie na wygląd i sposób konstrukcji strony przez nakazywanie lub zakazywanie stosowania pewnych rozwiązań.

O ile dodanie kolejnego elementu sterującego na stronie nie jest problematyczne, to kilka zakazów i nakazów może sprawić problemy projektantom i programistom. Zakaz używania elementów migających i odtwarzania dźwięku oraz nakaz stosowania skiplinków i jawnych etykiet na pewno zmieni nieco wygląd strony. Mam jednak wrażenie, że tego typu zmiany mogą wyjść  
stronie na dobre, czyniąc je przyjemniejszymi w użyciu dla wszystkich użytkowników. Trzeba też wziąć pod uwagę, że powyższe kryteria sukcesu są związane tylko z najniższym poziomem dostępności, a na poziomie AA kryteriów wpływających na wygląd może być znacznie więcej. W każdym razie listę argumentów do dyskusji już mam przygotowaną. A czy wpływ jest istotny, czy też nie – niechaj ocenią sami projektanci.