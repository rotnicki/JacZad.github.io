---
id: 450
title: 'Dostępność stron internetowych w systemach prawnych innych krajów'
date: '2012-12-20T13:00:52+01:00'
layout: post
guid: 'http://informaton.pl/?p=450'
permalink: /2012/12/20/dostepnosc-stron-internetowych-w-systemach-prawnych-innych-krajw/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - prawo
    - standardy
    - 'WCAG 2.0'
---

W związku z projektowaną [dyrektywą o dostępności stron internetowych podmiotów publicznych](http://informaton.pl/?p=413) oraz [stanowiskiem polskiego rządu w tej sprawie](http://informaton.pl/?p=446) przytaczam tekst przeglądowy, jaki opublikowałem w maju 2010 roku. Z całą pewnością już się zdezaktualizował, ale pokazuje różnice, jakie mogą się pojawić podczas implementowania dostępności. Wprowadzenie pojedynczej normy może się przyczynić do lepszego przepływu pracowników i usług na wspólnym rynku. Ciekawi mnie tylko, jak rozwiązać problem wyższych standardów, na przykład stosowanych we Włoszech.

Do polskiego prawa powoli wchodzi dostępność (accessibility) stron internetowych. Piszę tu oczywiście o rodzącym się rozporządzeniu Rady Ministrów. Ostatnio trochę o tym poczytałem i mogę ostrożnie napisać kilka słów na ten temat.

### Standardy

Dostępność informacji elektronicznej została opisana na wiele sposobów w różnych specyfikacjach. Najbardziej popularne są specyfikacje grupy roboczej [Web Accessibility Initiative](http://www.w3.org/wai) wewnątrz [World Wide Web Consortium](http://www.w3.org). Na potrzeby wdrażania dostępności w Internecie powstał cały zestaw dokumentów, z których najważniejsze to:

1. 1. Web Content Accessibility Guidelines ([1.0](http://www.w3.org/TR/WCAG10/) z 1999 r. i [2.0](http://www.w3.org/TR/WCAG20/) z 2008 r.)
    2. Authoring Tools Accessibility Guidelines ([1.0](http://www.w3.org/TR/ATAG10/) z 2000 r. i [2.0](http://www.w3.org/TR/ATAG20/) w wersji draft)

Pierwszy opisuje, jak powinna być zaprojektowana treść publikowana w Internecie, by była dostępna dla wszystkich użytkowników. Druga pokazuje, jak projektować narzędzia do publikowania treści, by ta treść była możliwie dostępna. Obie specyfikacje są podzielone na trzy poziomy dostępności (A, AA i AAA), z których pierwszy jest obowiązkowy, by osiągnąć podstawową dostępność, drugi rozszerzoną i trzeci ? zaawansowaną.

Szczególnie specyfikacja WCAG okazała się istotna dla dostępności, ponieważ większość innych rozwiązań czerpie z tego zasobu. Niektóre uregulowania wskazują wprost na ten dokument, a inne opierają się na nim, choć zostały zaprojektowane w inny sposób lub zostały rozszerzone. Tak czy inaczej – WCAG jest najważniejszym dokumentem o dostępności jaki istnieje obecnie w obrocie informacyjnym.

Mniej znanym (choć niezasłużenie) jest ATAG. Polecam go wszystkim programistom, którzy tworzą aplikacje sieciowe, w tym systemy społecznościowe. Tam, gdzie treść powstaje w wyniku pracy wielu użytkowników trudno zapanować nad jej dostępnością. Jednak można zaproponować użytkownikom pewne narzędzia, które zachęcą, a czasem wręcz zmuszą, do tworzenia treści w sposób dostępny.

Oba dokumenty są ze sobą równoległe, to znaczy że WCAG 1.0 jest zgodny z ATAG 1.0, a istniejąca wersja WCAG 2.0 będzie zgodna z rodzącym się ATAG 2.0 Nie znaczy to jednak, że nie warto korzystać z ATAG 1.0, bo jest przestarzały. Zasady są dosyć uniwersalne i ciągle warto się ich trzymać.

### Rozwiązania w innych krajach

W wielu krajach uregulowano już problem dostępności publicznych stron internetowych i poniżej znajduje się krótki przegląd wybranych rozwiązań. Uszeregowałem je w kolejności chronologicznej, a nie ważności, choć może nie jest to wybór najlepszy z możliwych.

### USA

The Rehabilitation Act, [Section 508](http://www.section508.gov) (1998)

Na podstawie amerykańskiej ustawy rehabilitacyjnej stworzono specyfikacje dotyczące dostępności, które nie ograniczają się wyłącznie do dostępności stron internetowych.

1. 1. ? 1194.21 Software applications and operating systems (oprogramowanie i systemy operacyjne).
    2. ? 1194.22 Web-based intranet and internet information and applications. 16 zasad, z których 11 jest zgodnych z WCAG 1.0 level A, a pozostałe 5 jest odrębnych.
    3. ? 1194.23 Telecommunications products (urządzenia telekomunikacyjne).
    4. ? 1194.24 Video and multimedia products (urządzenia multimedialne, na przykład telewizory).

Jak zatem widać Amerykanie poszli na całość i postanowili określić standardy na dużo więcej, niż tylko strony internetowe. Należy także dodać, że chociaż ustawowe zobowiązanie dotyczy tylko serwisów rządowych, to zaistniały już precedensy skarżenia o dostępność stron internetowych przez niewidomych obywateli. Dodam, że procesy zakończyły się ugodą ze wskazaniem na obywateli.

Sam standard dostępności stron internetowych jest dość prosty, ale stał się drugim po WCAG wyznacznikiem dostępności. Powołują się na niego Włosi w swoim Stanca Law, o którym wkrótce.

### Portugalia

[Resolution of the Council of Ministers n? 97/99](http://www.acesso.umic.pt/acesso/res9799_en.htm) (1999).

Wewnętrzne zobowiązanie rządu portugalskiego do oferowania informacji na stronach internetowych w formie dostępnej. Do tego celu zaprojektowano wytyczne oparte o WCAG 1.0. Warto zwrócić uwagę na to uregulowanie, bo nie jest to zobowiązanie innych, ale samych siebie. Nie umiem ocenić efektywności takiego mechanizmu, ale podoba mi się.

### Niemcy.

[Federal Ordinance on Barrier-Free Information Technology](http://www.einfach-fuer-alle.de/artikel/bitv_english/bitv_annex1/) (2002)

(Ordinance on the Creation of Barrier-Free Information Technology in Accordance with the Act on Equal Opportunities for Disabled Persons Barrierefreie Informationstechnik-Verordnung – BITV

Na podstawie sekcji 11(1) zdanie 2 ustawy o równych szansach osób niepełnosprawnych (27 kwietnia 2002 (Federal Law Gazette I p. 1467) zaproponowano specyficzny standard opisany w załączniku A do BITV. zawiera dwa poziomy dostępności, a w ich ramach 14 standardów opisanych bardziej szczegółowo w wymaganiach. Standardy są wspólne dla obu poziomów, a wymagania różne. Wśród wymagań znajdują się także te, które wymagają stosowania formatów publicznie dostępnych i dobrze udokumentowanych (na przykład z W3C).

Specyfikacja jest bardzo szczegółowa i uporządkowana. Z pewnością nie powstydziłaby się jej sama WAI, a dopisanie także wymogów co do otwartości specyfikacji czyni ten dokument jeszcze ciekawszym.

### Unia Europejska

Council Resolution of 25 March 2002 on the eEurope Action Plan 2002: accessibility of public websites and their content (2002/C 86/02)

Rezolucja nie ma charakteru wiążącego, ale wskazuje pożądaną sytuację. Wskazano specyfikację WCAG 1.0 jako tą, którą należy się kierować przy tworzeniu stron internetowych. Polska nie była wówczas członkiem UE, więc akcja ją całkowicie ominęła. Polska zobligowała się do tego samego deklaracją ryską, ale koniec 2010 roku zbliża się wielkimi krokami, a cel nie jest osiągnięty.

### Włochy

Stanca Law (2004)

Provisions to support the access to information technologies for the disabled

W rozporządzeniu określono własny standard, bardziej rozbudowany niż WCAG. Prawo wymaga zgodności także z najnowszymi standardami WAI. Rozporządzenie wskazuje wprost na WCAG 1.0 i Section 508 jako podstawy do zaprojektowania Stanca Law.

Włosi pojechali po bandzie, bo wymogi są wyjątkowo restrykcyjne – strony muszą być zgodne ze Stanca Law, WCAG i Section 508. Wszystkimi naraz. Potoczna nazwa (Stanca Law) pochodzi od nazwiska włoskiego ministra, który przeforsował tą specyfikację. Przetłumaczone na angielskie przepisy dotyczące dostępności zebrano w [tym dokumencie w formacie DOC](http://www.pubbliaccesso.it/normative/Italian_Legislation_on_Accessibility.doc).

### Irlandia.

Irish National IT  
Accessibility Guidelines (2005)

Nie ma uregulowania prawnego, ale zaproponowano własne rozwiązanie niekompatybilne w pełni z WCAG 1.0. Brak prawa stanowionego, które zastępuje się dobrymi praktykami i zaleceniami to dość często spotykane zjawisko w Irlandii. Poniekąd stanowi to element ich umowy społecznej.

### Czechy

Od 1 stycznia 2008 roku wszystkie publiczne serwisy internetowe powinny być zgodne z WCAG 2.0.

### Podsumowanie

Przed Ministerstwem Spraw Wewnętrznych i Administracji, które ma przygotować rozporządzenie, trudna decyzja. Czy napisać własną specyfikację wymagań, czy może po prostu wstawić do tabelki WCAG 2.0 i mieć problem z głowy. Ja jestem za tym pierwszym rozwiązaniem, bo jest elastyczniejsze i nie generuje problemów z prawami autorskimi. Ale gdzie mnie decydować o tak ważnych rzeczach…

Jeszcze apel do Czytelników – gdyby ktoś znalazł jeszcze jakieś ciekawe rozwiązania, to proszę o podesłanie informacji na adres <jacek.zadrozny@post.pl> lub w komentarzach pod tekstem. A ja postaram się w przyszłości (niedalekiej) napisać nieco więcej o konkretnych rozwiązaniach.