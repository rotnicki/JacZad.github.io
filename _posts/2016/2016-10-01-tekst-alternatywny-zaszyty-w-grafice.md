    ---
title: 'Tekst alternatywny zaszyty w grafice'
date: '2016-10-01T19:06:52+02:00'
layout: post
categories:
    - artykuły
tags: ['GIF', grafika, PNG, JPEG]
---

Wczoraj zastanawiałem się nad digitalizacją zasobów kultury i problemów technicznych z tym związanych. Zadałem sobie też pytanie, czy tekst alternatywny można na stałe przywiązać do pliku graficznego. Chodzi o to, by po wyjęciu go ze strony internetowej, dokumentu lub mając go luzem na dysku mieć opis alternatywny zawsze do wykorzystania. Poniżej efekty moich poszukiwań.

Moje zainteresowanie skierowałem na trzy najpopularniejsze formaty graficzne: PNG, GIF i JPEG. Dwa pierwsze są formatami bezstratnymi, chociaż GIF pozwala na użycie niewielkiej palety kolorów. JPEG jest formatem stratnym, ale za to bardzo popularnym. Wszystkie trzy są obsługiwane przez przeglądarki internetowe bez potrzeby instalowania rozszerzeń, co wydaje się bardzo istotne.

W [specyfikacji formatu PNG](https://www.w3.org/TR/PNG/) znalazłem chyba odpowiednie miejsce. Format przewiduje przechowywanie danych tekstowych, w tym także takich zdefiniowanych jako <span lang="EN">“Description”</span>. Z opisu wynika, że można tam umieścić opis, w tym długi. Tekst zaś można przechowywać w jednym z trzech standardów, z których tylko jeden (iTXt) nadaje się do naszych potrzeb, ponieważ obsługuje polskie znaki w standardzie Unicode. Pozostałe obsługują tylko standard Latin-1.

Wydaje się, że gorsza sytuacja ma miejsce w wypadku formatu GIF, nawet nowszej jego wersji – GIF89a. Dodano w nim dwa rozszerzenia tekstowe: plain-text i comment. Niestety – ten pierwszy służy do wyświetlania tekstu na grafice, a zatem nie nadaje się do przechowywania tekstu alternatywnego. Od biedy można byłoby użyć komentarzy, ale nie da się tam stosować polskich znaków. Znaki są kodowane na 7 bitach, więc wchodzą w grę tylko litery podstawowego alfabetu łacińskiego. Czytając informacje o formacie GIF odkryłem ze zdziwieniem, że ma on już niemal 30 lat!

Po dłuższym studiowaniu informacji o formacie JPEG stwierdziłem, że sytuacja jest podobna do opisanej w wypadku GIF. Tekst alternatywny można upchnąć w sekcji komentarza i tyle. Projektanci nie przewidzieli specjalnej sekcji dla opisu grafiki, jak to ma miejsce w wypadku PNG.

Poszukiwania dały mi jeszcze jedną podpowiedź, a mianowicie możliwość wykorzystania zewnętrznych metainformacji. Na przykład dane [IPTC](https://iptc.org/) pozwalają na dodanie całkiem wielu informacji kontekstowych. Standard został opracowany głównie na potrzeby ochrony praw autorskich i licencjonowania, ale spokojnie nadaje się do wykorzystania. Sprawdziłem w darmowym programie IrfanView i on obsługuje ten standard, więc pewnie jest dosyć rozpowszechniony. Na stronie standardu wymieniono kilka popularnych aplikacji, w tym od Adobe. Można zatem przyjąć, że jest to standard jakoś uznany.

A jak to dalej wykorzystać? Wyobrażam sobie, że osoby digitalizujące obrazy (fotografie, grafiki, malarstwo itp.) opracowują teksty alternatywne i umieszczają je w plikach graficznych w jeden z wyżej wymienionych sposobów. Portal służący do publikowania tych treści ma wbudowany skrypt wyciągający ten tekst i umieszczający go w atrybucie ALT oraz wykorzystujący go na inne sposoby. Wydaje się też, że takie pliki powinny być odpowiednio oznaczane jako dostępne, ale o tym może za kilka dni.
