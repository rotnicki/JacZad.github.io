---
id: 548
title: 'Do oceny dostępności serwisu internetowego nie wystarczy automat'
date: '2013-01-28T16:20:48+01:00'
layout: post
guid: 'http://informaton.pl/?p=548'
permalink: /2013/01/28/do-oceny-dostepnosci-serwisu-internetowego-nie-wystarczy-automat/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - narzędzia
    - specyfikacja
    - walidacja
---

Do napisania tego tekstu natchnęły mnie dwie rozmowy, jakie odbyłem ostatnio. Obie dotyczyły sposobu przyjmowania zamówionego serwisu internetowego i w obu przypadkach padła propozycja, by warunkiem było pozytywne przejście walidacji dostępności za pomocą konkretnego narzędzia. To bardzo zły pomysł, co postaram się za chwilę wyłuszczyć.

## Kto drogi prostuje, ten w polu nocuje

To hobbickie przysłowie pasuje jak ulał do sytuacji. Instytucja lub osoba zamawiająca serwis internetowy zgodny z zaleceniami dostępności musi jakoś ten produkt odebrać. Potrzebuje więc przynajmniej cień pewności, że serwis jest naprawdę dostępny. Samemu stwierdzić coś takiego jest dosyć trudno, więc szuka się drogi na skróty, czyli właśnie raportu z narzędzia do walidacji. Jednak takie narzędzie jest stosunkowo łatwo oszukać, jeżeli ktoś będzie miał taką potrzebę. Efektem będzie niedostępny serwis mający świetny wskaźnik walidacji.

## Narzędzia dla webmastera

Walidatory dostępności są narzędziem dla webmastera, które pomagają mu odnaleźć błędy, a czasem je usunąć. Te lepsze – oprócz wskazania problemu – potrafią podpowiedzieć, jak go rozwiązać i dlaczego należy to zrobić. Trzeba też bardzo mocno podkreślić, że dostępne walidatory nie są i nigdy nie będą w stanie sprawdzić wszystkich elementów dostępności. Potrafią w sposób w miarę dokładny wskazać ewidentne błędy semantyczne, braki w kodzie, przeanalizować kolorystykę, a nawet rozbłyski mogące wywołać atak epilepsji. To wszystko są jednak elementy sparametryzowane, które można precyzyjnie zbadać i automatycznie ocenić. Jest jednak bardzo wiele elementów, których w ten sposób już się nie da zbadać, chociażby dlatego, że generowane są przez skrypty pod wpływem działań użytkowników.

## Dobra i zła wola

Od biedy można się zdecydować na zatwierdzenie odbioru za pomocą raportu w wypadku zaufanego wykonawcy, który – w razie potrzeby – dokona później niezbędnych poprawek. Jednak w wypadku wykonawcy, do którego nie mamy zaufania lub po prostu go nie znamy – zrobić czegoś takiego nie wolno. Narzędzia walidujące można stosunkowo łatwo oszukać, chociażby umieszczając wątpliwy kod w skryptach JavaScript i w ten sposób maskując niedociągnięcia. Można też wszystkim grafikom przypisać losowy ciąg znaków jako tekst alternatywny i mieć klepnięte spełnienie [kryterium sukcesu 1.1.1](http://informaton.pl/?p=19) lub podobnie postępując z etykietami formularzy. Nie można tu zakładać dobrej woli, bo wykonawcy zależy, by oddać pracę jak najszybciej i z jak najmniejszym nakładem pracy. Trzeba założyć, że – podobnie jak w polityce społecznej – gdy wskaźnik staje się celem, to przestaje być dobrym wskaźnikiem.

## A zatem co należy zrobić?

Najlepszym rozwiązaniem jest zamówienie zewnętrznego audytu dostępności serwisu internetowego. Nie wolno poprzestać na oświadczeniu wykonawcy, że serwis jest zgodny z WCAG 2.0, bo widziałem już takie oświadczenia drastycznie niezgodne z prawdą. Skoro odbiorca się na tym nie zna, to przecież i tak nie sprawdzi prawdziwości oświadczenia, a papier zniesie wszystko. Ryzykownym pomysłem jest także żądanie takiego audytu od wykonawcy, który może go przecież zlecić podmiotowi bez kompetencji lub wręcz kupić bezwartościowy raport. Może jestem zbyt podejrzliwy, ale jeżeli już wydawane są spore pieniądze, to niech będą wydane dobrze.