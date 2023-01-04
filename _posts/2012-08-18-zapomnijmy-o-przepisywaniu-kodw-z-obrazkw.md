---
id: 143
title: 'Zapomnijmy o przepisywaniu kodów z obrazków'
date: '2012-08-18T10:31:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=143'
permalink: /2012/08/18/zapomnijmy-o-przepisywaniu-kodw-z-obrazkw/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audio
    - CAPTCHA
    - daltonizm
    - formularze
    - grafika
    - niewidomi
---

![Przekreślony kod obrazkowy CAPTCHA](https://i0.wp.com/informaton.pl/wp-content/uploads/2012/08/captcha_skreslona.jpg?w=1140)CAPTCHA – całkowicie zautomatyzowany test służący odróżnianiu komputera od człowieka (ang. Completely Automated Public Turing test to tell Computers and Humans Apart). Najczęściej służy do blokowania dostępu do pewnych treści komputerom (na przykład szkodliwym skryptom), a jednocześnie pozwalający na dostęp ludziom. Nazwany został od nazwiska naukowca Alana Turinga, który jako pierwszy zaproponował takie rozwiązanie.

## Do czego służy CAPTCHA?

Odpowiedź jest prosta ? do zabezpieczenia serwisów i usług internetowych przed robotami sieciowymi. Programiści z różnych przyczyn piszą aplikacje, które zakładają konta pocztowe w darmowych serwisach i konta użytkowników, najczęściej po to, by spamować. Ini programiści bronią serwisów przed tym procederem stosując różnorakie zabezpieczenia, w tym w pierwszej kolejności właśnie CAPTCHA. Może to być realizowane na wiele różnych sposobów, z których najpopularniejsze to:

- - kody obrazkowe;
    - kody dźwiękowe;
    - zagadki logiczne;
    - analiza ruchu i numerów IP.

Pierwsze trzy sposoby wymagają od użytkownika wykonania pewnych działań – odczytania liter z obrazka, odsłuchania nagrania lub odpowiedzi na zagadkę. W ten sposób przerzucają obowiązek zidentyfikowania się jako człowieka na użytkownika. A przecież roboty coraz lepiej podszywają się pod ludzi. Potrafią dekodować informacje graficzne i dźwiękowe, co czyni ten sposób zabezpieczenia nieskutecznym, a wręcz askutecznym.

Ponieważ automaty potrafią już odczytywać kody obrazkowe, więc następuje eskalacja ? kody robią się coraz bardziej skomplikowane do odczytania, a algorytmy podążają za tą komplikacją. Komplikacja wyglądu kodu posunięta bywa do tego stopnia, że poważny kłopot z odczytaniem mają też ludzie. Zniecierpliwiony klient to stracony klient, o czym zdają się zapominać projektanci stron internetowych. W pewnym momencie może dojść do sytuacji, gdy z odczytaniem obrazka poradzi sobie tylko automat, a człowiek już nie. Przy tym komputer jest nieskończenie cierpliwy, czego o człowieku powiedzieć się nie da.

Tymczasem kody obrazkowe wprowadzane są w sposób bezrefleksyjny, nawet tam, gdzie może ich nie być. Komentarze, zakupy, zakładanie konta użytkownika – wiele z tych operacji wykonywanych jest kompulsywnie i wprowadzenie utrudnień może sprawić, że użytkownik otrzeźwieje i zrezygnuje z danej operacji.

## Czy aby na pewno potrzebne mi takie zabezpieczenie?

Każdy projektant usługi internetowej powinien zadać sobie pytanie, czy aby na pewno potrzebne jest mi takie zabezpieczenie? Wbrew pozorom często odpowiedź na takie pytanie będzie brzmiała “nie”. Nader często jednak nikt sobie takiego pytania nie zadaje i wstawia kod obrazkowy “z rozpędu”. Potem mozolnie szuka odpowiedzi na pytanie, czemu ruch i rejestracje użytkowników są mniejsze od oczekiwanych. A użytkownicy są coraz wybredniejsi i coraz bardziej leniwi. Stąd lubią logować się za pomocą konta Facebooka lub w ogóle się nie rejestrują. Projektant musi zatem na jednej szali położyć zdegustowanego i zniechęconego użytkownika, a na drugiej – jeden zbędny rekord w bazie danych.

## Co zamiast?

Zamiast przerzucać obowiązek rozpoznania użytkownika na potencjalnego klienta można to zadanie powierzyć innym programom. Kodów zabezpieczających nie ma w serwisie WordPress.com, a przecież komentować może każdy. Nie ma ich w serwisie Allegro, który jest przecież narażony na skanowanie przez roboty sieciowe. Za to mały sklepik internetowy mający w ofercie 20 produktów, który wprowadza kody obrazkowe w momencie rejestrowania klientów, a nawet – co już zakrawa na samobójstwo sprzedażowe – w momencie składania zamówienia. Ten moment zatrzymania klienta i zmuszanie go do wykonywania dodatkowych, dosyć wymagających operacji, może go także powstrzymać od zakupów. A przecież jeżeli jakiś komputer chce u nas kupić towar i za niego zapłacić, to przecież nawet lepiej.

Czasem faktycznie trzeba zabezpieczyć się przed robotami i wtedy wystarczy sprawdzać zachowania klienta. Wielokrotne zakładanie konta z jednego numeru IP może poważnie sugerować robota, więc można zastosować zabezpieczenia CAPTCHA w momencie, gdy **po raz drugi** z tego samego numeru ktoś chce założyć konto. Komentarze można zabezpieczyć na wiele sposobów, na przykład przez prostą analizę treści lub potwierdzenie przez pocztę elektroniczną. Sposobów jest wiele i każdy z nich jest lepszy od obciążania klientów zadaniami, które może zrobić program.

Na koniec warto pamiętać, że kody obrazkowe uniemożliwiają dostęp klientom z niepełnosprawnością wzroku (niewidomym, słabowidzącym, z daltonizmem), których w Polsce jest około 1,8 miliona. Problemu nie rozwiązują kody dźwiękowe, bo są one jeszcze trudniejsze do zdekodowania słuchem, niż kody obrazkowe dla osób widzących.Na koniec zatem proponuję zrobić prosty eksperyment – wyłączenie tego rodzaju zabezpieczeń i sprawdzenie, czy liczba klientów wzrosła szybciej, niż ilość spamu.