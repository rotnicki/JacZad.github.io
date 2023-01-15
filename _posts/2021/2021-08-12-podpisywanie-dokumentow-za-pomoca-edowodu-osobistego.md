---
id: 2474
title: 'Podpisywanie dokumentów za pomocą edowodu osobistego'
date: '2021-08-12T19:00:00+02:00'
author: 'Jacek Zadrożny'
excerpt: 'Trwało to dość długo, ale w końcu aplikacja do składania podpisu osobistego pod Windows jest trochę dostępna. To ogromny postęp, bo wcześniej była zupełnie niedostępna. Napisałem zatem tutorial, który pomoże w korzystaniu z tej aplikacji.'
layout: post
guid: 'https://informaton.blog/?p=2474'
permalink: /2021/08/12/podpisywanie-dokumentow-za-pomoca-edowodu-osobistego/
categories:
    - tutoriale
tags:
    - edowód
    - 'podpisy cyfrowe'
    - tutorial
---

Dzisiaj przetestowałem zaktualizowaną wersję oprogramowania do podpisu osobistego. Dzielę się więc refleksjami i instrukcją obsługi dla niewidomych użytkowników.

## Czym jest podpis osobisty?

Podpis osobisty to rodzaj podpisu cyfrowego. Można za jego pomocą podpisywać dokumenty i przesyłać je przez Internet. To nie jest podpis kwalifikowany, którym można podpisywać niemal wszystko i traktowany jest na równi z odręcznym podpisem. Jednak uznawać go muszą podmioty publiczne. Jeżeli dwie strony się tak umówią, to można uznawać jes także w obiegu prywatnym. [Tu odnośnik do oficjalnego źródła](https://www.gov.pl/web/e-dowod/podpis-osobisty).

## Co jest potrzebne?

Do podpisywania dokumentów podpisem osobistym potrzebne są:

1. Dowód osobisty z warstwą elektroniczną. Takie dowody są wydawane od marca 2019 roku. Jeżeli masz stary dowód, możesz go wymienić na ten nowy. Przy składaniu wniosku zaznacz, że chcesz mieć warstwę elektroniczną.
2. Czytnik kart kryptograficznych kompatybilnych z edowodem. Ja kupiłem czytnik niemieckiej firmy Reiner i zapłaciłem niecałe 70 złotych. Certyfikowane czytniki kosztują znacznie więcej. Nie musisz kupować terminala/czytnika z klawiaturą.
3. Komputer osobisty, do którego można podłączyć czytnik kart. Oprogramowanie zostało przygotowane na różne systemy operacyjne, ale tylko to pod Windows nadaje się do użytku dla osób niewidomych.
4. Wspomniane wcześniej oprogramowanie. Zainstalować trzeba dwie aplikacje:  
    
    1. [oprogramowanie do podpisywania podpisem osobistym w wersji 64 bitowej](https://www.gov.pl/pliki/edowod/eDOSign-1.6.202_x64.msi) lub w [wersji 32-bitowej](https://www.gov.pl/pliki/edowod/eDOSign-1.6.202_x32.msi).
    2. [Oprogramowanie do zarządzania dowodem osobistym](https://www.gov.pl/pliki/edowod/e-dowod-4.2.2.2.exe).

## Jak to działa?

Kiedy podłączysz czytnik do komputera, na przykład przez port USB, pojawi się okno do wpisania numeru CAN. Ten numer znajduje się na dowodzie osobistym w wersji wydrukowanych cyfr i kodu kreskowego. Ja zeskanowałem ten kod aplikacją Seeing Assistant Home. Kod ma 6 cyfr, które trzeba wpisać w pole. Można zaznaczyć opcję zapamiętania kodu i zatwierdzić. Po chwili powinno pojawić się powiadomienie o wczytaniu certyfikatów.

Teraz możesz przystąpić do podpisywania dokumentu. Pracę można zacząć na 2 sposoby: otwierając aplikację do podpisu lub wybierając z menu kontekstowego pliku opcję podpisywania. Ten drugi sposób wydaje się prostszy, ale efekt jest podobny. Jeżeli zaczniesz od otwarcia aplikacji, to trzeba do niej i tak wczytać plik.

## Co można podpisywać?

Teoretycznie można wszystko. Jednak najwygodniejszym formatem jest PDF. W tym formacie można podpis upchnąć w jednym pliku, do tego obsługiwanym przez przeglądarki plików PDF. Jeżeli format jest inny, to powstaje dodatkowy plik z podpisem, na przykład XADES. Jest z tym potem sporo kombinowania, więc rekomenduję stosowanie plików PDF.

## Czy aplikacja jest dostępna?

Aplikacja do podpisywania jest częściowo dostępna w systemie Windows. Wersja na MacOS jest kompletnie niedostępna, a tej dla systemu Linux nie testowałem. W tej dla Windows napotkasz następujące problemy:

- Możesz poruszać się klawiszem Tab tylko do przodu. Skrót Shift + Tab nie działa.
- Na listach do wybierania różnych opcji, zawartość nie jest odczytywana. Listę trzeba rozwinąć i wybrać samemu opcję, żeby wiedzieć, co wybierasz.
- Aplikacja dość długo się uruchamia, więc uzbrój się w cierpliwość. U mnie trwało to kilkanaście sekund.
- Przy przełączaniu się między oknami, okno aplikacji do podpisu się nie anonsuje. Wyświetla się, ale uprzedzam, bo może to być konfundujące.
- Nie umiem dodać graficznego podpisu do dokumentu. Wydaje mi się, że tego nie da się zrobić z czytnikiem ekranu.

## Jak podpisać?

Wracam do procesu podpisywania. Jeżeli plik został otwarty z menu kontekstowego, to już jest na liście jako wybrany. Jeżeli został wczytany do aplikacji, to trzeba go jeszcze dodać. W tym trybie można dodawać wiele plików i hurtowo je podpisać.

1. Wybierz profil podpisu. Najczęściej będzie to “użytkownika”.
2. Wybierz format podpisu. Do wyboru jest kilka, ale ten najlepszy dla plików PDF to PADES.
3. Teraz masz możliwość zaznaczenia opcji, czy na dokumencie ma być umieszczony znak graficzny. Bez niego podpis i tak zostanie dodany, ale ludzie lubią od razu widzieć.
4. Dalej znajdziesz kilka jeszcze opcji do wyboru, które pozostaw domyślnie. Zazwyczaj zresztą te listy mają tylko jedną pozycję. Możesz ewentualnie wybrać typ zobowiązania z listy, jeżeli wiesz, co będzie najlepsze. Wreszcie dochodzimy do przycisku Podpisz.
5. pojawi się lista wyboru certyfikatów. Ja mam tylko jeden z moim imieniem i nazwiskiem, więc go wybieram.
6. W kolejnym kroku trzeba podać 6-cyfrowy PIN. To nie jest numer CAN! Ten PIN wymyślałem sam, podczas odbierania dowodu. Wpisałem numer… Nie, nie podam tutaj:) W tym oknie czeka nas mała niespodzianka. Otóż programiści wymyślili, że etykieta też będzie obsługiwana klawiaturą, więc musisz znaleźć pole edycyjne.
7. Dochodzimy teraz do okna ustawiania podpisu, o ile zaznaczona była opcja wstawiania znaku graficznego. Możesz wybrać stronę, na której będzie ten znak, dodać logo, wstawić dane z certyfikatu i obramowanie. Ja sobie wybrałem dane z certyfikatu i obramowanie. Niestety – podpis graficzny się nie pojawił w podpisanym dokumencie. Jeżeli ktoś znajdzie sposób, to proszę o informację.
8. Jeszcze jedno okno z poleceniem podpisania pliku i gotowe. W folderze z podpisywanym plikiem pojawia się drugi o niemal tej samej nazwie. Różni się tylko dodatkowymi literami BS. To jest właśnie podpisany dokument.

## Weryfikacja podpisu

Możesz też sprawdzić podpis i to przynajmniej na 2 sposoby.

1. Możesz otworzyć plik z podpisem w Adobe Reader i odszukać w narzędziach informacje o podpisie. Trochę to pracochłonne, ale się da.
2. Użyć aplikacji do podpisu także do weryfikacji. Do tego nie potrzebujesz czytnika i eDowodu.

W drugiej metodzie najłatwiej jest weryfikować podpis przez menu kontekstowe. Na pliku z podpisem rozwiń menu kontekstowe i wybierz “weryfikuj podpis”. Po chwili otworzy się aplikacja z wczytanym plikiem. Odszukaj przycisk “Weryfikuj podpis” i kliknij. Pojawi się okno z różnymi opcjami, które możesz przejrzeć. Najważniejszy dla Ciebie to “Odczytaj wynik weryfikacji”, pod którym dowiesz się, jaki to typ podpisu, kto go podpisał i co jest z nim ewentualnie nie tak. Jeżeli dokument jest podpisany więcej, niż jednym podpisem, to jeszcze z listy musisz wybrać, który podpis chcesz weryfikować.

To jest bardzo podstawowy tutorial. Jednak mam nadzieję go rozszerzyć o inne interesujące funkcje. A wkrótce tekst o podpisywaniu za pomocą aplikacji eDo App.