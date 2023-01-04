---
id: 2025
title: 'Pismo jest fundamentem dostępności cyfrowej, który się chwieje'
date: '2019-07-18T10:14:52+02:00'
layout: post
guid: 'http://informaton.blog/?p=2025'
permalink: /2019/07/18/pismo-jest-fundamentem-dostepnosci-cyfrowej/
timeline_notification:
    - '1563437693'
publicize_twitter_user:
    - jaczad
categories:
    - artykuły
tags:
    - grafika
    - język
    - kontrast
    - pismo
    - tekst
    - 'tekst alternatywny'
    - WCAG
    - 'WCAG 2.1'
---

Im dłużej przyglądam się skodyfikowanym zasadom dostępności cyfrowej, tym bardziej widoczne dla mnie jest, jak ważnym fundamentem jest tu pismo. WCAG jest dobrym dokumentem do analizy, bo jest najbardziej uznanym i szeroko przyjętym. Jednak dotyczy to chyba wszystkich tego typu wytycznych.

## Tekst na początku i końcu

WCAG zaczynają się od alternatywy tekstowej, jako głównego nośnika dostępności dla obiektów, które tekstem nie są. Mamy zatem elementy tekstowe i te nie będące tekstem, które o tekst należy uzupełnić. Wszędzie tekst, bo jest łatwo przetwarzalny na inne formy informacji, zarówno analogowe, jak i cyfrowe. Można go łatwo skonwertować do sztucznej mowy za pomocą syntezatora mowy; do alfabetu Braille’a; wyświetlić na ekranie w dowolnej wielkości i kolorystyce; przetłumaczyć na inne języki; wydrukować… W przyszłości może da się przetłumaczyć na język migowy lub poddać uproszczeniu. Automatyczne upraszczanie i streszczanie już jest dostępne dla innych języków, chociaż wciąż brakuje takiego rozwiązania dla języka polskiego.

Sięgając na koniec WCAG znajdziemy poprawność kodu, czyli sformalizowanego tekstu przetwarzalnego maszynowo. Ta klamra spina WCAG poczynając od pisma zrozumiałego dla ludzi, a kończąc na piśmie zrozumiałym dla maszyn. Informacja musi być zrozumiała zarówno dla ludzi, jak i dla oprogramowania, by mogła być uznana za dostępną. Stąd pojawiające się czasem uproszczenie, że informacja przetwarzalna maszynowo jest dostępna. Tak naprawdę, to jest jeden z warunków, wcale nie wystarczający, chociaż konieczny.

Pomiędzy tymi dwoma skrajami WCAG mieści się wiele innych elementów opartych na tekście. W multimediach – deskrypcje i napisy. W formularzach – etykiety i instrukcje. W semantyce – definiowanie programistyczne lub opis w tekście, zupełnie jak na początku i końcu WCAG.

## Wyspy na oceanie tekstu

Przebiegając przez WCAG można dostrzec kilka wyjątków od wszechobecności tekstu, jako nośnika dostępności. Małą wysepkę można znaleźć w zasadach dotyczących multimediów, gdzie mowa jest o audiodeskrypcji i tłumaczeniach na język migowy. Chociaż i tam zazwyczaj warstwą pośredniczącą jest tekst w postaci skryptu lub wstępnego tłumaczenia. Bez nich można się jednak czasem obejść.

Dużą wyspą, czy może wręcz kontynentem, jest druga zasada: funkcjonalność. Niemal wszystkie wytyczne i kryteria sukcesu dotyczą interakcji, a zatem sposobu użytkowania. Klawiatura, czas i migotanie treści – to wszystko dotyczy tekstu tylko pośrednio. Klawiatura może bowiem służyć do wprowadzania tekstu, a jednocześnie do nawigowania. Migotanie może dotyczyć tekstu, ale także każdego innego elementu interfejsu i treści. Nareszcie elementy zmienne w czasie mogą być tekstem lub czymkolwiek innym. Tekst jest tu zatem postawiony na równi z grafiką lub kontrolkami interfejsu użytkownika.

Dalej to już głównie tekst – jego zrozumiałość, określenie języka, etykiety, instrukcje, pomoc, komunikaty o błędach itp. Nawet jeżeli dopatrywać się tam fragmentów nie dotyczących tekstu wprost, jak zrozumiała nawigacja, tonie są to elementy oderwane od pozostałych wymagań, a zatem alternatywa tekstowa lub wyjaśnienie tekstowe są tam obecne.

## Nadchodzące zmiany

Jednak wszyscy dostrzegają zmiany, jakie zachodzą w tworzeniu i publikowaniu treści w sieci. Tekst jest wciąż ważny, ale coraz ważniejsze są multimedia i zupełnie nowe sposoby interakcji z interfejsami. Warto zatem zerknąć na aktualizację WCAG do wersji 2.1, by przemyśleć ten trend.

O ile w WCAG 2.0 tekst dominował, to w aktualizacji stał się marginalny. Co więcej – łata pewne braki, gdy tekst był nadmiernie promowany. Tak stało się choćby w kryterium sukcesu kontrastu dla treści nie będących tekstem. Faktycznie – obecnie grafika jest często ważniejszym lub wręcz jedynym nośnikiem informacji, więc powinna być dostępna.

