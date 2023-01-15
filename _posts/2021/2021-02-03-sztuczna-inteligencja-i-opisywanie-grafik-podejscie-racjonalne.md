---
id: 2077
title: 'Sztuczna inteligencja i opisywanie grafik &#8211; podejście racjonalne'
date: '2021-02-03T10:20:35+01:00'
layout: post
guid: 'http://informaton.blog/?p=2077'
permalink: /2021/02/03/sztuczna-inteligencja-i-opisywanie-grafik-podejscie-racjonalne/
timeline_notification:
    - '1612344038'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - badania
    - diagramy
    - infografiki
    - NCBR
    - Sages
    - 'sztuczna inteligencja'
    - tabele
    - 'tekst alternatywny'
    - wykresy
---

Narodowe Centrum Badań i Rozwoju przyznało dotację na [projekt badawczy](https://www.sages.pl/blog/3-i-pol-mln-zlotych-dla-spolki-sages-od-ncbr-na-oprogramowanie-dla-osob-z-niepelnosprawnosciami), w którego ramach mają powstać narzędzia do automatycznego przetwarzania obrazów na język naturalny. Mam sceptyczny stosunek do pomysłów tego typu, czemu dawałem wyraz kilkukrotnie. Tu jednak podejście jest nieco inne i obdarzam ten projekt kredytem zaufania.

Prace nad automatycznym tworzeniem alternatyw tekstowych na podstawie grafik nie są czymś nowym. Robi to Facebook, Google, Apple, Microsoft i pewnie wiele innych firm. Tylko że oni idą w kierunku, który jeszcze długo nie przyniesie zadowalających efektów. Próbują bowiem analizować dowolne grafiki, w tym zdjęcia, memy i podobne obrazy, w których bardzo istotny jest kontekst. Nie wystarczy wykryć, że na zdjęciu są dwie osoby, bo może to być równie dobrze bójka pod barem, scena seksu, jak i uroczyste podpisywanie umowy. Do tego te algorytmy bardzo często się mylą, co ogranicza zaufanie do nich.

W tym projekcie – o ile dobrze zrozumiałem cele – podejście jest inne. Analizowane mają być obrazy mające konkretną strukturę, na przykład wykresy, diagramy, infografiki. Będzie to zatem raczej rodzaj odwrócenia procesu zamiany danych na obraz, a nie próba zgadywania zawartości. I to podejście może się sprawdzić.

Automatyczne rozpoznawanie obrazu doskonale sprawdza się na razie w jednym obszarze: optycznym rozpoznawaniu znaków (OCR). Zestaw symboli do rozpoznania jest bowiem ograniczony i znane są wzorce. Trzeba zatem jedynie wyodrębnić taki znak, porównać go z wzorcami i zdecydować, czy prawdopodobieństwo poprawnego rozpoznania jest wystarczająco duże. Niby to proste, a dopiero od niedawna programy OCR stały się tak bardzo niezawodne. Jeszcze kilkanaście lat temu mój program OCR konsekwentnie rozpoznawał słowo “ból” jako “661”. Teraz takie rzeczy się właściwie nie zdarzają.

Wydaje się, że dla zaproponowanych obiektów, czyli tabel, wykresów, diagramów, infografik – automatyzacja jest możliwa do osiągnięcia. Są to obiekty bardziej skomplikowane i zróżnicowane, a za to kontekst sytuacyjny, kulturowy raczej nie występują. Może zatem osiągnięcie pożądanego efektu będzie możliwe.

Mam też nadzieję, że efektem ubocznym projektu będzie także instrukcja tworzenia opisów alternatywnych. Samo to już jest ciekawym wyzwaniem, czego doświadczyłem pisząc coś podobnego na potrzeby opisów służących do nawigowania.No i zaprzęgnięcie do tego sztucznej inteligencji też mnie rajcuje. Niechże te komputery na coś się wreszcie przydadzą.