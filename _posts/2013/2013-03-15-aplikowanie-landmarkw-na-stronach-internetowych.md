---
id: 634
title: 'Aplikowanie landmarków na stronach internetowych'
date: '2013-03-15T13:18:11+01:00'
layout: post
guid: 'http://informaton.pl/?p=634'
permalink: /2013/03/15/aplikowanie-landmarkw-na-stronach-internetowych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - formularze
    - landmarki
    - nagłówki
    - nawigacja
---

Pisałem już o sposobach na szybsze docieranie do różnych obszarów, na przykład za pomocą skiplinków. Jednak ARIA pozwala na semantyczny podział strony internetowej i przypisanie poszczególnym fragmentom odpowiednich ról. Takie znaczniki rodzaju treści nazywane są landmarkami i są dodatkową warstwą informacji, przeznaczoną przede wszystkim dla niewidomych użytkowników.

## Struktura strony internetowej

Na stronie internetowej można dosyć łatwo dostrzec pewne stałe elementy (nagłówek, stopka, system nawigacji) oraz zmienne (główna treść, interfejs aplikacji, obiekty nie związane z treścią strony). Na bardziej rozbudowanych stronach takich elementów może być bardzo dużo, co poważnie utrudnia nawigację po serwisie osobom niewidomym. Zastosowanie landmarków do oznaczenia tych fragmentów może wybitnie skrócić czas niezbędny do odnalezienia treści lub elementu nawigacji. Aplikowanie landmarków jest technicznie bardzo łatwe, bo ogranicza się do przypisania roli dla konkretnego obszaru, na przykład do warstwy DIV:

```
<div role="main">
...
</div>

```

Od tego momentu pojedynczy skrót klawiaturowy może zaprowadzić użytkownika dokładnie do miejsca, w którym znajduje się główna treść dokumentu.

## Rodzaje landmarków

Specyfikacja ARIA przewiduje następujące typy landmarków:

1. Application.
2. Banner.
3. Complementary.
4. Contentinfo.
5. Form.
6. Main.
7. Navigation.
8. Search.

Tych osiem landmarków wystarcza dla prawidłowego określenia ról poszczególnych obszarów strony internetowej. Ważne jest, by stosować je w sposób logiczny i zgodny z przeznaczeniem.

## Nagłówek i stopka

Dwoma stałymi elementami stron internetowych są nagłówki i stopki. Nagłówki to zazwyczaj banner z nazwą serwisu, logo, motto, nazwa właściciela i podobne stałe informacje zamieszczane na początku dokumentu. Taki obszar powinien mieć przypisany landmark “banner”. Z kolei w stopce umieszcza się zazwyczaj informacje o prawach autorskich, warunkach używania, polityce dostępności i prywatności. Ten obszar powinien mieć przypisany landmark “contentinfo”. Obu landmarków można użyć tylko raz na danej stronie.

## Główna treść

Element najistotniejszy na stronie powinien mieć przypisany landmark “main”, a na początku mieć także nagłówek z tytułem przypisanym do treści, na przykład tak:

```
<div role="main">
<h2>artykuł o landmarkach</h2>
...
treść artykułu
...
</div>

```

Podobnie jak “banner” i “contentinfo” – także landmark “main” może na stronie wystąpić tylko raz. W obrębie tego obszaru nie powinny znajdować się inne obszary, na przykład nawigacyjne lub do wyszukiwania.

## Nawigacja i wyszukiwanie

Linkinawigacyjne i menu powinny mieć przydzielony landmark “navigation”, który może pojawić się na stronie więcej niż jeden raz. Zazwyczaj menu występują na stronie dwa, trzy lub więcej razy i każdy powinien być otoczony warstwą z landmarkiem “navigation”. Jeżeli menu jest przygotowane w formie listy punktowanej, to landmark można przypisać do znacznika otwierającego listę:

```
<ul role="navigation">
...
</ul>

```

Jednak zgodnie z innymi zaleceniami takie menu powinno zostać poprzedzone nagłówkiem i wtedy taka technika już nie może zostać użyta. Wtedy trzeba to zrobić następująco:

```
<div role="navigation">
<h2>Menu główne</h2>
<ul>
...
</ul>

```

W analogiczny sposób należy podejść do wyszukiwarki umieszczonej na stronie internetowej, której należy przypisać landmark “search”. Można to zrobić na przykład tak:

```
<form role="search">
<label><input type="text" id="search"></label>
<input type="submit" value="szukaj" id="pushsearch">
</form>

```

## Formularze i aplikacje

Jeżeli na stronie pojawi się formularz lub jego elementy, to należy je oznaczyć landmarkiem “form”. W prawidłowo skonstruowanym dokumencie przyjmie to nieco redundantną postać:

```
<form role="form">
...
</form>

```

Jednak bywa, że programiści zapominają o stosowaniu niektórych znaczników i wtedy można sytuację uratować przez taki landmark. Jest on zresztą przeznaczony do formularzy bardziej tradycyjnych, ale już nie do tych, które są interfejsem do aplikacji webowej.

Dla takich aplikacji przeznaczony jest specjalny landmark “application”, który pozwala na łatwe odnalezienie interfejsów różnych aplikacji. Mogą nimi być różnego rodzaju edytory, chaty, mapy i podobne elementy. Nawet jeżeli wykorzystują one kontrolki formularzy, to jednak trudno je do formularzy zaliczyć.

## Pozostałe elementy

Jeżeli jakiś fragment strony nie nadaje się do zaliczenia do siedmiu powyższych kategorii, to mamy do dyspozycji ten ósmy – “complementary”. Można w nim zawrzeć reklamy, slajdy ze zdjęciami, widgety pogody, imienin i podobne. Generalnie wszystko, co nie pasuje do tych precyzyjniej opisanych. Ważną rzeczą jest bowiem, by żadna treść nie pozostała osierocona i każdy obrazek i każda litera zostały ujęte w landmarki. Nawiasem mówiąc – skórka używana przeze mnie ma błędnie zadeklarowane landmarki, czym zajmę się wkrótce.