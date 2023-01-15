---
id: 1081
title: 'Zapytanie ofertowe PFRON na wykonanie generatora wniosków'
date: '2014-07-10T09:20:03+02:00'
layout: post
guid: 'http://informaton.pl/?p=1081'
permalink: /2014/07/10/zapytanie-ofertowe-pfron-na-wykonanie-generatora-wnioskw/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - etykiety
    - 'generator wniosków'
    - klawiatura
    - PFRON
    - pieniądze
---

Państwowy Fundusz Rehabilitacji Osób Niepełnosprawnych (PFRON) opublikował [zapytanie ofertowe](http://www.pfron.org.pl/pl/komunikaty/2380,Zapytanie-ofertowe-w-sprawie-hostingu-oraz-uslug-programistycznych-swiadczonych-.html)na przygotowanie, a raczej zmodyfikowanie, generatora wniosków aplikacyjnych. W wymaganiach znajduje się zgodność z wymaganiami [WCAG 2.0](http://fdc.org.pl/wcag2/)na poziomie AA. Ponieważ jestem świeżo po pracy na tym systemie, to chętnie przyklasnę zmianom, bo praca z czytnikiem ekranu jest frustrująca. Poniżej zaś kilka sugestii płynących od użytkownika.

### Etykiety dla pól formularzy

Generator wniosków to przede wszystkim niezwykle rozbudowany formularz do wypełniania danymi. Ogromna liczba pól tekstowych, rozwijanych list, pól wyboru i opcji sprawia, że brak etykiet na stałe przypisanych do tych pól bardzo utrudnia pracę. Co prawda część z pól, szczególnie tekstowych, ma takie etykiety, ale brakuje ich w newralgicznych miejscach. Należą do nich harmonogram i budżet. W harmonogramie trzeba pracowicie odliczać kolumny, żeby w odpowiednim miejscu zaznaczyć pole wyboru, chociaż tak prosto jest dodać etykietkę z nazwą lub przynajmniej numerem miesiąca. W budżecie jest jeszcze gorzej, bo i jest on bardziej skomplikowany, a etykietek tam brakuje. Poza tym trzeba zadbać o etykiety do przycisków, które raz są, a innym razem ich nie ma.Można się nauczyć i klikać na pamięć, ale przecież nie o to chodzi.

### Wspomaganie nawigacji

W obecnej wersji generatora każda część wniosku to oddzielny, bardzo obszerny formularz. Oznacza to, że część B, czyli opis merytoryczny, jest wprost ogromny, zawiera bowiem opis działań, pełny opis form wsparcia, wskaźniki, opis zadań i wiele innych elementów. Nie byłoby w tym nic złego, gdyby zaopatrzyć ten formularz w jakiś poręczny system nawigacji, na przykład oparty o nagłówki. Nagłówek poziomu drugiego dla części o formach wsparcia i nagłówek poziomu 3 dla poszczególnych form wsparcia. Może nawet jeszcze czwarty poziom podziału wewnątrz opisu formy wsparcia, bo i tam da się wyróżnić mniejsze elementy. Teraz znajduję poszczególne fragmenty wyszukując tekst na stronie i nie jest to wygodne rozwiązanie.

### Pomoc w wypełnianiu formularza

Tutaj też jest sporo do poprawienia, bo obecne rozwiązania nie są optymalne. Przemieszczając się po formularzu za pomocą klawiatury słychać często podpowiedzi do konkretnych pól, ale dzieje się to zbyt często. Jest to szczególnie uciążliwe w tabeli budżetu, gdzie jest mnóstwo podobnych pól, z identycznymi podpowiedziami, czasem dosyć długimi. Jest to zdecydowanie zbyt redundantne (nadmiernie powtarzane), by wygodnie z tego mechanizmu korzystać. Pomoc powinna być dostępna na żądanie, a nie nachalnie wpychana użytkownikowi, który – być może – wcale jej nie potrzebuje. Trochę to wygląda tak, jakby po kliknięciu w każde pole użytkownikowi wyświetlało się ogromne okno z podpowiedzią zakrywające formularz, które trzeba za każdym razem zamknąć. Przy tej okazji wspomnę jeszcze o komunikatach o błędach i oknach modalnych, które zrobiono w sposób mocno niedostępny. Po pewnym czasie można się nauczyć, że jeżeli nie mogę czegoś zaznaczyć lub wpisać tekstu, to pewnie dlatego, że gdzieś jest jakieś otwarte okno z komunikatem, które trzeba zamknąć. Jest to jednak irytujące, a mniej doświadczonego użytkownika może wprawić w konfuzję.

### Tabele i tabelki

Wydawałoby się, że budżet i harmonogram są idealnymi przykładami stosowania tabel. Jednak w generatorze wniosków PFRON zrobiono z nimi coś dziwnego i zachowują się zupełnie nieprzewidywalnie. Nie chciało mi się analizować kodu, bo jest tam szczególnie zaplątany, ale dostrzegam efekty: problemy z nawigacją po kolumnach i wierszach tabeli. Z całą pewnością oba elementy nadają się do poprawy.

Do poprawienia jest tam jeszcze więcej, ale to raczej oczywistości. Ten generator i tak nie jest tak zły, jak poprzednia jego wersja instalowana na komputerze, chociaż na tym tle wszystko wygląda dobrze. Może wykonawca odnajdzie ten tekst i trochę mu on pomoże w wytworzeniu nowego generatora, z którym pracować będzie przyjemniej i łatwiej.