---
id: 292
title: 'Określenie języka strony (WCAG 2.0 SC 3.1.1, poziom A)'
date: '2012-10-05T08:46:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=292'
permalink: /2012/10/05/okreslenie-jezyka-strony-wcag-2-0-sc-3-1-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - język
    - niewidomi
    - semantyka
    - tekst
    - zrozumiałość
---

Właściwie każda strona internetowa jest napisana w jakimś języku, na przykład polskim, angielskim lub esperanto. Język ten powinien być prawidłowo zadeklarowany, by nie zakłócać możliwości korzystania z różnego rodzaju technologii, w tym asystujących. Na przykład automatycznych tłumaczy i odczytu treści za pomocą głosów syntetycznych.

Kryterium sukcesu 3.1.1 obliguje projektantów i redaktorów do jasnego określania języka, w jakim wyświetlana jest strona. Taka deklaracja powinna znajdować się w nagłówku dokumentu, by jak najszybciej przekazać ją do przeglądarki. Skorzystają na tym:

- użytkownicy niewidomi, korzystający z mowy syntetycznej i monitorów brajlowskich,
- użytkownicy słabo znający dany język,
- roboty sieciowe agregujące i wyszukujące treści,
- roboty tłumaczące treści.

Prawidłowa deklaracja języka dokumentu pozwala na zautomatyzowanie wielu zadań podczas pracy.

1. Syntezator mowy może przestawić się automatycznie na inny język, gdy wykryje taką zmianę na stronie. W ten sposób tekst polski będzie wypowiadany po polsku, a angielski – po angielsku. Brak deklaracji lub błędna deklaracja może spowodować, że polski tekst będzie wypowiadany po angielsku.
2. Oprogramowanie wyszukiwarek pozwala na określenie języka, w jakim mają być wyszukiwane treści. Błędna deklaracja języka może zatem doprowadzić do błędnego oznaczania treści w bazie wyszukiwarki, co utrudni lub uniemożliwi jej znalezienie.
3. Programy tłumaczące (translatory) mogą na podstawie błędnej deklaracji języka wykonywać błędne tłumaczenia lub nie będą w stanie przetłumaczyć treści.
4. W systemach wielojęzycznych może pojawić się problem z prawidłowym wyświetlaniem treści i użytkownikowi z Polski może ukazać się treść po fińsku i odwrotnie.

Kłopot z deklaracjami języka polega na tym, że negatywnych efektów prawie nikt nie dostrzega. Wszystkie czcionki wyświetlają się prawidłowo, co wynika ze stosowania standardu UTF-8, a problemy mają tylko użytkownicy z niepełnosprawnościami i właściciele serwisów, które z nieznanych dla nich powodów słabo się indeksują. A rozwiązanie jest tak proste: wystarczy prosty atrybut `lang="pl"` i wszystko zaczyna działać.