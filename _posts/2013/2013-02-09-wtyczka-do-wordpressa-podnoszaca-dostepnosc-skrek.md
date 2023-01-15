---
id: 588
title: 'Wtyczka do WordPressa podnosząca dostępność skórek'
date: '2013-02-09T11:38:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=588'
permalink: /2013/02/09/wtyczka-do-wordpressa-podnoszaca-dostepnosc-skrek/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - fokus
    - klawiatura
    - nawigacja
    - Wordpress
---

Właśnie została zaktualizowana [wtyczka WP Accessibility do wersji 1.2.](http://www.joedolson.com/articles/2013/02/wp-accessibility-version-1-2-0-now-available/)Jest to bardzo ciekawe rozwiązanie dla administratorów, stron postawionych na WordPress, którzy chcą zrobić coś w kierunku dostępności, a jeszcze nie zebrali się za gruntowne porządki. Od razu jednak ostrzegam – ta wtyczka nie rozwiązuje problemów za webmastera, a jedynie usuwa kilka problemów.

Wtyczka działa doskonale z moją skórką, ale zakładam, że tak bedzie także z innymi Poniżej krótki przegląd możliwości.

## Usuwanie zbędnych atrybutów

Wtyczkę można skonfigurować w taki sposób, by usuwała niektóre zbędne atrybuty, na przykład TITLE z różnych elementów interfejsu oraz z grafik osadzonych na stronie. Może też likwidować atrybuty TARGET, aby linki nie powodowały otwierania nowych kart lub okien w przeglądarce. Może wreszcie usuwać atrybut TABINDEX z elementów interfejsu, które i tak przechwytują fokus, a zatem atrybut ten może zaburzać kolejność nawigacji.

## Dodanie skiplinków

Wtyczka pozwala na dodanie skiplinków, czyli wewnętrznych łączy pozwalających na szybkie przeniesienie fokusa do głównej treści lub menu nawigacyjnego. Wystarczy tylko podać identyfikator elementu, do którego ma prowadzić skiplink i reszta odbywa się automagicznie.

## Regulacja powiększenia i kolorystyki

W tej wersji autor zdecydował się na dodanie narzędzia dostosowującego sposób wyświetlania strony. Są tam standardowe narzędzia pozwalające na powiększenie i pomniejszenie czcionek oraz zmianę kolorystyki strony. Ciekawostką jest możliwość przełączenia strony w tryb odcieni szarości, co jednak nie działa w przeglądarce Firefox.

## Rozszerzanie linków

Ta opcja jest już włączona w moim serwisie, a pozwala ona na dodanie tytułu artykułu do tekstu rozwijającego. Na przykład zamiast standardowego “czytaj dalej” można mieć “czytaj dalej:Wtyczka do WordPressa podnosząca dostępność skórek. Do tej pory – wedle mojej wiedzy – żadna skórka nie oferowała tego typu funkcjonalności. W ten sposób powstają linki, które są zrozumiałe poza kontekstem.

## Obrys dla fokusa

Dla osób posługujących się klawiaturą kluczowe jest, by wiedzieć, gdzie znajduje się fokus. Wiele skórek – ze względów estetycznych – wyłącza domyślne obrysowanie elementów interfejsu. WP Accessibility pozwala na ponowne aktywowanie widoczności obrysu oraz dobranie odpowiedniego koloru.

Wtyczka ma jeszcze kilka drobiazgów, na przykład kalkulator kontrastu. Warto jednak pamiętać, że nie zapewni ona dostępności w zupełnie źle zbudowanym serwisie. Może jednak zapoczątkować proces lub udoskonalić skórkę, która jest w miarę dobra. Poza tym jest w niej potencjał do dalszej pracy, czego autorowi gorąco życzę. Wtyczka jest dostępna z poziomu zarządzania wtyczkami w panelu administracyjnym WordPressa.