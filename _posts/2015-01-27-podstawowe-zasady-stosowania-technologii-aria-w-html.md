---
id: 1246
title: 'Podstawowe zasady stosowania technologii ARIA w HTML'
date: '2015-01-27T12:22:07+01:00'
layout: post
guid: 'http://informaton.pl/?p=1246'
permalink: /2015/01/27/podstawowe-zasady-stosowania-technologii-aria-w-html/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - formularze
    - HTML
    - HTML5
    - klawiatura
    - specyfikacje
    - standardy
---

<span lang="en">Accessible Rich Internet Applications</span> (ARIA) to technologia, której należy używać z umiarem i umiejętnie. Ona nie służy do tworzenia interfejsu, a tylko do jego uzupełniania w sytuacjach, gdy standardowe kontrolki HTML się nie sprawdzają. W przystępny sposób opisuje to dokument opublikowany przez W3C <span lang="en">(World Wide Web Consortium)</span> w dokumencie [Using WAI-ARIA in HTML](http://www.w3.org/TR/aria-in-html/#first-rule-of-aria-use). Poniżej tylko krótka lista po polsku, a sam materiał źródłowy zawiera przykłady dobrych i złych rozwiązań.

Dokument wymienia 5 podstawowych zasad stosowania ARIA:

1. Jeżeli możesz – używaj natywnych kontrolek HTML. Jest to rozwiązanie bezpieczniejsze i bardziej uniwersalne od łatania za pomocą ARIA.
2. Nie zmieniaj natywnych kontrolek za pomocą ARIA. Jeżeli chcesz utworzyć przycisk, to skorzystaj z odpowiedniego znacznika, a nie roli przypisanej do innego znacznika.
3. Każdy element przygotowany w technologii ARIA musi być dostępny z poziomu klawiatury. Oznacza to, że musi się na nim dać umieścić fokus oraz wchodzić z nim w interakcje za pomocą klawiatury.
4. Elementy aktywne (przyciski, linki, elementy formularzy) nie mogą mieć przypisanej roli “presentation” lub być ukryte za pomocą atrybutu aria-hidden=”true”. Fokus będzie bowiem przemieszczony i umieszczony na… niczym.
5. Każdy interaktywny element używający ARIA musi mieć dostępną nazwę (etykietę). Nazwa musi wynikać wprost z odpowiedniego kodu, a nie z otoczenia graficznego, które może nie być dostępne podczas pracy za pomocą klawiatury.

Wymagań nie jest dużo, a tak często są ignorowane. Spotykałem już pola edycyjne z rolą przycisku, przyciski z rolą łącza i podobne wynalazki. I wcale nie w niszowych samoróbkach eksperymentatorów webowych, ale w aplikacjach od Google lub Microsoftu. Chociaż oni się uczą i wychodzi im coraz lepiej.