---
id: 1291
title: 'Japońskie wytyczne dostępności różnią się od WCAG, bo Japończycy mają dziwne literki'
date: '2015-04-03T10:58:18+02:00'
layout: post
guid: 'http://informaton.pl/?p=1291'
permalink: /2015/04/03/japonskie-wytyczne-dostepnosci-rznia-sie-od-wcag-bo-japonczycy-maja-dziwne-literki/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - Japonia
    - standardy
    - tekst
    - 'WCAG 2.0'
---

Czytając różne informacje w sieci napotkałem na ciekawy dokument, a mianowicie [japońskie wytyczne dostępności dla treści w Internecie.](http://www.comm.twcu.ac.jp/~nabe/data/JIS-WAI/) Japończycy uznali, że WCAG 1.0 i WCAG 2.0 nie bardzo pasują do ich kultury i języka, więc postanowili zaprojektować swoje własne wytyczne dostępności. Nie robili tego w próżni, bo przykładali i porównywali do tych dwóch specyfikacji z W3C i podlinkowany dokument pokazuje różnice. <span lang="en">JIS Web Content Accessibility Guideline</span> powstał w roku 2004, a zatem w połowie okresu pomiędzy rokiem 1999, kiedy opublikowano WCAG 1.0, a 2008, kiedy oficjalnie opublikowano WCAG 2.0. W wypadku tego drugiego dokumentu opierali się na szkicu, a nie na pełnym dokumencie.

Okazuje się, że głównym powodem utworzenia własnego dokumentu jest inny alfabet, niż w wypadku alfabetów europejskich. Jak się zastanowić, to jest w tym sens, bo ideogramy japońskie są raczej grafikami oznaczającymi konkretne pojęcia lub sylaby, a nie graficznym odwzorowaniem fonemów. Innymi słowy – nasze alfabety to tekst, a japoński – raczej grafika. Problemy te opisano w części 6.2.2 dokumentu, gdzie wspomina się na przykład o tym, że ideogramy japońskie muszą być większe od liter alfabetów europejskich, aby dawały się odczytać. Sporo miejsca poświęcono też na kwestie stosowania wyróżnień i spacji w tekście oraz wykorzystywania niektórych znaków jako elementów graficznych, na przykład jako punktorów. Wreszcie – wspomniano o konieczności definiowania sposobu wymowy, co zaowocowało [kryterium sukcesu 3.1.6](http://informaton.pl/wcag-2-0/wymowa-wcag-2-0-sc-3-1-6-poziom-aaa/)w WCAG 2.0. Z kolei wielkość znaków alfabetów azjatyckich przewidziano w [kryterium sukcesu 1.4.8](http://informaton.pl/wcag-2-0/prezentacja-blokow-tekstu-wcag-2-0-sc-1-4-8-poziom-aaa/). Oba kryteria znajdują się na najwyższym poziomie dostępności, czyli AAA. Zakładam jednak, że są na tyle ważne dla Japończyków, że ten poziom ich nie satysfakcjonuje i wolą mieć te kryteria spełnione na poziomie o wiele niższym.

W dokumencie poruszane są jeszcze inne ciekawe aspekty, na przykład technologiczne (wprowadzanie i kodowanie znaków, czytniki ekranu), które mają lub mogą mieć wpływ na dostępność.Zawsze mnie frapowało, jak za pomocą zwykłej klawiatury komputerowej lub dotykowej w smartfonie można wprowadzać tysiące znaków ideograficznych alfabetów z Azji. Okazuje się jednak, że problem jest jeszcze większy, bo oznacza też kłopoty z kodowaniem znaków i to o wiele większe, niż w wypadku polskich diakrytyków. Dokument jest sprzed ponad dekady i zakładam, że Unicode rozwiązał te problemy, ale w momencie pisania dominującym systemem kodowania był ten oferowany przez system Windows. Ciekawe, jakie jeszcze czynniki mogą wpływać na dostępność treści w sieci, a o których nawet nie pomyśli ktoś z europejskiego kręgu kulturowego. A może s ą jakieś przesłanki religijne lub kulturowe… Szukam dalej.