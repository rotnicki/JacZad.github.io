---
id: 150
title: 'Tekst, a nie obraz tekstu (WCAG 2.0 SC 1.4.5, poziom AA)'
date: '2012-08-19T10:48:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=150'
permalink: /2012/08/19/tekst-a-nie-obraz-tekstu-wcag-2-0-sc-1-4-5-poziom-aa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - czcionki
    - dokumenty
    - grafika
    - kolor
    - kontrast
    - powiększenie
    - tekst
    - wzrok
---

Tekst umieszczony w grafikach nie jest tekstem, chociaż mogłoby się tak wydawać. Jest obrazem tekstu, który niez nadaje się do przetwarzania jako łańcuchy tekstowe. Jest to grafika, którą można przetwarzać jak fotografie czy inne obrazy. A przecież niesie ze sobą (potencjalnie) informację tekstową. Taka grafika podlega ograniczeniom wynikającym z wybranego rodzaju medium i może być niedostępna dla wielu odbiorców.

Kryterium sukcesu 1.4.5 zaleca, by – jeżeli technologia na to pozwala – stosować raczej tekst niż obraz tekstu. Czyni przy tym dwa wyjątki od zasady. Po pierwsze – można od tego odstąpić, gdy obraz ztekstem może być przez użytkownika dostosowany do własnych potrzeb. Po drugie – gdy dokładny wygląd układu tekstu jest kluczowy dla zrozumienia informacji. Na przestrzeganiu tej zasady skorzystają:

- użytkownicy słabowidzący,
- użytkownicy przeglądarek z wyłączonym ładowaniem grafiki,
- użytkownicy przetwarzający informacje do innych form,
- użytkownicy wolnych łączy internetowych.

Opisana zasada najczęściej jest łamana przez publikowanie plików PDF powstałych przez zeskanowanie dokumentów papierowych. Takie pliki to kontenery PDF zawierające **obrazy** tekstu, a nie sam tekst. Takie pliki mają w zasadzie same wady:

- są znacząco, nawet stukrotnie, większe od swoich odpowiedników z warstwą tekstową,
- nie można ich przeszukiwać, zaznaczać i kopiować fragmentów,
- są niedostępne dla osób niewidomych i słabowidzących.

Można zatem zapytać, dlaczego w ogóle powstają. Odpowiedź jest prosta – bo komuś się wydaje, że jeżeli coś wygląda jak tekst, to jest tekstem, a to nie jest prawda. W dużym uproszczeniu można powiedzieć, że tekstem jest to, co można przetwarzać jak tekst. Można zatem usunąć jedną literę lub wyraz i zastąpić je innymi. Można też powiększyć czcionki lub zmienić ich krój. Tego właśnie dotyczy pierwsze odstępstwo od zasady.

Można sobie wyobrazić, że ktoś opracował technologię, która pozwala użytkownikowi dokonywać modyfikacji tekstu zawartego w grafice analogicznie, jak ma to miejsce w wypadku zwykłego tekstu. Autor daje możliwość zmiany kroju i wielkości czcionek, zmiany kolorów tła i tekstu, czy też zmiany odległości między literami, wyrazami i liniami tekstu. W takiej sytuacji WCAG dopuszcza umieszczanie tekstu w grafice. Nadal jednak obowiązuje ulokowane na poziomie A [kryterium sukcesu 1.1.1](http://informaton.pl/?p=19), co czyni przedsięwzięcie niecelowym.

Czasem precyzyjny układ informacji ma na tyle duże znaczenie, a jednocześnie trudno jest go oddać za pomocą standardowych mechanizmów, że tekst w grafice jest dopuszczalny. Dobrym przykładem jest publikowanie zrzutów ekranu, gdzie prezentowany jest cały interfejs użytkownika i zależności pomiędzy informacjami. Podobnie – schematy blokowe, grafy czy wykresy stanowią grafikę, w której ważnym elementem są ciągi tekstu. Także w tej sytuacji można umieścić takie obrazy tekstu, z jednoczesnym uwzględnieniem SC 1.1.1.