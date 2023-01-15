---
id: 2323
title: 'Dostępny formularz &#8211; sprawa nie jest prosta'
date: '2021-05-16T19:12:40+02:00'
excerpt: 'Kilka podpowiedzi, jak podejść do kwestii dostępnych formularzy.'
layout: post
guid: 'http://informaton.blog/?p=2323'
permalink: /2021/05/16/dostepny-formularz-sprawa-nie-jest-prosta/
timeline_notification:
    - '1621185165'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - etykiety
    - formularz
    - HTML
    - PDF
    - Word
---

Jednym z częściej pojawiających się pytań podczas szkoleń, spotkań i webinarów jest to o dostępne formularze. Bo i sprawa nie jest trywialna. Rozwiązań jest kilka i każde ma swoje wady. Poniżej kilka moich propozycji oraz ostrzeżeń.

## Czego unikać przy tworzeniu dostępnych formularzy?

Jako człowiek realizujący zlecenia dla różnych klientów, miałem konieczność wypełniania przeróżnych formularzy. Były to przede wszystkim oświadczenia do celów podatkowych i ubezpieczeniowych. Każdy robi te formularze po swojemu, chociaż zbiera dokładnie te same informacje. Jednak dzięki temu miałem możliwość przeglądu różnych rozwiązań, których lepiej unikać.

1. Oznaczanie kolorem. Spotkałem się z formularzami, gdzie pewne informacje oznaczone były kolorem. Na przykład wskazywano w ten sposób pola obowiązkowe. Tego nie należy robić, ponieważ taki formularz może być niedostępny dla wielu użytkowników.
2. Skomplikowana tabela wizualna. To dość często spotykane rozwiązanie w formularzach, gdy autor stara się odwzorować papierowy formularz. Tworzy rozbudowaną tabelę, w której umieszcza etykiety i pola do wpisania danych. Sęk w tym, że formatowanie w ten sposób zazwyczaj oznacza mnóstwo pustych komórek tabeli. Dla osoby widzącej jest oczywiste, gdzie wpisać dane. Jednak dla osoby niewidomej nie jest to oczywiste, zwłaszcza gdy w okolicach komórki z etykietą jest kilka pustych komórek. Tego zdecydowanie warto unikać.
3. Komórki na cyfry. Spotkałem się z formularzem, w którym na numer rachunku bankowego, numeru PESEL i NIP ktoś wymyślił tabelki z jednym wierszem i odpowiednio 26, 11 i 10 komórek. Należało pracowicie wpisywać cyfry do kolejnych komórek, a potem pewnie równie pracowicie ktoś je przepisywał. To jest zbędne utrudnianie sobie pracy, bo numer rachunku zazwyczaj po prostu się kopiuje.
4. Kontrolki formularzy Word. Edytor tekstu Word pozwala na umieszczenie w formularzu kontrolek, w tym pól wyboru, edycyjnych itp. Bardziej zaawansowani użytkownicy wiedzą o tym i wykorzystują je do tworzenia elektronicznych formularzy. Niestety – te kontrolki są słabo dostępne dla technologii asystujących. Nie przenoszą się także do formatu PDF lub HTML. Sugeruję zatem unikanie, przynajmniej do czasu, gdy Microsoft ogarnie temat.

## To jak to robić?

Na początek przypomnienie, o co trzeba zadbać przy tworzeniu formularzy. Zwróciłbym szczególną uwagę na następujące kryteria sukcesu:

