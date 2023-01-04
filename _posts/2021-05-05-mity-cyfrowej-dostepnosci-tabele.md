---
id: 2294
title: 'Mity cyfrowej dostępności &#8211; tabele'
date: '2021-05-05T16:31:14+02:00'
excerpt: 'Czy tabela może służyć do prezentacji układu graficznego strony internetowej? Moim zdaniem - tak!'
layout: post
guid: 'http://informaton.blog/?p=2294'
permalink: /2021/05/05/mity-cyfrowej-dostepnosci-tabele/
timeline_notification:
    - '1620225075'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - ARIA
    - Mity
    - tabele
    - wygląd
---

Jakoś ostatnio często mam potrzebę dekonstruowania cyfrowej dostępności i standardu WCAG. Wpływ na to ma wiele czynników, ale tym najważniejszym jest dla mnie powracająca wciąż fala mitów dotyczących cyfrowej dostępności. Ich źródeł czasem trudno dociec, chociaż dłuższe poszukiwania pozwalają domyślić się skąd pochodzą. Dzisiaj tabele, bo wypłynęły ostatnio dwukrotnie w różnych rozmowach.

Tabela w HTML to taka dwuwymiarowa struktura posiadająca wiersze i komórki. Ma niby też kolumny, ale zazwyczaj w kodzie nie są one obecne. Po prostu pierwsza komórka w pierwszym wierszu znajduje się nad pierwszą komórką w drugim wierszu. O ile ktoś nie namiesza w tej strukturze. Tabele mogą być rozbudowane także o podpis, wyjaśnienie, komórki nagłówkowe i wiele innych elementów opisujących jej strukturę. To jednak dzisiaj nie jest istotne.

## Do czego służy tabela?

Tabela służy do prezentowania danych tabelarycznych. Jesteśmy oswojeni z tabelami już od szkoły podstawowej i odruchowo wiemy, że komórka to jest to coś na przecięciu wiersza i kolumny. Wiele razy przygotowywałem w tabeli budżet jakiegoś projektu i była to informacja przejrzysta, chociaż sam budżet nigdy się nie sprawdzał. Dostępność danych w tabeli to przede wszystkim wytyczna 1.3, a w jej ramach kryterium sukcesu 1.3.1 – informacje i relacje. Chodzi bowiem o to, by wiedzieć, w którym wierszu i kolumnie znajduje się komórka.

Umieszczenie danych tabelarycznych w sposób wizualny, a nie semantyczny, jest jednym z największych grzechów dostępności. Coś wyglądającego na tabelę z danymi, ale nie będąca nią sprawia, że nie da się zorientować, jakich wartości dotyczą dane w tabeli. Nie wiadomo, w którym roku uprawa buraka cukrowego była największa i w którym województwie.

## Na czym polega problem?

Mamy zatem zasadę, że dane tabelaryczne umieszcza się w tabeli. Jednak dość często pojawia się interpretacja rozszerzająca, według której nie można tabeli stosować do niczego innego. Stąd zgłaszanie błędu podczas audytu, gdy układ strony oparty jest na tabeli. Tymczasem to nie jest żaden błąd dotyczący dostępności. Można powiedzieć, że jest to rozwiązanie przestarzałe i wątpliwe technicznie, ale na pewno nie łamie zasad cyfrowej dostępności.

Co więcej – takie rozwiązania zostały przewidziane w standardach. W ARIA jest taka rola, którą przypisuje się elementom, które pełnią wyłącznie funkcję prezentacyjną, a zatem na przykład tabeli. I technologie asystujące wiedzą, że mają tą tabelę zignorować, jak grafikę ornamentową.

## To używać, czy nie?

Raczej nie, bo wygląd powinno się oddzielać od warstwy informacyjnej. Poza tym można się narazić na pogardliwe prychanie ze strony innych webmajstrów, bo teraz przecież pozycjonuje się stylami. Jeżeli jednak jest to strona zastana, zrobiona kilka lub kilkanaście lat temu – nie ma co robić z tego tragedii. To nie ma wpływu na cyfrową dostępność.