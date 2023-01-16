---
title: 'Virtualo &#8211; księgarnia, która nie chce mi sprzedawać książek'
date: '2019-02-08T15:42:16+01:00'
layout: post
categories:
    - artykuły
tags:
    - ARIA
    - ebooki
    - EPUB
    - Mobi
    - pieniądze
    - sklepy
    - Virtualo
---

Virtualo to chyba największa w Polsce księgarnia z książkami elektronicznymi. Ogromny wybór i częste oraz atrakcyjne promocje, z których kiedyś korzystałem. Dzisiaj też wpadła promocja na książkę Terry’ego Pratchetta. Jednak nie skorzystałem. Virtualo nie chce, abym kupował u nich książki, co osobiście uważam za afront. Ta niechęć nie jest skierowana bezpośrednio do mnie, ale do wszystkich niewidomych klientów.

Serwisy internetowe są dostępne w różnym stopniu. Księgarnie internetowe też są pod tym kątem różnorodne. Jednakże z Virtualo jest tak, że następuje tam ciągły regres i to pomimo informowania o tym przez klientów, w tym przeze mnie. Kiedyś książki można było pobierać, chociaż było to niewygodne. Potem można to było zrobić w systemie Windows na przeglądarce Firefox, o ile się wiedziało, jak to zrobić. Na Safari nie dało się tego zrobić ani pod MacOS ani iOS. Problemów było znacznie więcej, a pokazałem je podczas prezentacji w Krakowie.

<div class="jetpack-video-wrapper"><div class="suki-oembed suki-oembed-video" style="padding-top: 56.228%;"><iframe allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" frameborder="0" height="641" loading="lazy" src="https://www.youtube.com/embed/7eg3pJMuzYc?feature=oembed" title="Internetowe sklepy tracą klientów, bo nie da się z nich korzystać — Jacek Zadrożny / Wiedza Babel #2" width="1140"></iframe></div></div>Pod koniec stycznia dowiedziałem się, że Virtualo zadbało, by już żadna sztuczka nie pomogła. Okno modalne do pobierania ebooków zostało ukryte przed czytnikami ekranu za pomocą atrybutu aria-hidden=„true” i od tego momentu stało się niewidzialne. Niewidomi klienci zaczęli pisać do Virtualo i ja oczywiście także. Nie był to mój pierwszy kontakt z obsługą klienta tej firmy. Kilka lat temu wysłali mi ebooki na adres email. Jednak teraz zrobili inaczej i jedyne, co mieli do zaoferowania, to zwrot pieniędzy. Nie wiem, czy zwrot miałby dotyczyć wszystkich książek, bo przecież do żadnej nie mam dostępu, czy tylko do ostatniego zamówienia. Na razie nie skorzystałem. Jednak historia się jeszcze nie kończy, bo pojawił się niewidomy hacker – Sylwek Piekarski. Na liście osób niewidomych opublikował tutorial, w jaki sposób można pobrać ebooki z Virtualo. Za jego zgodą, przeklejam go poniżej, z zachowaniem oryginalnej pisowni.

> Najpierw musimy zalogować się do systemu i otworzyć swoją bibliotekę. Następnie w bibliotece wyświetlamy stronę, na której znajduje się książka, którą chcemy pobrać.
> 
> Bezpośredni link do materiału wygląda tak:
> 
> https://virtualo.pl/virtualodownload.php?product=1″id produktu”&amp;file=&amp;download=1
> 
> Gdzie w miejsce napisu “id produktu” musimy wstawić numer pliku, który chcemy pobrać. Po takiej operacji przykładowy link może wyglądać tak:
> 
> https://virtualo.pl/virtualodownload.php?product=2930976&amp;file=&amp;download=1
> 
> Powyższe linki wskazują na plik w formacie epub. Jeżeli ten sam plik będziemy chcieli pobrać w mobi to link musi wyglądać tak:
> 
> https://virtualo.pl/virtualodownload.php?product=2930976&amp;file=&amp;download=1&amp;format=mobi
> 
> Jak znaleźć id pliku
> 
> Po wyświetleniu w bibliotece strony, na której znajduje się książka, którą chcemy pobrać, otwieramy jej źródło. W większości przeglądarek zrobimy to naciskając ctrl+u.
> 
> Następnie w źródle szukamy ciągu znaków data-title=” z tytułem książki. Nie musimy wpisywać pełnego tytułu możemy podać pierwsze dwa słowa jak w przykładzie:
> 
> data-title=”Pytanie o
> 
> Pod tym tekstem w kolejnej linii znajdziemy następujący wpis
> 
> /virtualodownload.php?product=”id produktu”&amp;amp;file=&amp;amp;download=1
> 
> Gdzie w miejscu wpisu “id produktu” będzie numer naszego pliku. Przykładowy wpis może wyglądać następująco:
> 
> /virtualodownload.php?product=185643&amp;amp;file=&amp;amp;download=1
> 
> Zaznaczamy te cyferki i wstawiamy je do naszego linku otrzymując np. coś takiego:
> 
> https://virtualo.pl/virtualodownload.php?product=185643&amp;file=&amp;download=1
> 
> to co powyżej, to bezpośredni link do naszego pliku w formacie epub.
> 
> A tak będzie wyglądał link do pliku w formacie mobi:
> 
> https://virtualo.pl/virtualodownload.php?product=185643&amp;file=&amp;download=1&amp;format=mobi
> 
> Kopiujemy powyższy link do schowka, w przeglądarce otwieramy nową kartę i w pole adresowe wklejamy link. Po naciśnięciu entera Zostanie wyświetlone okno pobierania pliku. Jeżeli zostaniemy wylogowani, to musimy się ponownie zalogować. Osobiście sprawdziłem kilka razy i działa. Mam nadzieję, że u was też zadziała. Dajcie znać, czy sposób jest skuteczny.

Nie sprawdziłem skuteczności, bo i tak wkładam zbyt dużo czasu w kupowanie tam książek, by poświęcać go jeszcze więcej na hackowanie systemu. Sylwek się martwił, że opublikowanie tego tutoriala sprawi, że Virtualo odetnie nas od tego **prostego** sposobu. A dla mnie to będzie test, czy Virtualo ma zamiar walczyć z klientami, czy ich obsługiwać. Dla jasności – strona mobilna i aplikacja na iOS też są niedostępne.

Zdecydowałem się opisać tą sytuację, bo firma nie reaguje na informacje zwrotne od klientów. Psuje i tak bardzo kiepski serwis, nie przejmując się tym, że komuś tam nie uda się pobrać książek. Dlatego przestałem kupować książki w Virtualo, skoro mam dostatecznie poręczne Publio, Nexto, Ebookpoint lub Woblink. Sayonara Virtualo!