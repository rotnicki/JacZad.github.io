---
id: 1310
title: 'Wielkie umysły myślą podobnie, czyli o generatorze raportów dostępności od W3C'
date: '2015-04-22T10:01:16+02:00'
layout: post
guid: 'http://informaton.pl/?p=1310'
permalink: /2015/04/22/wielkie-umysly-mysla-podobnie-czyli-o-generatorze-raportw-dostepnosci-od-w3c/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - A3Web
    - audyt
    - badania
    - metodyka
    - raport
    - W3C
---

<span lang="en">World Wide Web Consortium</span> przygotowało [generator raportów z audytu dostępności](http://www.w3.org/WAI/eval/report-tool/#/), który może się przydać audytorom. Narzędzie jest proste, ale trudno je nazwać rozwiązaniem dla nowicjuszy. Do jego używania trzeba mieć odpowiedni zasób wiedzy związanej z dostępnością i WCAG 2.0. Generator jest zgodny z zaproponowaną przez W3C [metodyką stwierdzania dostępności.](http://www.w3.org/WAI/eval/conformance) Generator jest zatem czymś podobnym do opisywanego w tym blogu polskiego narzędzia [A3Web](http://informaton.pl/narzedzia/zapraszam-do-testowania-a3web/), co budzi wewnętrzną dumę, bo jestem ojcem chrzestnym tego ostatniego. Jednak są między nimi także różnice.

Generator od W3C jest po prostu generatorem raportów i niewiele więcej. W początkowej fazie generowania audytor wprowadza dane metryczkowe, na przykład poziom dostępności, stosowane technologie, adresy sprawdzanych stron, by wreszcie przejść do samego raportu. Przy każdym kryterium sukcesu może z listy wybrać jedną z możliwości: nie sprawdzono, spełnione, nie spełnione, nie występuje, a nawet “trudno powiedzieć”. Potem miejsce na wpisanie uwag i to w zasadzie tyle. W każdym momencie można pobrać plik z raportem w formacie HTML lub JSON na swój dysk, a generator większość pracy wykonuje po stronie użytkownika i zamknięcie przeglądarki niweczy całą pracę. Generator jest na razie tylko po angielsku, ale być może wkrótce będzie także po polsku.

A3Web został zaprojektowany nieco inaczej i głównym zadaniem tego narzędzia ma być edukacja jego użytkowników. Raport jest elementem dodatkowym, niejako podsumowaniem pracy. Dlatego przy każdym pytaniu są obszerne wyjaśnienia, sposób sprawdzenia, linki do materiałów zewnętrznych i oprogramowania. Jest jeszcze jedna różnica – A3Web działa bardziej awaryjnie i czasem potrafi zgubić jakieś wyniki. Zatem najgorzej działa w nim to, co działa świetnie w generatorze od W3C, a najlepiej to, czego ten drugi w ogóle nie posiada. Mogę zatem ze spokojnym sumieniem stwierdzić, że są to narzędzia komplementarne, przy czym zaczynać należy od A3Web, a dopiero później używać generatora od W3C.