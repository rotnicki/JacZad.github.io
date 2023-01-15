---
id: 411
title: 'Nazwa, rola i wartość (WCAG 2.0 SC 4.1.2, poziom A)'
date: '2012-11-29T13:15:23+01:00'
layout: post
guid: 'http://informaton.pl/?p=411'
permalink: /2012/11/29/nazwa-rola-i-wartosc-wcag-2-0-sc-4-1-2-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - formularze
    - wzrok
---

Technologie asystujące, w tym przede wszystkim czytniki ekranu, muszą mieć jasną i pewną informację na temat interfejsu użytkownika. Wszelkiego rodzaju zakłócenia, niejasności mogą wpłynąć negatywnie na możliwość korzystania przez osoby niepełnosprawne z serwisów internetowych. Jednak na takie same problemy napotykać mogą programy przetwarzające zasoby sieciowe, na przykład katalogujące treści. Dlatego każdemu elementowi interfejsu trzeba przypisać nazwę i rolę, a wartość powinna być łatwa do odczytania.

Kryterium sukcesu 4.1.2 zobowiązuje do projektowania interfejsów użytkownika w taki sposób, by każdemu elementowi była przypisana nazwa i rola, a wartość była dostępna dla technologii asystujących. Skorzystają na tym:

- użytkownicy niewidomi,
- programiści.

### Nazwa

Elementami interfejsu serwisu internetowego są linki, elementy formularzy i inne elementy, za pomocą których użytkownik może wchodzić z serwisem w interakcje. Każdy z takich elementów powinien mieć zdefiniowaną nazwę (identyfikator), który pozwoli na jego identyfikację. W wypadku formularzy robi się to standardowo, ale w wypadku linków – niekoniecznie. Tymczasem taki identyfikator może wydatnie ułatwić obsługę elementu przez skrypty, a przede wszystkim pozwala na bezproblemową obsługę przez czytniki ekranu.

### Rola

Dla dobrej obsługi przez czytniki ekranu jeszcze bardziej kluczowe jest określenie roli, jaką pełni w interfejsie dany element. Czasem wynika to z samego typu kontrolki i wówczas nie ma potrzeby niczego doprecyzowywać Tak jest w sytuacjach, gdy stosuje się standardowe kontrolki typu BUTTON, CHECKBOX, czy też TEXTAREA. Jednak coraz częściej programiści wykorzystują kontrolki do innych celów, na przykład link zamiast przycisku lub element listy jako checkbox. W takiej sytuacji należy takiemu elementowi przypisać jego faktyczną rolę, jaką pełni w interfejsie, za pomocą atrybutów oferowanych przez ARIA (Accessible Rich Internet Aplications). Po takim przypisaniu interfejs pośredniczący pomiędzy serwisem internetowym, a czytnikiem ekranu przekazuje prawidłową informację i użytkownik nie ma problemów z jego obsłużeniem.

### Wartość

Ostatnim elementem, jaki należy uwzględnić w projektowaniu interfejsów, jest łatwy dostęp do informacji o wartości lub stanie kontrolki. Ponownie – w wypadku standardowych kontrolek nie ma z tym większego problemu, bo pole wyboru jest zaznaczone lub nie, w polu edycyjnym jest coś wpisane, a na liście wyboru coś wybrane. Problem pojawia się, gdy tworzy się bardziej skomplikowane struktury, których HTML nie przewiduje, na przykład zakładki, menu czy drzewa. Wówczas trzeba przekazać wyraźnie informację o stanie kontrolki (zaznaczone, rozwinięte itp.), która może zostać zaprezentowana użytkownikowi. Ponownie można wykorzystać odpowiednie atrybuty ARIA, które są stale rozbudowywane i wciąż ich przybywa.