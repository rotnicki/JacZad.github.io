---
id: 153
title: 'Podwyższony kontrast (WCAG 2.0 SC 1.4.6, poziom AAA)'
date: '2012-08-20T10:03:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=153'
permalink: /2012/08/20/podwyzszony-kontrast-wcag-2-0-sc-1-4-6-poziom-aaa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - czcionki
    - dokumenty
    - grafika
    - kolor
    - kontrast
    - tekst
---

Odpowiedni kontrast pomiędzy tekstem a tłem ogromnie ułatwia, a niektórym wręcz umożliwia odczytanie informacji. Warto zatem, by taki kontrast był zachowany przy przygotowywaniu treści w Internecie. Dla spełnienia wymogu odpowiedniego kontrastu na poziomie AA wystarczy stosowanie [SC 1.4.3](http://informaton.pl/?p=129), ale dla spełnienia poziomu AAA trzeba ten kontrast podwyższyć.

Kryterium sukcesu 1.4.6 określa minimalny kontrast pomiędzy kolorem tekstu a tłem na 7:1, przy czym dotyczy to zarówno tekstu tworzonego w sposób jawny, jak i tego umieszczanego w grafikach. Wyjątek uczyniono dla logotypów i oznaczeń firmowych (ale nie dla całej tożsamości graficznej) oraz dla informacji nieistotnej (na przykład przypadkowych tekstów na fotografiach). Dla tekstów pisanych powiększoną czcionką kontrast może być mniejszy i powinien wynosić przynajmniej 4,5:1. Skorzystają z tego:

- użytkownicy słabowidzący,
- daltoniści,
- seniorzy,
- użytkownicy drukujący treści internetowe,
- użytkownicy małych i monochromatycznych wyświetlaczy.

Liczbowo podany kontrast niewiele mówi. Można jednak powiedzieć, że minimalny kontrast (biały na białym) wynosi 1:1, zaś maksymalny (czarny na białym) wynosi 21:1. W praktyce oznacza to stosunek składowych luminancji dwóch kolorów, wyliczanych na podstawie składowych RGB (red, green, blue). A tutaj można zobaczyć [wzór na obliczenie kontrastu](http://www.w3.org/WAI/GL/2006/07/mathml-exp/luminosity-contrast-ratio.xml). Wzór wyświetli się prawidłowo w przeglądarkach interpretujących MatHML, ale w innych także da się odczytać. jest to wzór dosyć skomplikowany, ale na szczęście nie trzeba się nim posługiwać bezpośrednio. Powstało sporo narzędzi obliczających kontrast, ułatwiających pracę webmasterom.