---
id: 1096
title: 'Jak sobie poradzić z dostępnością sliderów i karuzel?'
date: '2014-08-09T10:44:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=1096'
permalink: /2014/08/09/jak-sobie-poradzic-z-dostepnoscia-sliderw-i-karuzel/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - czas
    - karuzela
    - klawiatura
    - slider
---

Popularnym elementem graficznym na stronach internetowych są zmieniające się automatycznie informacje, na przykład fotografie lub reklamy. Problem w tym, że najczęściej naruszają ważne [kryterium sukcesu 2.2.2 WCAG 2.0.](http://informaton.pl/?p=208) Rozwiązanie jest zazwyczaj bardzo proste, chociaż rzadko stosowane: należy dodać przyciski sterujące jak w odtwarzaczu multimedialnym – wstrzymaj, odtwarzaj, wstecz i do przodu. Ostatnio fajne rozwiązanie Wykorzystujące [ARIA](http://www.w3.org/TR/wai-aria/) zademonstrowano na [tej stronie.](http://www.romaingervois.fr/implementations/en/carousel.html). Zmiany można zatrzymać i sterować nimi, na przykład wyświetlając dowolny element. Autor wykorzystał zakładki ARIA (ang. <span lang="en">tabs</span>), po których można się przemieszczać za pomocą klawiatury. Zmiany można też wstrzymać za pomocą przycisku <span lang="en">Pause the carousel below</span>, który zmienia się w przycisk <span lang="en">Play the carousel below</span>. Naprawdę fajne i warte powielania.