---
id: 1691
title: 'Sprawdzaj dostępność produkowanych treści w czasie rzeczywistym'
date: '2017-06-14T07:50:57+02:00'
layout: post
guid: 'http://informaton.pl/?p=1691'
permalink: /2017/06/14/sprawdzaj-dostepnosc-produkowanych-tresci-w-czasie-rzeczywistym/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - CMS
    - edytor
    - narzędzia
    - walidacja
---

[<span style="font-weight:400;">CKSource</span>](https://cksource.com/)<span style="font-weight:400;"> (firma stojąca za Accessibility Checkerem) od początku swojego istnienia za swą misję uważa dostarczanie narzędzi służących do produkowania treści na najwyższym poziomie. Taki też cel przyświeca tworzonemu edytorowi </span>[<span style="font-weight:400;">(</span><span style="font-weight:400;">CKEditor</span>](http://ckeditor.com/)<span style="font-weight:400;">) który niemal od samego początku dba o semantyczność generowanego kodu HTML. Obecnie, gdy powstaje CKEditor 5, nacisk na tworzenie poprawnego kodu stał się jeszcze większy, czego doskonałym dowodem jest stworzenie otwartego dla wszystkich projektu</span>[ <span style="font-weight:400;">Editor Recommendations</span>](http://ckeditor.github.io/editor-recommendations/)<span style="font-weight:400;">. Niemniej takie podejście nie wystarcza…</span>

<span style="font-weight:400;">CKEditor jest reprezentantem grupy produktów znanych szerzej jako Rich Text Editors (RTE, edytory “bogatego” tekstu). Prezentują one użytkownikowi podgląd “na żywo”, tego jak będzie wyglądać stworzona przez niego treść. Co więcej: użytkownik może nanosić na ten podgląd zmiany. To sprawia, że tego typu edytory znalazły bardzo szerokie zastosowanie w przeróżnego rodzaju CMS-ach (WordPress, Drupal, Joomla, itp.) i tym samym zrewolucjonizowały sposób tworzenia i zarządzania treścią w Internecie. Dzięki tym narzędziom treści tworzą również ludzie bez znajomości technicznych zawiłości Sieci, a zwłaszcza tego, jak powinien wyglądać semantyczny kod HTML. Dla tego typu użytkowników podstawowym kryterium, według którego oceniają edytor, jest fakt, że stworzona strona wygląda dokładnie tak, jak podczas edytowania w edytorze. Cała trudna praca związana z przerobieniem zamysłu użytkownika do porządnego kodu HTML spada na edytor.</span>

<span style="font-weight:400;">Oczywiście, CKEditor robi wszystko, by wygenerować jak najbardziej porządny HTML, niemniej nie zawsze jest w stanie to zrobić. Użytkownicy często bowiem omijają pola służące wpisaniu tekstu alternatywnego dla obrazków czy też stosują ręczne numerowanie akapitów (coś, co wygląda jak lista, dla użytkownika nietechnicznego </span>*<span style="font-weight:400;">jest</span>*<span style="font-weight:400;"> listą). W takim wypadku należy podsunąć użytkownikowi odpowiednie narzędzie.. W przypadku CKEditora najlepszy będzie</span>[ <span style="font-weight:400;">Accessibility Checker</span>](https://cksource.com/accessibility-checker/)<span style="font-weight:400;"> (AC).</span>

<span style="font-weight:400;">To niewielkie narzędzie służy do wykrywania najbardziej popularnych błędów, jakie popełniają użytkownicy edytorów, i pomaga im je poprawić. Jakiś obrazek nie posiada tekstu alternatywnego? AC szybko nam go wskaże i udzieli niezbędnych porad pozwalających nam dobrać odpowiedni opis do obrazka. Jakiś akapit za bardzo przypomina nagłówek? AC trzyma rękę na pulsie i zasugeruje, żeby użyć w tym miejscu </span>*<span style="font-weight:400;">prawdziwego</span>*<span style="font-weight:400;"> nagłówka. Dodatkowo ostrzeże nas przed ręcznie numerowanymi akapitami, tabelami bez opisu czy sąsiadującymi ze sobą linkami prowadzącymi do tego samego miejsca. Wystarczy postępować zgodnie z jego instrukcjami, żeby poprawić semantykę kodu HTML, co w bezpośredni sposób wpłynie także na dostępność strony (np. obrazki z dobrze dobranymi tekstami alternatywnymi będą prawidłowo odczytane przez czytniki ekranowe).</span>

<span style="font-weight:400;">Dla bardziej technicznych użytkowników CKEditora na pewno nie bez znaczenia będzie fakt, że kod AC jest dostępny na licencji Open Source i</span>[ <span style="font-weight:400;">znajduje się do pobrania na GitHubie</span>](https://github.com/cksource/ckeditor-plugin-a11ychecker)<span style="font-weight:400;">. Dzięki temu nawet najbardziej wymagający użytkownicy będą w stanie dostosować AC pod swoje zastosowania. Czy już wspominałem, że wśród nich znajduje się m.in.</span>[ <span style="font-weight:400;">rząd Holandii</span>](https://cksource.com/blog/Government-of-the-Netherlands-Case-Study)<span style="font-weight:400;">?</span>

<span style="font-weight:400;">Jednym z głównych zadań CKEditora jest generowanie najwyższej jakości kodu HTML, który spełniałby wszystkie normy i AC w tym zadaniu mu pomaga. Dzięki temu żaden użytkownik edytora nie musi się obawiać, że po edycji otrzyma po</span><span style="font-weight:400;">&lt;b&gt;</span><span style="font-weight:400;">a</span><span style="font-weight:400;">&lt;br&gt;</span><span style="font-weight:400;">aną papkę zamiast prawdziwego, soczystego HTML-a. </span>

<span style="font-weight:400;">Bo dobra treść zasługuje na najlepsze traktowanie!</span>