---
id: 1625
title: 'JavaScript i dostępność &#8211; zarządzanie fokusem i powiadamianie użytkownika'
date: '2017-03-01T09:09:55+01:00'
layout: post
guid: 'http://informaton.pl/?p=1625'
permalink: /2017/03/01/javascript-i-dostepnosc-zarzadzanie-fokusem-i-powiadamianie-uzytkownika/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - fokus
    - JavaScript
    - klawiatura
---

Niedawno podczas rozmowy ze znajomym na temat dostępności pojawił się problem, jak zakwalifikować pewien błąd dostępności. Chodziło o odtwarzacz multimediów, który uruchamiał się jako okno modalne. Sęk w tym, że okno dodawane było na samym końcu drzewa DOM i nie było w żaden sposób anonsowane. Efekt był taki, że niewidomy użytkownik klikał na link z filmem i z jego punktu widzenia nic się nie działo. Klikał więc ponownie i jeszcze raz, z dokładnie takim samym skutkiem. Mógł oczywiście znaleźć okno odtwarzacza, gdyby przyszło mu do głowy, by go szukać na końcu strony, ale niby skąd miałoby mu taka myśl zaświtać? Podczas rozmowy uzgodniliśmy, jak to opisać w raporcie z badania, a dzisiaj trafiłem na artykuł w Medium, który traktuje dokładnie o tym samym.

Artykuł jest dosyć krótki i autor daje tylko kilka podstawowych wskazówek, jak skorzystać z JavaScript i ARIA dla rozwiązania problemu modalnego okienka. Opisuje zarządzanie fokusem klawiatury oraz anonsowanie okna, a także dodawanie obsługi klawiaturą do elementów, które tej obsługi wymagają. Bardziej zestaw tricków, niż obszerne opracowanie, ale dosyć przejrzyście napisane. Polecam, w szczególności zaczynającym przygodę z dostępnością.

Źródło: *[Writing JavaScript with accessibility in mind – A List Apart Sidebar – Medium](https://medium.com/@matuzo/writing-javascript-with-accessibility-in-mind-a1f6a5f467b9)*