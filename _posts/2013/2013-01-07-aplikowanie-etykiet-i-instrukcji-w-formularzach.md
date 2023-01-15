---
id: 480
title: 'Aplikowanie etykiet i instrukcji w formularzach'
date: '2013-01-07T12:51:12+01:00'
layout: post
guid: 'http://informaton.pl/?p=480'
permalink: /2013/01/07/aplikowanie-etykiet-i-instrukcji-w-formularzach/
restapi_import_id:
    - 5ca8405547793
geo_public:
    - '0'
amp_status:
    - enabled
categories:
    - artykuły
tags:
    - etykiety
    - formularze
    - 'HTML 5'
---

Formularze są trudnym i wymagającym elementem serwisów internetowych. Dlatego wiele z rozwiązań związanych z dostępnością dotyczy tego właśnie obszaru. WCAG 2.0 wymaga stosowania etykiet i instrukcji, więc specyfikacja HTML 5 wychodzi naprzeciw tym oczekiwaniom.

Kontrolki formularzy powinny zawierać w sobie dwa elementy informujące użytkownika: etykiety i instrukcje. Etykiety informują o tym, co należy wpisać, a instrukcje – jak należy to wpisać lub w inny sposób podpowiadają użytkownikowi, co ma z danym polem zrobić. Etykieta powinna być możliwie krótka, a instrukcja, chociaż zwięzła, to jednak na tyle precyzyjna, by była użyteczna. Poniżej przykład kodu:

```
<form>
<label for="szukaj">Szukaj: </label>
<input type="search" name="szukaj" placeholder="tutaj wpisz tekst, który chcesz wyszukać">
<input type="submit" placeholder="kliknij, aby wysłać zapytanie" value="Szukaj">
</form>

```

&gt;W formularzu wykorzystany został znacznik “label”, który zawiera w sobie etykietę dla konkretnej kontrolki. Powiązanie odbywa się za pomocą atrybutu “for”, którego wartością jest identyfikator kontrolki, w tym wypadku “szukaj”. Etykieta w formularzu jest w ten sposób nierozerwalnie związana z kontrolką i wcale nie muszą występować w kodzie obok siebie.

&gt;W przykładzie użyty został nowy typ kontrolki formularza wprowadzony w HTML 5 – “search”. Jest to wyspecjalizowane pole edycyjne, w którym należy wpisywać hasła do wyszukiwania. Jeżeli przeglądarka nie obsługuje takiego typu pól, to wyrenderuje je jako zwykłe pole tekstowe.

&gt;Nowością jest atrybut “placeholder” wprowadzony także w HTML 5. Jego wartością jest ciąg znaków będący podpowiedzią dla użytkownika. Spełnia zatem zadanie, jakie ma być realizowane przez instrukcje. Nie wszystkie przeglądarki odpowiednio interpretują ten atrybut, ale warto go już stosować, bo stał się elementem specyfikacji nowego HTMLa.

&gt;Mamy też przycisk do wysyłania zapytania typu “submit”. W jego wypadku etykietowanie nie jest potrzebne, bo za etykietę służy wartość atrybutu “value”. Gdyby jednak na przycisk został nałożony obrazek, to należałoby go zaetykietować.

&gt;Bardzo ważne jest, by nie stosować wymiennie znacznika “label” i atrybutu “placeholder”. Ich role są różne i trzeba je stosować zgodnie z przeznaczeniem. Pojawienie się “placeholder” wcale nie wypchnie z użytku “label”, jak piszą niektórzy webmasterzy. A przynajmniej tak nie powinno się stać.