- Kryterium sukcesu 1.3.1 Informacje i relacje, zwłaszcza w kontekście skomplikowanych układów graficznych.
- Kryterium sukcesu 1.3.3 Właściwości zmysłowe, zwłaszcza przy instruowaniu o sposobie wypełniania formularza. W tym samym miejscu wskazałbym kryterium sukcesu 1.4.1 Użycie koloru.
- Kryterium sukcesu 2.1.1 Klawiatura, czyli aby wypełnienie formularza było możliwe z użyciem wyłącznie klawiatury.
- Kryterium sukcesu 3.2.1 Po otrzymaniu fokusu i 3.2.2 Podczas wprowadzania danych, w przypadku tzw. interaktywnych formularzy.
- Kryterium sukcesu 3.3.1 Identyfikacja błędu, oczywiście tylko w przypadku formularza sprawdzającego poprawność danych.
- Kryterium sukcesu 3.3.2 Etykiety lub instrukcje – chyba najważniejsze kryterium w przypadku formularzy, którego **zawsze trzeba pilnować**
- Kryterium sukcesu 3.3.3 Sugestie korekty błędów i 3.3.4 Zapobieganie błędom (prawnym, finansowym, w danych – co dotyczy formularzy do wprowadzania danych i przesyłania ich przez Internet lub inną sieć.
- Kryterium sukcesu 4.1.2 Nazwa, rola, wartość, czego również należy pilnować. W standardowych rozwiązaniach (HTML, PDF) jest to robione automatycznie. W innych – trzeba sprawdzać.

Pozostałe kryteria powinny być także uwzględnione, chociaż wydają się być mniej istotne. Poszczególne elementy z powyższej listy mają zastosowanie tylko w konkretnych rozwiązaniach, jak choćby walidowanie danych, co w Wordzie zrobić jest dość trudno.

Biorąc to wszystko pod uwagę zaproponuję kilka rozwiązań problemu dostępnych formularzy. To z pewnością nie jest lista wyczerpująca, ale może pomoże w poszukiwaniach.

## Word i prosta tabela

Jednym z prostszych rozwiązań, jakie spotkałem w przypadku formularzy przygotowanych w edytorze Word było takie oparte na tabeli. Składała się z 2 lub 3 kolumn, przy czym można zrobić wersję z numeracją wierszy lub sobie odpuścić. Zasadnicza tabela to 2 kolumny, z których pierwsza to etykieta, a druga – miejsce na wpisanie danych. Rozwiązanie jest dość oczywiste dla większości użytkowników, ale dla pewności można dodać instrukcję wypełniania. Może wyglądać na przykład tak:

> W pierwszej kolumnie tabeli zawsze znajduje się etykieta, a w drugiej miejsce na wpisanie danych. W przypadku pytań należy wpisać „tak” lub „nie”.

## Word i lista

Drugim rozwiązaniem możliwym do przygotowania w dowolnym edytorze tekstu jest wariacja pierwszej propozycji. Zamiast tabeli można użyć listy i umieszczać w niej etykiety zakończone dwukropkiem i spacją. Użytkownik zapewne domyśli się, że trzeba dane wpisywać po dwukropku, ale instrukcja na pewno nie zawadzi.

> Informacje należy wpisywać po dwukropku. W przypadku pytań należy wpisywać „tak” lub „nie”.

## Formularz w PDF

Dobrze przygotowany formularz w formacie PDF może być w pełni dostępny i interaktywny. Narzędzia do przygotowania takiego formularza znajdują się w aplikacji Adobe Acrobat. I jest to podstawowa wada tego rozwiązania. Oprogramowanie jest komercyjne, stosunkowo drogie i trudne w użyciu. Sam format PDF nie jest przeze mnie lubiany, czemu [dawałem wielokrotnie wyraz.](https://informaton.blog/2013/07/18/opamietajcie-sie-i-przestancie-uzywac-formatu-pdf-bez-potrzeby/) Tak więc nie mam zamiaru zachęcać, ale uczciwie przyznaję, że się da.

## Formularz w HTML

To rozwiązanie jest najbardziej optymalne. HTML zawiera w sobie wszystkie niezbędne kontrolki: pola tekstowe, wyboru, opcji, listy, które wiadomo, jak uczynić w pełni dostępnymi. Wersja 5 wprowadza też nowe typy pól tekstowych, które pozwalają na podstawową walidację danych. Odpowiednie skrypty mogą inteligentnie podpowiadać poprawne wartości, coś przeliczać itp. Samo dobre.

Problemem jest jedynie, co z takim wypełnionym formularzem zrobić. Najlepiej, jeżeli na drugim końcu jest aplikacja, która przyjmie te dane, przetworzy i na tym się skończy. Tak się dzieje w przypadku formularzy usług publikowanych w portalu gov.pl. Jednak to jest już pewne wyzwanie techniczne, a poza tym czasem trzeba to zrobić inaczej.

Można zatem wypełnić formularz i przekonwertować do formatu PDF za pomocą jakiejś biblioteki. Tak wiem – format PDF jest do niczego, ale sprawdza się w przynajmniej dwóch sytuacjach. Jeżeli taki dokument mamy wydrukować i podpisać odręcznie lub podpisać go cyfrowo. Tylko format PDF pozwala na wygodne podpisywanie zarówno podpisem kwalifikowanym, osobistym, jak i zaufanym.

## Na co zwracać uwagę?

Na koniec kilka rad dla autorów elektronicznych formularzy.

1. Pamiętaj o instrukcjach dla osoby wypełniającej. Sucha etykieta „PESEL” nie dla wszystkich będzie zrozumiała. Dopisz, że to numer składający się z 11 cyfr umieszczony na dowodzie osobistym.
2. Dbaj o to, by użytkownik zawsze wiedział, co będzie mu potrzebne do wypełnienia formularza. Jest to szczególnie ważne w przypadku formularzy, w których czas jest ograniczony. Frustrujące jest szukanie w panice numeru dowodu osobistego, adresu urzędu skarbowego lub daty wystawienia paszportu.
3. Stosuj odpowiednio duże litery, gdy formularz ma być wydrukowany. Po wydrukowaniu użytkownik może chcieć sprawdzić poprawność danych, więc ułatw mu to.
4. Jeżeli nie wszystkie pola formularza są obowiązkowe, oznacz wyraźnie te które trzeba wypełnić. Zrób to kolorem, pogrubieniem, informacją tekstową, a gdy się da – semantyczną (HTML i PDF).
5. Jeżeli tylko się da, stosuj prosty język. W szczególności unikaj mało znanych pojęć i skrótów.

Mam nadzieję, że trochę podpowiedziałem. A na dodatkowe pytania mogę odpowiedzieć w komentarzach.