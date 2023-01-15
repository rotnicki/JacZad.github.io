---
id: 951
title: 'Raport Rzecznika Praw Obywatelskich na temat dostępności publicznych stron internetowych'
date: '2014-01-31T11:00:56+01:00'
layout: post
guid: 'http://informaton.pl/?p=951'
permalink: /2014/01/31/raport-rzecznika-praw-obywatelskich-na-temat-dostepnosci-publicznych-stron-internetowych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - FIRR
    - 'narzędzia KRI'
    - RPO
    - Utilitia
    - walidator
    - 'WCAG 2.0'
---

Rzecznik Praw Obywatelskich, wraz z Fundacją Instytut Rozwoju Regionalnego, wydał [raport pt. “Dostępność witryn internetowych instytucji publicznych”](http://www.brpo.gov.pl/sites/default/files/Biuletyn%20Rzecznika%20Praw%20Obywatelskich%202013%2C%20Nr%209%20%C5%B9r%C3%B3d%C5%82a.pdf) wchodzący w skład serii ?Zasada Równego Traktowania. Prawo i praktyka?. Przeczytałem go uważnie i ma on zarówno zalety, jak i wady, które poniżej postaram się wyłuszczyć.

### Kontekst prawny

Na pochwałę zasługuje rozdział poświęcony kontekstowi prawnemu dostępności serwisów internetowych. Wymieniono bodaj wszystkie istotne akty prawne i mniej znaczące, które zobowiązują podmioty publiczne do publikowania informacji w sposób dostępny. Poruszono nawet aspekt dostępu do informacji publicznej, który faktycznie wiąże się z dostępnością (accessibility) dosyć ściśle. Na pewno ten rozdział będę w przyszłości cytował.

### Błędy merytoryczne

Autorzy nie ustrzegli się jednak błędów merytorycznych, z których najbardziej rzucił mi się w oczy następujący fragment:

> WCAG 2.0 można określić jako zbiór dokumentów opublikowanych przez Web Accessibility Initiative (WAI), skierowanych do budowniczych i administratorów witryn. Zawierają one wytyczne, które pozwalają projektować strony i serwisy internetowe dostępne dla wszystkich osób na zasadzie równości, co oznacza taką architekturę strony internetowej, aby skorzystać z niej mogły także osoby niepełnosprawne, nie używając przy tym dodatkowych urządzeń i aplikacji. (s. 12 pliku PDF)

Nieprawdziwą jest w tym cytacie teza, że strony mogą być zaprojektowane w sposób nie wymagający z technologii asystujących. Co więcej – wytyczna 4.1 nakazuje zbadanie zgodności z tymi technologiami. To może kierować w stronę poszukiwania iWebReaderów i innych rozwiązań stojących z uniwersalnym projektowaniem w sprzeczności. Ja nawet domyślam się, co autor miał na myśli. Podejrzewam, że chodzi o to by dało się odczytywać treści niezależnie od sprzętu i oprogramowania używanego przez osobę niepełnosprawną, ale to jednak jest coś zupełnie innego. Są jeszcze inne błędy, chociaż znacznie mniejszego kalibru. Szkoda, że ten jest taki gruby.

### Metodologia badania

Czytałem ten rozdział kilka razy i za każdym razem wychodziło mi to samo. Autor wyolbrzymiał zalety badania automatycznego i pomijał jego ograniczenia. Z kolei błędnie wskazuje sposób wykonania “klasycznej oceny”, by na jej tle ocena automatyczna wypadała lepiej. Badanie automatyczne jest faktycznie szybkie i powtarzalne, bo oparte jest o algorytmy. Jednak już co do obiektywności można mieć spore wątpliwości. Owszem – jeżeli subiektywnością nazwać brak zewnętrznego wpływania na ocenę, to jest to prawda. Jednak pewnego rodzaju subiektywność wbudowana jest w same algorytmy, w których przyjęto pewne rozwiązania za jedyne słuszne, a z takim postawieniem sprawy nie bardzo daje się dyskutować. Można zatem porównywać dwa audyty wykonane jednym narzędziem na różnych stronach, ale nie można porównywać dwóch audytów wykonanych walidatorem oraz w inny sposób na jednym serwisie.

Pełny audyt polega na wykonaniu trzech elementów: testowania narzędziem automatycznym, analizie eksperckiej i ocenie przez użytkowników. Z oczywistych względów jest to audyt o wiele dokładniejszy, bo walidacja odbywa się w jego ramach. Jeżeli ktoś dokonuje audytu bez narzędzi, to nie jest to żaden audyt dostępności, tylko klikanie po stronach. Z kolei autor bardzo delikatnie wspomina o tym, że automat **nie jest w stanie wykonać pełnego audytu**, a zatem nie pozwala na wnioskowanie o spełnieniu wymagań WCAG 2.0, a jedynie o ewentualnym nie spełnienia tych wymagań. Różnica jest diametralna i szkoda, że o tym ani słowa nie napisano.

### Wyniki badania

Mam poczucie, że cała część ilościowa ma niewielki sens w kontekście ograniczeń narzędzia, o których napisałem wcześniej. Utilitia jest narzędziem dobrym, ale ograniczonym i nie da się na podstawie raportu wnioskować o spełnieniu wymagań WCAG 2.0 na jakimkolwiek poziomie oraz o zgodności z rozporządzeniem Rady Ministrów o Krajowych Ramach Interoperacyjności. Do tego w opisie starannie wymieszano kryteria wymagane (poziom A i AA) z tymi, które nie są wymagane (poziom AAA). Możliwość sprawdzenia tych ostatnich jest cenna, ale powinny one być wyraźnie oddzielone od obowiązkowych. Pisząc tą część w tak ogólny sposób nie opisuje się zgodności z rozporządzeniem o KRI, ale ogólnie o dostępności na różnych poziomach i do tego dosyć wyrywkowo. Wartościowa jest jednak część jakościowa, pokazująca najczęściej pojawiające się błędy i ich skalę.

Jest takie powiedzenie, że jeżeli ktoś chce mieć zrobione coś dobrze, szybko i tanio, to tego się nie da zrobić. Trzeba z jednej z tych rzeczy zrezygnować. Ten raport opisuje jak zrobić coś szybko i tanio, ale na pewno nie dobrze. To jednak nie sprawia, że badanie jest bezwartościowe. Moje uwagi dotyczą jedynie formy jego prezentacji, przekonującej nie obeznanego czytelnika, że walidatorem można zastąpić porządne testy. Gdyby forma była inna, a i zrezygnowano z niemal reklamiarskiego opisywania walidatora, to można byłoby zrobić coś naprawdę cennego. Na przykład wyjąć najczęstsze błędy i opisać je bliżej, ze wskazaniem sposobów ich likwidacji. A tak dostaliśmy materiał na poły merytoryczny, na poły marketingowy.