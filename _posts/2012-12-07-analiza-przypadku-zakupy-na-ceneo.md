---
id: 420
title: 'Analiza przypadku &#8211; zakupy na Ceneo'
date: '2012-12-07T16:07:02+01:00'
layout: post
guid: 'http://informaton.pl/?p=420'
permalink: /2012/12/07/analiza-przypadku-zakupy-na-ceneo/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - Ceneo
    - e-handel
    - formularze
---

Postanowiłem kupić do domu nawilżacz powietrza. Nie znam się, więc sięgnąłem do mojej ulubionej porównywarki cen [Ceneo](http://www.ceneo.pl) i po krótkich konsultacjach na Facebooku wybrałem konkretny model. A ponieważ od pewnego czasu Ceneo oferuje także sprzedaż produktów, a nie tylko ich porównanie, to postanowiłem skorzystać.

### Zaczynamy na spokojnie

Pierwszym krokiem było wybranie produktu, którym był [HB UH 1025](http://www.ceneo.pl/8684279?se=BlVCsvLCzgRlqh2HyOyE2T_H4ZjbMHZt&gclid=CL-klbSviLQCFQ1Y3godxQEAPA). Potem kliknąłem na przycisk “DODAJ DO KOSZYKA i sprawdziłem stan koszyka. Nadal było w nim zero produktów, więc kliknąłem jeszcze raz. Teraz miałem już dwa produkty… Zapewne treść nie odświeżyła się odpowiednio szybko, ale to można załatwić prostym atrybutem ARIA

Poprawiłem liczbę produktów na jeden i kliknąłem przycisk PRZELICZ i teraz było już w porządku. Koszyk się zgadzał, ale chciałem zmienić formę dostawy na kuriera. Przeszedłem więc do kasy i z rozwijanej listy wybrałem stosowną opcję. Kwota się przeliczyła i teraz byłem już zadowolony i gotowy do sfinalizowania transakcji.

### Sierotki etykietki

Zamierzałem złożyć zamówienie bez logowania, a zatem trzeba było wprowadzić moje dane teleadresowe. I tu pierwszy poważny zgrzyt, bo pola edycyjne nie miały przypisanych etykiet. Co ciekawsze – etykiety były oznaczone tagiem LABEL, ale latały sobie luzem. Jaki sens ma tworzenie etykiet, które nie są przypisane do kontrolek formularzy? Jednak te artefakty wskazują, że projektant już usłyszał dzwony, tylko kościół mu się na razie myli. Ciekawostka – etykiety do pól wyboru były użyte prawidłowo, a w wypadku pola na adres email zastosowano nawet ARIA. Dlaczego zatem w polach edycyjnych na dane jest taki bajzel? Jakoś przebrnąłem, chociaż z problemami przez to okno i przeszedłem do płacenia.

### Niedostępny świat obrazków

Jednak prawdziwy hardcore zaczął się po kliknięciu przycisku PŁACĘ, a ponieważ wybrałem przelew… Ukazało mi się 50 (słownie pięćdziesiąt) opcji wyboru, z których tylko jedna była opisana. Założyłem inteligentnie, że obok tych opcji są stosowne obrazki, zupełnie oczywiste dla widzących użytkowników. Dla mnie zaś były zupełnie niedostępne. Na szczęście żona była w domu, więc zerknęła i powiedziała mi, która z opcji odpowiada za mój bank. Potem już poszło z górki. Ponownie – tam były znaczniki etykiet, ale użyte w niedopuszczalny sposób. Walidator dostępności wykazał na tej podstronie “tylko” 26 błędów dostępności, a powinien przynajmniej trzykrotnie więcej.

### Podsumowanie

Podsumowując – panel transakcyjny Ceneo ma bardzo wiele niedoróbek. Część z nich jest do usunięcia niemal od ręki przez poprawienie błędów w rodzaju osieroconych etykiet. Część wymaga dodania opisów alternatywnych i sprawdzenia zachowań przy użyciu klawiatury. Robota na jeden dzień dla programisty. A ja, gdyby nie żona w domu, kupiłbym towar gdzieś indziej.