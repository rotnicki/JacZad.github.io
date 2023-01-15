---
id: 572
title: 'Dostępne okna dialogowe &#8211; wykorzystanie HTML 5 i ARIA'
date: '2013-02-02T21:13:30+01:00'
layout: post
guid: 'http://informaton.pl/?p=572'
permalink: /2013/02/02/dostepne-okna-dialogowe-wykorzystanie-html-5-i-aria/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - aplikacje
    - ARIA
    - formularze
    - 'HTML 5'
    - niewidomi
---

Dzisiaj mały przykład wykorzystania HTML 5 i ARIA (Accessible Rich Internet Aplications). Korzystając z kilku dodatkowych atrybutów można sprawić, by okienko dialogowe stało się w pełni dostępne dla programów odczytu ekranu.

Okna dialogowe i alertowe można w sposób bardzo prosty tworzyć za pomocą HTML 5. Jeżeli na takie okno natknie się czytnik ekranu używany przez niewidomego użytkownika, natychmiast przechodzi w tryb aplikacji i traktuje cały obszar jak okienko dialogowe aplikacji. Można się po nim poruszać za pomocą klawisza tabulacji, zaznaczać i odznaczać spacją i wpisywać tekst. Jednak niedostępny jest wówczas tryb przeglądania, który starałem się wyjaśnić w tekście o [testowaniu za pomocą czytnika ekranu](http://informaton.pl/?p=352). W takiej sytuacji użytkownik traci dostęp do wszystkich elementów, które nie mogą przechwycić fokusa sterowanego klawiaturą. Jest to ogromny problem spotykany na przykład na Facebooku i Google+. A rozwiązania są dostępne i wystarczy z nich korzystać.

## Struktura okna dialogowego

Ogólna budowa okna dialogowego jest prosta i składa się z zadeklarowanego obszaru z przydzieloną rolą “dialog”. Takiemu oknu trzeba koniecznie przydzielić nazwę, która jest odpowiednikiem paska tytułu okna. Wykorzystuje się do tego atrybut “aria-labelledby” odwołujący się do identyfikatora opisu. W poniższym przykładzie jest to tekst zawarty w nagłówku poziomu pierwszego.

```
<div aria-labelledby="wndtitle" role="dialog">
<h1 id="wndtitle">Dodaj użytkownika do kręgu</h1>
...
</div>

```

Od tego momentu program odczytu ekranu będzie anonsował tytuł okna za każdym razem, gdy wejdzie w jego obszar.

## Wkładamy kontrolki

W tak przygotowanym kontenerze możemy umieścić niezbędne kontrolki. W tym wypadku będą to trzy pola wyboru i przycisk. Dla uporządkowania umieszczamy je w liście punktowanej, chociaż można je dowolnie formatować. Nie zapominamy o etykietach. Mamy zatem następujący kod:

```
<div aria-labelledby="wndtitle" role="dialog">
<h1 id="wndtitle">Dodaj użytkownika do kręgu</h1>
<ul>
<li> rodzina</li>
<li> znajomi</li>
<li> pozostali</li>
<li></li>
</ul>
</div>

```

Okno jest już prawie gotowe, ale trzeba jeszcze dodać objaśnienie.

## Dodajemy objaśnienie

W najprostszy sposób można to zrobić umieszczając na początku okna, a za nagłówkiem tytułowym, krótki opis: Zaznacz kręgi, do których chcesz dodać użytkownika. Jednak taki akapit nie jest elementem aktywnym, a zatem nie jest w stanie przechwycić fokusa. Należałoby ten opis jakoś dowiązać do okna w taki sposób, by był anonsowany użytkownikowi. Możemy do tego wykorzystać grupowanie i legendę.

```
<div aria-labelledby="wndtitle" role="dialog">
<h1 id="wndtitle">Dodaj użytkownika do kręgu</h1>

Zaznacz kręgi, do których chcesz dodać użytkownika
<ul>
<li> rodzina</li>
<li> znajomi</li>
<li> pozostali</li>
<li></li>
</ul>

</div>

```

W specyfikacji ARIA jest jeszcze inne rozwiązanie, a mianowicie atrybut “aria-describedby”, ale tutaj jego użycie byłoby niezbyt efektywne. Wkrótce podam przykład, gdzie sprawdzi się o wiele lepiej.

## Podsumowanie

HTML 5 i ARIA dają bardzo wiele możliwości stworzenia dostępnych okienek. Wymaga to nieco staranności i wyobraźni, a na koniec przetestowania za pomocą czytnika ekranu. Najważniejsze jest, by każdy istotny element zawartości okna był anonsowany i to w sensownym powiązaniu z innymi elementami. Bardzo często zdarzają się okna, w których dostępne są kontrolki, ale nie da się dotrzeć do pozostałych informacji, na przykład treści komunikatu. Może być więc tak, że dostępne są tylko przyciski “tak” i “nie”, ale brakuje do nich pytania.