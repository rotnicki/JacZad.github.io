---
id: 629
title: 'Skiplinki, landmarki i nagłówki &#8211; sposoby na ułatwienie nawigacji'
date: '2013-03-12T13:29:58+01:00'
layout: post
guid: 'http://informaton.pl/?p=629'
permalink: /2013/03/12/skiplinki-landmarki-i-naglwki-sposoby-na-ulatwienie-nawigacji/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - landmarki
    - nagłówki
    - skiplinki
---

Część użytkowników serwisów internetowych ma ograniczony dostęp do całości treści i korzysta tylko z konkretnego kawałka. Tak się dzieje w wypadku osób niewidomych, które posługują się stroną linearnie; słabowidzący, którzy widzą tylko wycinek strony, niekoniecznie z nawigacją; wreszcie użytkownicy małych wyświetlaczy, na których po prostu nie wszystko się mieści. Jak mają łatwo dotrzeć do interesującej ich części strony dokumentu?

Możliwość przeskoczenia do głównej treści dokumentu wymusza WCAG 2.0 w [kryterium sukcesu 2.4.1](http://informaton.pl/?p=243)i to już na poziomie A. Można jednak rozszerzyć te ułatwienia w nawigacji na znacznie więcej elementów: menu nawigacyjne, formularz wyszukiwania, stopkę, czy okno z reklamami. W każdym wypadku można skorzystać z różnych metod docierania do treści: nagłówków, skiplinków i landmarków. Każde z tych rozwiązań ma swoje wady i zalety, więc najlepiej jest stosować je wszystkie jednocześnie.

## Nagłówki

Nagłówki są bodaj najczęściej wykorzystywanym elementem nawigacyjnym przez osoby niewidome. Z tego powodu [powstał nawet mit, że należy całą treść upychać w nagłówki](http://informaton.pl/?p=627), co nie jest prawdą. Jednak prawidłowe stosowanie nagłówków faktycznie pomaga w nawigacji, więc warto je stosować. Trzeba przy tym pamiętać, że nagłówki poziomów 1-6 powinny być zagnieżdżane w sposób logiczny, a nie losowy. Na stronie powinien występować dokładnie jeden nagłówek poziomu pierwszego. Wadą tego rozwiązania jest fakt, że jest użyteczne wyłącznie dla osób niewidomych.

## Skiplinki

Skiplinki są linkami wewnętrznymi w dokumencie HTML, które prowadzą do konkretnego miejsca w danym dokumencie, a nie do innego dokumentu. Takie linki należy umieszczać na początku dokumentu, a wedle uznania – także na końcu, a nawet wewnątrz. Jednym z najpopularniejszych skiplinków jest umieszczany na końcu link pozwalający przenieść fokus na początek dokumentu, co jest dosyć często spotykane w portalach pod dłuższymi artykułami. Jednak dla osób niepełnosprawnych kluczowe są linki prowadzące do głównej treści dokumentu, na przykład tekstu artykułu, z pominięciem całego systemu nawigacji. Takie linki, o ile nie zostaną ukryte za pomocą stylów lub innych sztuczek, posłużą także użytkownikom małych wyświetlaczy, na przykład w smartfonach. Koniecznie należy też sprawdzić, czy skiplinki działają po użyciu klawiatury, gdyż inaczej będą nieużyteczne.

## Landmarki

Ostatnia metoda zaczerpnięta jest z bogatego arsenału dostępności ARIA. Landmarki to przypisanie roli do całego obszaru objętego znacznikiem lub po prostu layerem DIV. Całość polega na dodaniu atrybutu ROLE, którego wartością jest rodzaj treści, na przykład role=”main” określa główną treść dokumentu. Najważniejszymi landmarkami są:

- banner – treść dotycząca samego serwisu internetowego: logo, nazwa, ewentualnie wyszukiwarka,
- contentinfo – treść umieszczana zazwyczaj w stopce: informacje o prawach, dane kontaktowe, wykonawca itp,
- form – formularz lub zestaw kontrolek,
- main – główna treść dokumentu, na przykład treść artykułu,
- navigation – elementy nawigacji: menu, linki itp,
- search – system wyszukiwania informacji.

Nie są to wszystkie landmarki zawarte w dokumentacji ARIA, ale kilka wybranych, najczęściej stosowanych. Przy stosowaniu landmarków należy zadbać o kilka rzeczy:

1. Landmarki main, banner i contentinfo mogą wystąpić na pojedynczej stronie najwyżej raz.
2. Obszary objęte landmarkami muszą wypełniać całą treść dokumentu i żadna treść nie może znajdować się poza nimi.
3. Landmarki należy stosować zgodnie z ich przeznaczeniem, a przede wszystkim nie otaczać landmarkiem treści, która powinna być przypisana innemu typowi treści.

## Co stosować?

Pojawia się pytanie, którą z tych technik stosować… Odpowiedź jest prosta – wszystkie trzy. Każda jest skierowana do trochę innego odbiorcy, a jednocześnie nie kolidują one ze sobą. Ważne jest, by robić to konsekwentnie i w sposób logiczny.