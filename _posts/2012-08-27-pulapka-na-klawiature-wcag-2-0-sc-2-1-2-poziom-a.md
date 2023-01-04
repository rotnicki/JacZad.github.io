---
id: 188
title: 'Pułapka na klawiaturę (WCAG 2.0 SC 2.1.2, poziom A)'
date: '2012-08-27T09:21:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=188'
permalink: /2012/08/27/pulapka-na-klawiature-wcag-2-0-sc-2-1-2-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - fokus
    - interfejs
    - klawiatura
    - myszka
    - nawigacja
    - niewidomi
---

Na klawiaturę nie wolno zastawiać pułapki! Jeżeli ktoś chce lub musi korzystać z tego sposobu wprowadzania danych i nawigacji, to nie wolno mu tego utrudniać.

Kryterium sukcesu 2.1.2 zabrania tworzenia pułapek na fokus sterowany klawiaturą. Jeżeli do danego elementu można dotrzeć za pomocą klawiatury, to można go także za pomocą klawiatury opuścić. Skorzystają z tego:

- użytkownicy z niedowładami rąk,
- użytkownicy terminali wyposażonych tylko w klawiaturę,
- użytkownicy niewidomi.

Rzecz jest bardzo prosta – programista powinien unikać tworzenia serwisu internetowego w taki sposób, by jakikolwiek element interfejsu więził kursor. Standardowe kontrolki HTML tego na pewno nie robią, ale czasem ktoś wpada na pomysł, by dodatkowo oprogramować na przykład formularz. Kursor jest przetrzymywany w danym polu do momentu, aż zostanie wykonana jakaś dodatkowa akcja przy pomocy myszy. Co jednak w wypadku, gdy użytkownik nie ma myszy lub nie może jej użyć? Nawigacja musi odbywać się metodami standardowymi (klawisze kursorów, tabulatora i spacji) lub w jasno określony sposób, na przykład przy użyciu skrótów klawiaturowych.