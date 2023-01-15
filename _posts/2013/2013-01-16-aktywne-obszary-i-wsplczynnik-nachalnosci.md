---
id: 499
title: 'Aktywne obszary i współczynnik nachalności'
date: '2013-01-16T09:36:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=499'
permalink: /2013/01/16/aktywne-obszary-i-wsplczynnik-nachalnosci/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - niewidomi
    - semantyka
    - sklep
---

Niewidomi i słabowidzący użytkownicy serwisów internetowych mają ograniczony dostęp do całości wyświetlanych informacji. Niekiedy istotne jest, by pewien obszar był wyróżniony i w sposób automatyczny zwracał użytkownikowi uwagę na siebie. W tym celu w specyfikacji ARIA powstały aktywne obszary. Można je stosować w HTML i XHTML, chociaż najlepiej sprawdzą się w HTML 5.

## Aktywny obszar

W sklepie internetowym mamy koszyk, w którym dosyć kluczową informacją jest jego wartość. Dodając towary do koszyka sprawiamy, że ta wartość się zmienia, o czym klient jest informowany na bieżąco. Jednak klient niewidomy odczytuje w tym momencie zupełnie inny fragment strony i nie ma świadomości takiej zmiany. Można mu jednak zwrócić na to uwagę przez użycie aktywnego regionu, w którym umieścimy wartość koszyka.

```
<div>
W koszyku są towary o wartości 219 złotych
</div>

```

W powyższym przykładzie wartość koszyka jest umieszczona w aktywnym obszarze, ale nie będzie on anonsowany, ponieważ jego wartość jest ustawiona na “off”. Możliwe są jednak dwie inne wartości, które nazwałem współczynnikiem nachalności.

## Współczynnik nachalności.

Mamy zatem trzy możliwe wartości dla aktywnego obszaru

1. “off” – oznaczający brak anonsowania zmian.
2. “polite” jest współczynnikiem małej nachalności, a przeglądarka czeka z przekazaniem informacji na użytkownika, na przykład aż przestanie pisać.
3. “assertive” oznacza najbardziej nachalny poziom, w którym informacja jest przekazywana użytkownikowi natychmiast, gdy dokona się zmiana.

Wartość “off” oznacza w praktyce wyłączenie aktywnego obszaru, a każda z pozostałych – włączenie. Wartości “assertive” należy używać wyłącznie w sytuacjach, gdy jest to niezbędne, ponieważ może zakłócać korzystanie z serwisu przez nadmierne gadulstwo. Najlepiej jest stosować wartość “polite”, która dostosowuje się do aktywności użytkownika. A zatem kod w wypadku koszyka powinien wyglądać następująco:

```
<div>
W koszyku są towary o wartości 219 złotych
</div>

```

## Kawałki informacji

Gadulstwo można dodatkowo wyregulować stosując dodatkowy atrybut aria-atomic. Jest on opcjonalny i ma tylko dwie możliwe wartości: domyślną “false” i “true”. Ten atrybut decyduje o tym, czy komunikat ma być oznajmiany w postaci całej treści aktywnego obszaru, czy może ma oznajmiać tylko treść, która się zmienia. Odpowiedź na pytanie, którą wartość wybrać, wcale nie jest trywialna. Z jednej strony komunikat “W koszyku są towary o wartości 219 złotych” jest dosyć długi i może irytować, ale wybierając wartość atrybutu na “false” ryzykujemy utratę informacji, bo dodając do koszyka coś o wartości 20 złotych zmienimy jego wartość na 239, co zostanie zaanonsowane jako… “3”, bo tylko ta cyfra zmieni się w całym ciągu tekstowym. Dlatego bezpieczniej jest stosować w tym wypadku wartość “true”, która spowoduje odczytanie całego obszaru.

```
<div>
W koszyku są towary o wartości 219 złotych
</div>

```

## Role dla obszarów

Do aktywnych obszarów można podejść nieco inaczej, przypisując im pewne zdefiniowane role. Role są podobne do występujących w interfejsach użytkownika w aplikacjach i mają predefiniowane pewne zachowania. Spójrzmy zatem na dostępne role i dopasujmy którąś do naszego koszyka.

1. “alert” – oznacza informację, którą użytkownik powinien otrzymać natychmiast. Komunikat o błędzie lub innej sytuacji nadzwyczajnej, na przykład zagrożeniu. Dla tej roli atrybut aria-live jest oczywiście ustawiony na “assertive”.
2. “status” – rola dla informacji, do której użytkownik powinien mieć w miarę swobodny dostęp, chociaż niezbyt nachalnie powinna się objawiać.
3. “timer” – obszar dla zegara odmierzającego czas od początku operacji lub do jej końca.
4. “marquee” – rola dla informacji uciekającej, na przykład paska informacyjnego, która nie jest kluczowa dla użytkownika.
5. “log” – rola dla informacji, która pojawia się przyrostowo, na przykład w chacie lub w logu aplikacji.

Wydaje się, że dla naszego koszyka najlepiej będzie się nadawać rola “status” – niezbyt nachalna, ale jednak anonsująca informacje. Zatem możemy użyć następującego kodu:

```
<div role="status">
W koszyku są towary o wartości 219 złotych
</div>

```