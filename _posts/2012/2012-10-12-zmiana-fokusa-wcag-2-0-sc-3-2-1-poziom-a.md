---
id: 309
title: 'Zmiana fokusa (WCAG 2.0 SC 3.2.1, poziom A)'
date: '2012-10-12T08:34:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=309'
permalink: /2012/10/12/zmiana-fokusa-wcag-2-0-sc-3-2-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - fokus
    - formularze
    - klawiatura
    - przewidywalność
---

Współcześnie projektowane serwisy internetowe często próbują domyślać się, czego chce użytkownik. Takie funkcje zaprogramowane są przez człowieka, który ma swoje wyobrażenie na temat sposobu pracy hipotetycznego użytkownika. Te wyobrażenia mogą być bardzo błędne i wówczas zamiast pomagać, takie rozwiązania utrudniają korzystanie z serwisu. Tak jest w wypadku akcji wyzwalanych automatycznie w momencie, gdy fokus znajdzie się na konkretnym elemencie interfejsu.

Kryterium sukcesu 3.2.1 zabrania projektowania interfejsów w taki sposób, że po przeniesieniu fokusa (punktu uwagi) następuje automatycznie zmiana kontekstu. Zmiana kontekstu oznacza otwarcie innego programu, zmianę obszaru kontrolowanego (otwarcie innej strony, wczytanie innej ramki), przeniesienie fokusa w inne miejsce lub zmianę sensu strony. Na przestrzeganiu tej zasady skorzystają:

- użytkownicy niewidomi i słabowidzący,
- użytkownicy klawiatur,
- użytkownicy z ograniczeniami kognitywistycznymi,
- seniorzy.

Serwis internetowy powinien zachowywać się w przewidywalny sposób, a w szczególności reagować na planowane działania użytkowników. Film powinien się odtwarzać po kliknięciu na przycisk “odtwarzaj”, a nie w momencie, gdy po prostu znajdzie się w punkcie uwagi. Użytkownicy klawiatur muszą przemieszczać się po stronie w sposób sekwencyjny i po kolei przesuwać fokus z elementu na element. Akcje wywoływane automatycznie poważnie utrudnią im dostęp do treści.

Stosowanie tej zasady nie ogranicza rozwiązań, gdzie wywoływane są akcje innego rodzaju. Na przykład umieszczenie fokusa w polu edycyjnym może wywołać kontekstową pomoc opisującą sposób wprowadzania danych. Jednak nie może to być wyskakujące okienko, przeglądarka plików PDF z instrukcją, a w szczególności fokus nie może być nigdzie przeniesiony. Sekwencyjność wymusza bowiem na użytkowniku odwiedzenie tego pola edycyjnego, nawet jeżeli nie zamierza tam nic wpisywać, a fokus chce przenieść dalej, na przykład do dalszego menu.