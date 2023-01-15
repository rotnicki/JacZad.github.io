---
id: 88
title: 'Tworzenie opisów alternatywnych grafiki na stronach internetowych (1) Dla webmasterów'
date: '2012-08-06T11:12:15+02:00'
layout: post
guid: 'http://informaton.pl/?p=88'
permalink: /2012/08/06/tworzenie-opisw-alternatywnych-grafiki-na-stronach-internetowych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - grafika
    - multimedia
    - 'tekst alternatywny'
    - tutorial
---

Artykuł jest efektem przemyśleń na temat sposobów opisywania grafiki w sposób alternatywny, na jakie napotykam czasem podczas przeglądania stron internetowych. Brak wiedzy na ten temat sprawia, że niektóre rozwiązania są nieco śmieszne, a niektóre bardzo irytujące. Opisywanie grafiki nie jest czymś trywialnym i wymaga nie tylko nieco pracy, ale też pewnej dozy pomysłowości, a przede wszystkim wiedzy.

### Dla kogo tekst alternatywny

Zacznę od tego, że mało kto zdaje sobie sprawę, po co tworzy się opisy alternatywne. Głównymi odbiorcami tej informacji są niewidomi użytkownicy Internetu, którzy używają do obsługi komputera (w tym także przeglądarki internetowej) programów do odczytu ekranu (ang. Screen reader), które przekazują użytkownikowi informacje za pomocą mowy syntetycznej lub alfabetu braille?a. Drugą dużą grupą odbiorców, niezwykle wprost ważną dla projektantów stron internetowych, są wyszukiwarki internetowe, na przykład Google, które nie są w stanie analizować grafiki, ale są w stanie odczytać opisy alternatywne. Dlatego serwisy, w których zadbano o opisy alternatywne do grafiki są lepiej indeksowane w wyszukiwarkach. Na koniec wreszcie ? opisywanie alternatywne jest potrzebne użytkownikom, którzy z różnych powodów wyłączyli ładowanie grafiki w przeglądarce. Zamiast informacji otrzymują prostokątny obszar, w którym powinien znajdować się obrazek. Jeżeli obrazek zaopatrzono w tekst alternatywny, to zostanie wyświetlony w tym prostokącie, a w przeciwnym wypadku użytkownik pozbawiony będzie jakiejkolwiek informacji.

### Wstawianie tekstu alternatywnego

Na początek to, co najprostsze ? opis alternatywny do zwykłej grafiki osadzanej za pomocą polecenia IMG. Specyfikacja HTML przewiduje dla tego znacznika specjalny atrybut ALT, którego wartością jest ciąg znaków umieszczony w cudzysłowach. To właśnie ten ciąg stanowi opis alternatywny, na przykład w taki sposób:

`<img src="listek_klonu.jpg" alt="Liść klonu">`

Czasem taki krótki opis jest niewystarczający, ale to także zostało przewidziane w specyfikacji HTML, dzięki czemu dysponujemy kolejnym atrybutem LONGDESC, czyli długi opis. Wartością tego atrybutu jest adres do strony zawierającej bardziej rozbudowany opis. W poniższym przykładzie prowadzi do odpowiedniego hasła w polskiej Wikipedii.

`<img src="listek_klonu.jpg" alt="Liść klonu" longdesc="http://pl.wikipedia.org/wiki/Klon_(ro%C5%9Blina)">`

Atrybut LONGDESC służy do linkowania do bardziej złożonych opisów, na przykład diagramów, tabel i podobnych. Jednak w praktyce okazał się mało użyteczny. W ogóle nie nadaje się w sytuacjach, gdy ma być opisem dla elementu aktywnego, na przykład łącza, ponieważ jest wywoływany w ten sam sposób. Dlatego zamiast ALT i LONGDESC warto stosować osadzanie obiektów.

Grafikę można osadzać na stronach internetowych za pomocą znacznika OBJECT. W ten sam sposób osadza się także inne elementy multimedialne, a ta metoda daje nawet więcej możliwości, niż atrybut ALT, ponieważ tekst wewnątrz ciała obiektu może być dowolnie skomplikowany. Poniżej przykład osadzenia wykresu i odpowiedniej informacji alternatywnej w postaci tabeli.

``

````

````

````

````

````

````

````

````

Wysokość minimalnego wynagrodzenia w latach 2010-2012
| rok | 2010 | 2011 | 2012 |
|---|---|---|---|
| w złotych | 11317 | 1386 | 1500 |

````

`<br></br>`

` `

Na koniec technika nazywana mapą bitową, czyli duży obszar, w którym wyróżnione są mniejsze obszary aktywne. Dobrym przykładem może być mapa Polski podzielona na województwa, taka jaka jest dostępna na stronie Pełnomocnika Rządu ds. Osób niepełnosprawnych pod adresem [http://www.niepelnosprawni.gov.pl](http://www.niepelnosprawni.gov.pl/).. Zapewniam, że mapa ta jest w pełni dostępna, choć wydaje się to niemożliwe. Aby zaprezentować odpowiednią technikę posłużę się przykładem z broszury ?Dostępne WWW? mojego autorstwa:

``

````

&lt;img src=”rodzina.jpg” usemap=”#rodzina” alt=”rodzina”&gt;

````

&lt;map name=”rodzina”&gt;

````

&lt;area href=”tata.html” shape=”circle” coords=”100,100,30″ alt=”Tata, czyli głowa rodziny”&gt;

````

&lt;area href=”mama.html” shape=”circle” coords=”170,120,30″ alt=”Mama, czyli prawdziwa głowa rodziny”&gt;

````

&lt;area href=”dziecko.html” shape=”circle” coords=”200,130,30″ alt=”Dziecko, zazwyczaj cwańsze od obu głów rodziny”&gt;

````

&lt;/map&gt;

`<br></br>`

``

Jak widać mechanizmy osadzania tekstów alternatywnych są proste i należy je stosować w zaprezentowany sposób. Przy czym zmiany zachodzące w specyfikacji HTML pokazują, że stosowanie znacznika OBJECT jest dużo bardziej elastyczne i wygodne. Zamiast grafiki można analogicznie osadzić film wideo lub applet Javy i zagwarantować dla nich pełną dostępność.