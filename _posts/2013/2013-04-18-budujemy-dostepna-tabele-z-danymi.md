---
id: 675
title: 'Budujemy dostępną tabelę z danymi'
date: '2013-04-18T16:47:57+02:00'
layout: post
guid: 'http://informaton.pl/?p=675'
permalink: /2013/04/18/budujemy-dostepna-tabele-z-danymi/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - podpisy
    - semantyka
    - tabele
    - 'WCAG 2.0'
---

Tabele obecne w elektronicznych dokumentach, w tym na stronach internetowych, służą do prezentacji danych tabelarycznych. Zbudowanie dostępnej tabeli jest dosyć proste, o ile stosuje się kilka prostych zaleceń, które opisuję poniżej.

## Tabela to nie blejtram

Język HTML dostarcza kilku znaczników do budowania tabel, ale mają to być faktycznie tabele, czyli struktura zawierająca dane w układzie pionowym i poziomym. Znaczników tych nie powinno się stosować do budowania układu wyglądu strony internetowej. Jest to rozwiązanie błędne i nieeleganckie, a na dodatek świadczy o niewielkich umiejętnościach projektanta. Jeżeli już jednak ktoś tak robi lub zastał taką sytuację, to może podreperować dostępność przekazując informację o tej funkcji tabeli.

```
<table role="presentation">
...
</table>

```

Przypisanie atrybutu informującego o roli prezentacyjnej tabeli sprawi, że będzie ona ignorowana przez oprogramowanie asystujące. Z drugiej strony – nie wolno do danych tabelarycznych stosować innych rozwiązań, na przykład pozycjonowania za pomocą stylów lub – o zgrozo – rozsuwania znakami tabulacji lub spacjami. To nie jest żadna tabela, tylko ciąg tekstu, nie nadający się do przetworzenia. Nie można się w nim poruszać jak po tabeli, przenieść do arkusza kalkulacyjnego, ani domyślić zależności.

## Nagłówki, podpis i objaśnienie

Większość tabel ma konstrukcję taką, że w pierwszym rzędzie lub w pierwszej kolumnie są dane nagłówkowe. Informują one czytelnika o tym, jakiego typu dane znajdują się w poszczególnych komórkach. Przyjrzyjmy się takiej oto tabelce:

```
<table summary="Tabela ma dwa wiersze i pięć kolumn. W pierwszym wierszu znajdują się rok, a w drugim wysokość minimalnego wynagrodzenia w złotych">
<caption>Minimalne wynagrodzenie w latach 2008-2013</caption>
<tr>
<th>2009</th><th>2010</th><th>2011</th><th>2012</th><th>2013</th>
</tr>
<tr>
<td>1276</td><td>1317</td><td>1386</td><td>1500</td><td>1600</td>
</tr>
</table>

```

Komórki nagłówkowe umieszczone są w znaczniku TH, a zwykłe dane w znaczniku TD. Użytkownik programu odczytu ekranu przemieszczając kursor po tabeli będzie miał informację kontekstową, na przykład odczytując kwotę “1600” dowie się, że jest ona aktualna w roku 2013. Z tego samego powodu **nie wolno** stosować znaczników TH do zwykłych danych, ponieważ wprowadzają zamieszanie informacyjne.

Podpis umieszczany w znacznikuCAPTION stosuje się zupełnie standardowo. W przykładzie zawarty jest jednak element niezbyt często stosowany, a mianowicie atrybut SUMMARY. Służy on do umieszczania w nim opisu struktury tabeli, która ma ułatwiać zrozumienie osobom nie mającym dostępu do całości, przede wszystkim niewidomym i słabowidzącym. Opis ten nie będzie widoczny, a jedynie odczytywany za pomocą programów odczytu ekranu.

## Układ tabeli

Tabela z danymi może mieć prosty układ, w którym w każdym rzędzie i kolumnie jest tyle samo komórek. Jest to układ najkorzystniejszy z punktu widzenia osób z niepełnosprawnością wzroku. Czasem jednak komórki łączy się w poziomie lub pionie, w celu uzyskania odpowiedniego efektu wizualnego lub informacyjnego. O ile to możliwe, to należy tego unikać w wypadku komórek z danymi. Komórki nagłówkowe można łączyć, ponieważ w mniejszym stopniu zaburzają odbiór takiej tabeli. Jednak w takim wypadku **koniecznie** powinny być ujęte w znaczniki TH.

Na koniec warto powiedzieć, że istotne jest także to, w którą stronę zorientowana jest tabela. Dane tabelaryczne odczytywane są przez osoby niewidome w sposób sekwencyjny: od lewego górnego rogu, przesuwając się w prawo do końca wiersza, przechodząc do pierwszej komórki drugiego wiersza i tak do prawego dolnego rogu. W tej sytuacji układ w tabeli zaprezentowanej powyżej nie jest optymalny, ponieważ użytkownik odczytuje najpierw po kolei lata, a potem po kolei wysokość minimalnego wynagrodzenia. Czytniki ekranu posiadają narzędzia, by przemieszczać się po tabeli w inny sposób, ale nie jest to postępowanie standardowe. Nieco lepszym rozwiązaniem byłoby zatem odwrócenie tej tabeli w taki sposób, że miałaby dwie kolumny (pierwsza z rokiem i druga z wysokością wynagrodzenia) i pięć wierszy. Odczytując ją sekwencyjnie użytkownik najpierw czytałby rok, a potem odpowiadającą mu wysokość minimalnego wynagrodzenia.

Minimalne wynagrodzenie w latach 2008-2013
| 2009 | 2010 | 2011 | 2012 | 2013 |
|---|---|---|---|---|
| 1276 | 1317 | 1386 | 1500 | 1600 |