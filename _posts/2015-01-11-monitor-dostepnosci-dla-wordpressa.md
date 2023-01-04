---
id: 1220
title: 'Monitor dostępności dla WordPressa'
date: '2015-01-11T09:25:35+01:00'
layout: post
guid: 'http://informaton.pl/?p=1220'
permalink: /2015/01/11/monitor-dostepnosci-dla-wordpressa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - narzędzia
    - 'WCAG 2.0'
    - Wordpress
    - wtyczka
---

Niezrównany Joe Dolson znowu dodał do repozytorium wtyczek do WordPressa coś ciekawego. Jest to rozszerzenie, którego podstawowym zadaniem jest badanie serwisu internetowego opartego na WordPress. Nazywa się [Access Monitor](https://wordpress.org/plugins/access-monitor/)i wykorzystuje aplikację webową [Tenon.io](http://tenon.io/). Działanie jest bardzo proste i całkiem nieźle się sprawdza.

Instalacja wtyczki jest standardowa i nie nastręcza trudności. Potem jedynie trzeba oddać trochę swoich danych osobowych za API Key do Tenon.io, aby wpisać go w odpowiednie pole. Teraz przeglądając serwis i mając włączony panel administracyjny, można kliknąć na przycisk “A11Y Check”, by wtyczka sprawdziła stan danej strony serwisu i zapisała raport na liście. Tylko i aż tyle, a przy tym komunikaty mają sens, chociaż są tylko po angielsku. W raporcie można zobaczyć jaki błąd został popełniony, jaką ma wagę oraz wczytać się we fragment kodu. Całkiem zgrabnie to działa, chociaż zawiodłem się planowaniem testów. Miałem nadzieję na większą automatyzację procesu, a tu raczej ręczna robota z przeklejaniem adresów URL. To jednak jest dopiero pierwsza wersja tej wtyczki, więc może w przyszłości będzie lepiej. Po poprzednich [przejściach z Utilitią](http://informaton.pl/artykuly/tajemniczy-wskaznik-dostepnosci-utilitii-czyli-o-ograniczonym-zaufaniu-do-automatow/) i dzisiejszych wynikach z Access Monitora poprawiłem wreszcie dwa błędy, które byłem w stanie wyeliminować. Teraz czeka mnie polowanie na kolejne, znajdowane na różnych podstronach serwisu. Jak zwykle dodaję zastrzeżenie – automat za mnie nic nie załatwi i nie znajdzie wszystkich błędów. Jednak pomoc stanowi całkiem przyjemną. Polecam i proszę o więcej!