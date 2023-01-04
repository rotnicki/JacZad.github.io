---
id: 616
title: 'Dostęp do elementów nieaktywnych za pomocą klawiatury'
date: '2013-02-24T09:39:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=616'
permalink: /2013/02/24/dostep-do-elementw-nieaktywnych-za-pomoca-klawiatury/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - fokus
    - klawiatura
    - semantyka
---

Jakoś ostatnio namnożyło się na stronach elementów, które trzeba kliknąć myszką, a nie da się do nich dotrzeć za pomocą klawiatury. Jest to naruszenie kryterium sukcesu 2.1.1, a zatem bardzo poważna usterka. Warto zatem poświęcić kilka akapitów temu problemowi.

## Dostęp za pomocą klawiatury jest ważny

Nie każdy musi używać myszy, a niektórzy użytkownicy nawet nie mogą tego robić. Część użytkowników niesprawnych manualnie musi korzystać z klawiatury, bo sterowanie urządzeniami wskazującymi (myszka, trackball) jest dla nich niewykonalne. Wyłącznie z klawiatury korzystają także użytkownicy niewidomi, bo w ich przypadku niemożliwa jest koordynacja wzrokowo-ruchowa, niezbędna do posługiwania się myszką. wreszcie – wielu zaawansowanych użytkowników woli używać klawiatury, bo jest to po prostu szybsza metoda pracy. Koniecznie zatem należy zadbać o to, by do każdego elementu aktywnego dało się dotrzeć i aktywować za pomocą klawiatury.

## Prawidłowe korzystanie z elementów HTML

Język HTML daje całą kolekcję elementów, które domyślnie przechwytują fokus klawiatury. Są to wszystkie kontrolki formularzy oraz linki. Stosowanie linków lub przycisków BUTTON jest zachowaniem pożądanym, bo pozwala uniknąć ryzyka niedostępności dla klawiatury. Przeglądarka internetowa, interfejs dostępnościowy i technologie asystujące doskonale poradzą sobie z tymi elementami, a w drzewie DOM także znajdzie się dla nich stosowne miejsce.

Jednak programiści mają tendencję do stosowania niestandardowych rozwiązań. Podejrzewam, że głównie dlatego, że mogą, a nie dlatego, że to sensowne. Dlatego aktywnymi elementami czynią grafiki, elementy list, akapity i inne elementy, które domyślnie nie przyjmują fokusa klawiatury. Jednak zastosowanie akcji onClick sprawia, że taki bierny element można – w sposób sztuczny – uczynić aktywnym na kliknięcie myszą. Niestety – tylko myszą, bo dla klawiatury nie jest on dostępny. Taka technika bierze się z potrzeby precyzyjnego określenia wyglądu graficznego, co w wypadku niektórych elementów nie jest możliwe lub łatwe.

## Rozwiązanie problemu

Można jednak wykorzystać kilka prostych sztuczek, by taki mało aktywny element uczynić zupełnie dostępnym. Taka na przykład ikonka służąca do zapisywania pliku może wyglądać jak dyskietka z paska narzędzi w edytorze tekstów. Będzie to po prostu mały obrazek, który ze swej natury aktywny nie jest.

```
<img src="zapisz.jpg"
onclick="alert('działa!')">

```

W powyższym przykładzie wyświetli się obrazek, po kliknięciu którego wyskoczy okienko alertowe. Jednak dla użytkowników klawiatur będzie to element zupełnie bezużyteczny. Trzeba zatem uzupełnić kod w sposób, który przekona przeglądarkę, że da się go odwiedzić za pomocą klawiatury. Posłuży do tego atrybut TABINDEX.

Oczywiście należy także wstawić tekst alternatywny dla grafiki, chociaż akurat w tym przykładzie dałoby się domyślić funkcji przycisku z nazwy pliku. Jednak tutaj nie robimy takiego dziadostwa i porządny ALT też się musi znaleźć. Mamy zatem coś takiego:

```
<img src="zapisz.jpg"
alt="Zapisz plik"
tabindex="0"
onclick="alert('działa!')">

```

Niby już powinno działać, ale pozostało nam jeszcze jedno – przekonać przeglądarkę, a właściwie czytnik ekranu, że to jest przycisk. W przeciwnym wypadku da się co prawda dotrzeć do elementu za pomocą klawiatury, ale już niekoniecznie kliknąć spacją lub klawiszem enter. Wykorzystamy do tego rolę z wartością BUTTON.

```
<img src="zapisz.jpg"
alt="Zapisz plik"
tabindex="0"
role="button"
onclick="alert('działa!')">

```

Od tego momentu nasza ikonka będzie anonsowana jako przycisk i będzie działała jak przycisk. W ten sposób trochę oszukaliśmy oprogramowanie asystujące, ale w zbożnym celu. Pozostaje jedynie pytanie, czemu nie zrobić tego samego zgodnie ze sztuką, na przykład:

```
<button onclick="alert('Działa!')"><img src="zapisz.jpg" alt="zapisz plik"></button>

```

Na to odpowiedzi trzeba poszukać samemu, bo ja jej nie znam.