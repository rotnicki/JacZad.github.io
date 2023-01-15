---
id: 113
title: 'Określenie prawidłowej kolejności (WCAG 2.0 SC 1.3.2, poziom A)'
date: '2012-08-11T11:38:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=113'
permalink: /2012/08/11/okreslenie-prawidlowej-kolejnosci-wcag-2-0-sc-1-3-2-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - prezentacja
    - semantyka
    - tabele
---

Informacje umieszczone na stronie internetowej mają określoną kolejność. Mamy zatem tytuł, po nim obrazek ilustrujący treść i wreszcie akapit tekstu. Ta kolejność powinna być nie tylko widoczna, ale także określona w kodzie dokumentu. Dzięki temu każdy będzie z niej korzystał w analogiczny sposób.

Kryerium sukcesu 1.3.2 obliguje do zapisywania w dokumencie sekwencji informacji w sposób zrozumiały dla użytkownika. Oznacza to tyle, że kolejność informacji wynikająca z jej wyglądu powinna odpowiadać tej zakodowanej w sposób semantyczny. Skorzystają z tego:

 użytkownicy niewidomi, - użytkownicy starych przeglądarek internetowych,
- użytkownicy i programy przetwarzające informacje do innych form.

Za przykład niech nam posłuży dwukolumnowy układ wyświetlania artykułu. Są w nim dwie kolumny tekstu rozdzielone przerwą, a czasem także pionową linią. Odbierając tak sformatowaną informację wzrokiem, doświadczenie podpowiada że musimy przeczytać pierwszy wiersz w pierwszej kolumnie, a potem drugi wiersz w tej samej kolumnie. Jeżeli ktoś jednak nie odbiera tej informacji wzrokiem, to może nie dostrzec tej przerwy między kolumnami i pionowej linii i zacząć czytać będący na tej samej wysokości pierwszy wiersz w drugiej kolumnie. Wychodzi bełkot. To jest powszechnie spotykany problem w plikach PDF, które operują niemal wyłącznie informacją wizualną. Jeżeli jednak w pliku zawarta będzie informacja, że należy czytać informacje w konkretnej kolejności, to problem zniknie, a układ wizualny pozostanie bez zmian.

Innym przykładem może być wypełnianie formularza na stronie internetowej. Kolejność wypełniania pól bywa bardzo ważna i powinna być precyzyjnie określona. W formularzu rejestracji dzieci do przedszkoli powinno się w pierwszej kolejności wpisać numer PESEL, by system mógł sprawdzić, czy dziecko w ogóle kwalifikuje się do przedszkola. Jeżeli zaś ktoś wypełni wszystkie pola, by na końcu wpisać numer PESEL, to może się okazać, że zrobił to wszystko bez potrzeby.

Warto też zadbać o drobiazgi, na przykład o podanie formatu daty, jaki trzeba wpisać w pole formularza **przed** polem edycyjnym. Niewidomi użytkownicy korzystają ze stron w sposób sekwencyjny, to znaczy poznają treść po kolei, a nie skanują wzrokiem, jak użytkownicy widzący.