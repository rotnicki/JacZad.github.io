---
id: 1104
title: 'Analiza przypadku &#8211; kupuję elektroniczną książkę w Woblinku'
date: '2014-08-14T13:57:14+02:00'
layout: post
guid: 'http://informaton.pl/?p=1104'
permalink: /2014/08/14/analiza-przypadku-kupuje-elektroniczna-ksiazke-w-woblinku/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ebooki
    - EPUB
    - formularze
    - klawiatura
    - landmarki
    - nawigacja
    - pieniądze
    - sklep
    - 'tekst alternatywny'
    - Woblink
---

Zachęcony przez podcast ["Radio Stephen King"](http://radio-sk.blogspot.com/) postanowiłem kupić książkę Joe Hilla pod tytułem Nos4a2. Oczywiście ma to być ebook w formacie EPUB, a do tego – możliwie tanio. No i tak zaczęły się moje peregrynacje po e-księgarniach.

### Najpierw poszukam najtańszej oferty

Zacząłem od mojej ulubionej [wyszukiwarki ebooków w serwisie Świat czytników.](http://ebooki.swiatczytnikow.pl/), gdzie mogę wpisać tytuł książki i poszukać atrakcyjnych ofert. Przy filtrze odhaczyłem format PDF, którego nie lubię i wyświetliłem wyniki. Ceny wahały się od 22,77 złotych (Woblink) do 34,50 złotych (Legimi). Jak widać różnice w cenach są duże i warto korzystać z porównywarek. Zaczynam od najtańszej oferty.

### Woblink

Po kliknięciu w link do księgarni otwiera mi się od razu strona z opisem książki. Jest też jakiś suwak służący do ocenienia książki, ale nie jest dostępny z poziomu klawiatury. Na szczęście jest standardowy przycisk dodania do koszyka. Klikam i co dalej? Znajduję link do koszyka, przy którym jest informacja o liczbie produktów i koszcie. Klikam żeby sfinalizować transakcję.

### Płacę!

W tym momencie się zalogowałem i – na szczęście – system pamiętał o dodanej książce, chociaż zażądał potwierdzenia, że chcę ją dodać do koszyka. Pod koszykiem link “Płacę”, więc jesteśmy w ogródku. O nie! Wcale nie tak szybko! Muszę wybrać operatora płatności z dwóch, ale nie ma żadnych opisów tekstowych przy nich. Zapewne są jakieś logotypy, które mówią wszystko, ale nie mi. Zaryzykować? Zaryzykuję…

Wybrałem pierwszą opcję i chyba się udało. Teraz z przelewów elektronicznych wybieram mój bank, a przynajmniej sądzę, że wybieram, bo przycisk nie ma opisu. Opis jest obok i może dotyczyć także innego przycisku. Znowu na chybił-trafił… Uff… Udało się i po zalogowaniu do banku zrobiłem przelew.

### Pobieram książkę

Gwizdnął program pocztowy i w skrzynce odbiorczej wylądowały emaile potwierdzające transakcję. Zakupione książki są gotowe do pobrania, więc kliknąłem i przeniosło mnie od razu do serwisu na półkę. A tam po dłuższym poszukiwaniu docieram do książek, których już kilka kupiłem wcześniej. Na pierwszym miejscu świeży zakup, ale… niedostępny dla klawiatury! Trochę mnie zmroziło, bo już miałem sytuację, że nie mogłem pobrać kupionej pozycji i do tej pory mi się to nie udało. Klikam spacją i enterem i po kilku próbach rozwija się menu, w tym też “pobierz EPUB”. Ulga i już książka ląduje na moim dysku. Tylko czy ja muszę się tak stresować przy wydawaniu pieniędzy?

### Rekomendacje

Może kiedyś ktoś z Woblinka zajrzy do tego wpisu, więc niżej kilka rekomendacji do zmian. Poprawki nie wydają się być zawiłe, więc liczę na zmiany.

1. Poprawki w nawigacji. Strona nie jest bardzo duża, ale i tak nie ma potrzeby przeglądania jej w całości. Na stronie są landmarki, ale nie wszystkie, a szczególnie brakuje tego najważniejszego, czyli “main”. Warto też popracować nad nagłówkami, które teraz są dosyć przypadkowo umieszczone w kodzie, a mogłyby być pomocne.
2. Alternatywne teksty. Za poważne uchybienie należy uznać braki w tekstach alternatywnych dla elementów nie będących tekstem – grafik, kontrolek formularzy i innych. Szczególnie kiepsko to wygląda na etapie płacenia, gdy klient powinien mieć pewność, że robi wszystko dobrze, a nie po omacku. trzeba uzupełnić atrybuty ALT przy obrazkach (np. badge, formy płatności) i LABEL przy wszystkich elementach formularzy.
3. Dostęp z klawiatury. Wiele elementów nie jest dostępnych z poziomu klawiatury, co odczułem szczególnie przy próbie pobrania ebooka. To trzeba koniecznie poprawić, choćby stosując atrybuty ARIA. Skoro to jest przycisk, to niechże przeglądarka o tym wie.

Znalazłoby się jeszcze kilka rzeczy, ale powyższe powinny być wdrożone w pierwszej kolejności.