W dwóch kryteriach dotyczących tekstu wprost, definiują one sposób jego prezentacji lub możliwości dostosowania wyglądu. Do tego należy dodać dwa kryteria dotyczące etykiet funkcjonalnych i tożsamych z prezentacją graficzną oraz ostatnie z kryteriów, które z tekstem związane jest pośrednio. Reszta to interakcja z interfejsami dotykowymi i kilka innych.Może to wynikać z faktu, że WCAG 2.0 były dobrze przemyślane, ale równie dobrze może być tak, że nowe technologie wskazały nowe wyzwania dla dostępności.

## Wyzwania dla dostępności

Te rozważania nie biorą się znikąd. Kilka dni temu dostałem serię pytań po szkoleniu z dostępności cyfrowej, a pośród nich dwa dosyć często się powtarzające. Pierwsze dotyczyło alternatyw tekstowych dla zdjęć publikowanych w galeriach, a drugie – skanów dokumentów papierowych. Czy bowiem każde zdjęcie w galerii powinno mieć tekst alternatywny? Z punktu widzenia WCAG – oczywiście. Chociaż z drugiej strony… Jaki jest cel istnienia galerii zdjęć? Czy niosą ze sobą istotną informację, czy są tylko efektem zbyt dużej łatwości tworzenia i udostępniania multimediów? Dodanie zdjęcia do galerii może się ograniczyć do intuicyjnego rozpoznania dobrze zrobionej fotografii i dwóch kliknięć myszą. Zapewnienie mu alternatywy tekstowej wymaga nie tylko wiedzy, jak to zrobić, ale każdorazowego uruchomienia procesu myślowego, by taki opis przygotować. Jeżeli robi się to z urządzenia mobilnego, to pisanie jest dodatkowo uciążliwe technicznie, zwłaszcza gdy tekst zawiera znaki diakrytyczne.Mamy zatem z jednej strony proste przeciągnięcie palcem zdjęcia w odpowiednie miejsce, a z drugiej grzebanie w interfejsie, zastanawianie się nad deskrypcją i mozolne wpisywanie alternatywy w odpowiednie pole. A na koniec często brak pewności, że czynność została wykonana prawidłowo, bo przecież tekstu alternatywnego nie widać. Innymi słowy – z jednej strony satysfakcja przy niewielkim nakładzie sił, a z drugiej – spory nakład pracy i niepewność skuteczności. Kiedyś ta różnica była mniejsza, bo opublikowanie zdjęcia odbywało się w topornym interfejsie webowym i to na komputerze. Więc może jednak przyjąć że te galerie to takie ozdobniki strony, nie niosące ze sobą istotnej informacji, a zatem nie wymagające alternatywy tekstowej. Na razie nie umiem odpowiedzieć na to pytanie.

Ze skanami dokumentów w formacie PDF jest inaczej. Najczęściej wciąż są publikowane za pomocą interfejsu webowego na komputerze, a przygotowanie alternatywy tekstowej wymaga jedynie mechanicznego przeniesienia informacji. Poza tym – tych plików jest drastycznie mniej, bo ich powstanie nie polega na kliknięciu jednego przycisku w smartfonie, tylko sporego nakładu czasu i pracy człowieka. Nawet wówczas, gdy część tej pracy wykona komputer. Poza tym pliki PDF zazwyczaj rodzą się dostępne tekstowo, bo w edytorze tekstu na komputerze użytkownika. Dopiero potem ich dostępność jest niszczona przez wydrukowanie i ponowną digitalizację, tym razem do niedostępnej formy mapy bitowej. Dlatego tu mam zdecydowanie mniej zrozumienia dla braku dostępności cyfrowej. Tym bardziej, że one zawsze niosą informację i nie mają charakteru ozdobnego.

Mamy zatem dwa rodzaje obiektów publikowanych w sieci: zdjęcia i pliki PDF. Dla zdjęć tekst jest elementem pochodnym, a dla plików PDF – pierwotnym. Zdjęcie robi się szybko, a plik PDF – długo i mozolnie. Właściwie każde multimedia robi się obecnie łatwiej, niż dokument tekstowy. Zdjęcia, filmy, nagrania dźwiękowe – smartfon pozwala robić to za pomocą wbudowanych lub instalowanych aplikacji w prosty i efektowny sposób. Ewa robi zazwyczaj kilkanaście zdjęć, by zostawić jedno w albumie, więc efekt jest dobry przy wciąż niewielkim nakładzie pracy. A tekst powstaje mozolnie, z wklepywanych cierpliwie liter, słów, znaków przestankowych. Dlatego tekst jako fundament dostępności się chwieje. Zbyt dużo ludzi produkuje łatwo treści, a zbyt mało dba o ich dostępność, by można było dostrzec postęp. Jedyną szansą są nieskończenie cierpliwe komputery, które może kiedyś nauczą się interpretować obraz na zdjęciach i filmach, jak obecnie potrafi rozpoznawać mowę. To jednak wciąż odległa, a może wręcz nieosiągalna przyszłość.