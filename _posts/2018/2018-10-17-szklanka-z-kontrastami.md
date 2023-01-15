---
id: 1870
title: 'Szklanka z kontrastami'
date: '2018-10-17T09:27:01+02:00'
layout: post
guid: 'http://informaton.pl/?p=1870'
permalink: /2018/10/17/szklanka-z-kontrastami/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - kolor
    - kontrast
    - tekst
    - 'WCAG 2.0'
---

We wrześniu brałem udział w spotkaniu dla projektantów stron internetowych w Krakowie, które organizowała firma Making Waves. Jak to zwykle bywa – z sali posypały się pytania, a w tym to, z którym spotykam się co jakiś czas. Streścić zaś je można do *Czy musimy rezygnować z własnej wizji kolorystycznej dla spełnienia potrzeb wąskiej grupy odbiorców?* Chodzi zaś o to, że nie zawsze zestaw kolorów opisujący tło i tekst mają odpowiedni kontrast.

### Czym jest odpowiedni kontrast

Standard WCAG zaleca, by podstawowy kontrast wynosił 4,5:1, a dla dużego tekstu może być nieco mniejszy i wynosić 3:1. Jeżeli zaś sięgnąć do poziomu AAA, to kontrasty powinny być większe i wynosić odpowiednio 7:1 oraz 4,5:1. Są to oczywiście wartości minimalne i mogą być wyższe, ale jednak ogranicza to projektantów w doborze kolorystyki. I znowu przypomniało mi się męczące mnie pytanie – jak bardzo ogranicza to w praktyce?

Pytanie wcale nie jest trywialne. Na stronach WAI podany jest [wzór do wyliczania kontrastu](https://www.w3.org/WAI/GL/2006/07/mathml-exp/luminosity-contrast-ratio.xml) i wymyśliłem, że trzeba go po prostu przeliczyć dla wszystkich par kolorów, a potem sprawdzić, ile z nich spełnia wymagania odpowiedniego kontrastu. Wymyślić było łatwo, ale ze mnie programista jak z koziej dupy trąba, więc się poddałem i wezwałem na pomoc mistrza programowania, czyli [Grzegorza Złotowicza](http://www.zlotowicz.pl). Najpierw marudził, że wzoru nie może znaleźć i że do obliczenia tylu par czasu wszechświata nie starczy, ale potem się uzgodniliśmy. Wzór mu przesłałem, a co do liczby par zdecydowaliśmy się na uproszczenie i badanie czterobitowe na składową kolorów zamiast ośmiobitowego. No i skrypt powstał, a wyniki trochę mnie zaskoczyły.

### Szklanka z kolorami po części pusta

Intuicyjnie podejrzewałem, że obawy programistów są bezpodstawne i ograniczenia są mniejsze od spodziewanych. Tymczasem wcale nie jest aż tak dobrze. W skrypcie policzono 16777216 par kolorów. z nich 12103062 nie spełnia wymagań kontrastu nawet dla dużego tekstu. Oznacza to, że aż 72% par należy odrzucić całkowicie, jako nieprzydatne.

Dla dużego tekstu pasującychzestawów było 2473522. Z kolei chcąc spełnić wymagania podwyższonego kontrastu zastosować można jeden z 716424 zestawów. Można zatem rzec, że szklanka jest w 28% pełna, co wygląda gorzej, niż mi się zdawało, ale wcale nie tak źle.

Na moje marudzenie, że jednak jest dosyć marnie, Grzegorz napisał mi, żebym się opanował, bo przecież nie każdy zestaw nadaje się tak samo do użytku. Może to zatem oznaczać, że w praktyce proporcje są nieco inne i to na korzyść tych kontrastowych. Po przemyśleniu nie przyznam mu racji, bo primo – tak samo może być w tych obszarach o odpowiednim kontraście i secundo – nie ma jak tego oszacować. Chodzi też za mną pytanie, czy nasze uproszczenie kolorystyczne, czyli opisanie kolorów na 12, a nie 24 bitach nie zaważyło jakoś na wynikach.

Nie zmienia to faktu, że akurat dobry kontrast jest przydatny dla absolutnie każdego użytkownika i warto z niego korzystać. Protesty wizjonerów projektantów zawsze mogę skwitować, że strona internetowa to nie obrazek do powieszenia na ścianie i musi być przede wszystkim czytelna, a efektowna w drugiej kolejności. Tak więc zachęcam do sięgania po te 28% zestawów kolorów, które czytelność zapewnią.