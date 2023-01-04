---
id: 456
title: 'Lista sprawdzająca dostępność aplikacji'
date: '2012-12-29T14:33:14+01:00'
layout: post
guid: 'http://informaton.pl/?p=456'
permalink: /2012/12/29/lista-sprawdzajaca-dostepnosc-aplikacji/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - IBM
    - klawiatura
    - kolor
    - kontrast
    - oprogramowanie
    - semantyka
    - specyfikacja
---

Projektując interfejs użytkownika aplikacji warto zwrócić uwagę także na jego dostępbność. Za narzędzie wspomagające może nam posłużyć [lista sprawdzająca dostępność oprogramowania](http://www-03.ibm.com/able/guidelines/software/accesssoftware.html) zaproponowana przez firmę IBM. Jej ogromną zaletą jest zwięzłość i łatwość stosowania. Poniżej opis i krótkie wyjaśnienia ode mnie.

Poniższe zasady można aplikować dla dowolnej technologi służącej tworzeniu interfejsu użytkownika: bibliotek graficznych typu Swing, QT, MFC, ale także tworzonych w technologiach webowych HTML, CSS i ARIA.

### 1. Dostęp za pomocą klawiatury

1.1. Zapewnienie dostępu za pomocą klawiatury do każdej funkcji programu. Każde zadanie możliwe do wykonania za pomocą myszy, dotyku lub innego interfejsu wejściowego powinno być możliwe do realizacji za pomocą klawiatury. Rozwiązanie powinno być możliwie standardowe, a zatem zgodne z założeniami systemu operacyjnego, na przykład przemieszczanie fokusa za pomocą klawisza Tab, aktywowanie za pomocą spacji czy przesuwanie za pomocą kursorów. Nie wyklucza to stosowania skrótów klawiaturowych przyśpieszających pracę.

1.2. Nie wprowadzaj zakłóceń w standardowo stosowanej w systemie obsłudze klawiatury. Każdy system ma pewne standardowe rozwiązania i skróty klawiaturowe, których aplikacja nie powinna zmieniać. Na przykład skrót CTRL+Z standardowo oznacza cofnięcie ostatnio wykonanej operacji i aplikacja nie powinna wprowadzać innej funkcjonalności podpiętej pod ten skrót.

### 2. Informacje o obiektach

2.1. Zapewnij widzialny fokus przemieszczany pomiędzy poszczególnymi elementami interfejsu użytkownika. Fokus powinien być prezentowany technologiom asystującym. Widoczny fokus (punkt uwagi) jest szczególnie istotny w sytuacji, gdy obsługa nie odbywa się za pomocą myszy. Dzięki takiemu fokusowi użytkownik wie, z jakim obiektem będzie się odbywała interakcja. Informacje o miejscu fokusu powinny być dostępne dla technologii asystujących, najczęściej przez interfejsy w rodzaju MSAA, AT-SPI czy UIAutomation.

2.2. Zapewnij semantyczną informację o elementach interfejsu. Jeżeli elementem interfejsu jest grafika, powinna mieć zapewnioną interpretację tekstową. Stosując standardowe kontrolki interfejsu użytkownika wszystkie informacje semantyczne powinny być już zapewnione. Jeżeli jednak projektant przygotuje własne kontrolki, to każda powinna mieć określoną rolę: przycisk, lista, pole edycyjne, tabela, menu, pasek statusu, pole wyboru itp. W ten sposób można poinformować technologie asystujące, w jaki sposób obsłużyć daną kontrolkę.

2.3. Powiąż etykiety z kontrolkami, obiektami, ikonami i grafikami. Jeżeli grafika pełni rolę elementu interfejsu, jej opis powinien przekazywać informacje o jej funkcji. Każda biblioteka graficzna pozwala na przypisanie do kontrolek etykiety tekstowe i ważne jest, by to przypisanie było semantyczne, a nie tylko wizualne. Najczęściej ta właściwość kontrolki ma nazwę LABEL.

2.4. Jeżeli w aplikacji stosowane są elektroniczne formularze, to powinny być przygotowane w sposób umożliwiający użytkownikom technologii asystujących dostęp do informacji, elementów formularzy i funkcji pozwalających na wypełnienie i przesłanie danych, włączając wszystkie polecenia i podpowiedzi. Należy tu szczególnie zwrócić uwagę na formularze przygotowane w technologii innej, niż podstawowa dla aplikacji. W aplikacji można stosować formularze oparte o HTML, a zatem warto skorzystać ze specyfikacji WCAG 2.0.

### 3. Dźwięki i multimedia

3.1. Zapewnij możliwość włączenia wizualnych powiadomień dla wszystkich alarmów dźwiękowych. Dla osób niesłyszących istotne jest, by nie umknęła im żadna informacja. Jeżeli zatem program powiadamia o zdarzeniach (nadejście wiadomości, błąd działania, brak połączenia itp.) za pomocą sygnałów dźwiękowych, to projektant powinien dać możliwość włączenia także powiadomień wizualnych, na przykład ikonek na pasku statusu, wyskakujących okienek itp.

3.2. Zapewnij alternatywę dla istotnych elementów multimedialnych. Jeżeli w aplikacji znajdują się istotne informacyjnie elementy multimedialne (dźwięki, animacje, filmy), to należy zapewnić dla nich treści alternatywne. Nagrania audio należy uzupełnić o podpisy, animacje i filmy o audiodeskrypcję oraz napisy, jeżeli to będzie konieczne.

3.3. Zapewnij możliwość dostosowania głośności. Programy wykorzystujące dźwięk powinny mieć możliwość dostosowania głośności niezależnie od głośności systemowej. Osoby słabosłyszące będą podwyższać poziom głośności, a użytkownicy mowy syntetycznej – obniżać.

### 4. Wyświetlanie

4.1. Zapewnij wyświetlanie tekstu przez wywoływanie standardowych funkcji systemu lub przez API współpracujące z technologiami asystującymi. Przekazywanie tekstu w ten sposób zapewni dostęp do niego technologiom asystującym. Nie należy stosować własnych rozwiązań, na przykład grafik z generowanym w locie tekstem.

4.2. Używaj koloru jako uzupełnienia, a nie podstawowego nośnika informacji lub oznaczenia akcji. Ponieważ duża grupa użytkowników nie widzi kolorów wcale lub częściowo, należy zadbać o przekazanie ważnych informacji w inny sposób. Zmiana koloru ikonki na czerwony może nie zostać zauważona przez użytkownika.

4.3. Wspieraj systemowe ustawienia wysokiego kontrastu dla interfejsu użytkownika i obszaru roboczego. Aplikacja powinna korzystać z ustawień systemowych związanych ze sposobem wyświetlania elementów interfejsu w wysokim kontraście przeznaczonym dla osób słabowidzących.

4.4. Jeżeli aplikacja pozwala na zmianę kolorystyki, należy zapewnić szeroki wybór kolorów tła i czcionek, aby dobrać odpowiedni kontrast. Oznacza to, że zaproponowanie predefiniowanych skórek nie jest wystarczające, jeżeli nie da się oddzielnie ustawiać kolorów dla tła i informacji.

4.5. Dziedzicz ustawienia systemowe dla czcionek, wielkości i kolorów wszystkich elementów interfejsu. Interfejs aplikacji powinien być zgodny z ustawieniami dla całego systemu operacyjnego.

4.6. Zapewnij dla animacji informację w innej postaci. Jeżeli animacja niesie jakąś informację (np. o kopiowaniu plików) to powinna być zapewniona informacja ekwiwalentna (np. tekstowa “pliki są kopiowane”).

### 5. Czas

5.1. Zapewnij opcję dostosowania czasu na reakcję użytkownikaw wypadku działań opartych o czas lub pozwól na wstrzymanie. Przy projektowaniu interakcji trzeba pamiętać, że nie każdy użytkownik jest w stanie odpowiednio szybko zareagować i wykonać odpowiednią operację. Dla tej grupy trzeba zapewnić inne rozwiązania polegające na spowolnieniu upływu czasu lub całkowitego zatrzymania.

5.2. Nie używaj błyskających i migających tekstów, obiektów oraz innych elementów, których częstotliwość jest większa niż 2 Hz i mniejsza niż 50 Hz. To zalecenie ma na celu wyeliminowanie elementów mogących wywołać ataki epileptyczne.