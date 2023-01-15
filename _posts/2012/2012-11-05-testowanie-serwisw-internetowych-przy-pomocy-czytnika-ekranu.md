---
id: 352
title: 'Testowanie serwisów internetowych przy pomocy czytnika ekranu'
date: '2012-11-05T18:01:52+01:00'
layout: post
guid: 'http://informaton.pl/?p=352'
permalink: /2012/11/05/testowanie-serwisw-internetowych-przy-pomocy-czytnika-ekranu/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - formularze
    - grafika
    - klawiatura
    - narzędzia
    - niewidomi
---

Jednym z najczęściej pojawiających się pytań podczas szkoleń, jakie prowadzę jest – jak sprawdzić, czy moja strona jest dostępna? Na takie pytanie trudno jest odpowiedzieć w prosty sposób, chyba że po prostu zasugeruję oddanie tego zadania specjalistom. Jednak kilka rzeczy można sprawdzić samemu, by mieć przynajmniej ogólny ogląd. Dzisiaj kilka rad, jak wykorzystać do tego celu czytnik ekranu.

### Czytnik ekranu

Czytnik ekranu to program używany przez osoby niewidome do korzystania z komputera. Jego zadaniem jest interpretowanie informacji prezentowanej na ekranie komputera i przesyłanie jej do urządzenia wyjściowego, którym może być syntezator mowy lub monitor brajlowski. Na potrzeby testu wykorzystamy bezpłatny program o otwartym źródle o nazwie [NVDA](http://nvda-project.org), który jest wyposażony w bezpłatny i otwartoźródłowy syntezator mowy [Espeak](http://espeak.sourceforge.net). Syntezatora nie trzeba pobierać oddzielnie, bo zawarty jest już w samym programie NVDA. Stabilne wersje NVDA są spolszczone i Espeak także mówi po polsku, chociaż trzeba się do tego trochę przyzwyczaić. Zatem pierwszym zadaniem testera jest pobranie instalatora NVDA i zainstalowanie lub utworzenie wersji przenośnej. Program działa na każdej wersji systemu Windows od XP w górę, chociaż Windows 8 nie jest jeszcze oficjalnie wspierany.

### Przeglądarka internetowa

Drugim niezbędnym elementem jest przeglądarka internetowa. Ja polecam użycie przeglądarki [Mozilla Firefox](http://www.mozilla.org/pl/firefox/new/). Przeglądarki nie trzeba uzupełniać o rozszerzenia i wtyczki, a w szczególności nie należy instalować takich, które ingerują w wygląd lub kod wyświetlanych stron. Najlepiej, jeżeli przeglądarka nie będzie miała żadnych rozszerzeń.

### Przygotowanie do testu

Pierwszą rzeczą, którą warto zrobić jest odłączenie myszy oraz touchpada. Podczas testów można się posługiwać wyłącznie klawiaturą. Teraz trzeba uruchomić program NVDA, co zrobimy skrótem CTRL + ALT + n, czyli takim, którym wpisujemy zazwyczaj literę “ń”. Ten skrót został domyślnie wybrany podczas instalacji i można go zmienić edytując właściwości ikony NVDA na pulpicie. Po uruchomieniu NVDA pojawia się okienko, w którym zaznaczamy opcję by klawisz CapsLock służył nam za klawisz NVDA i jesteśmy gotowi do dalszej pracy.

### Wczytanie strony

Teraz uruchamiamy Firefoksa i wpisujemy adres strony, którą będziemy testować.Ponieważ nie mamy myszy, robimy to klawiaturą: Ctrl – l lub F6. Strona powinna się wczytaćdo przeglądarki, a punkt uwagi przenieść do jej treści.

### Tryb przeglądania

Programy do odczytu ekranu pracują w sposób odmienny od oczekiwań, a widoczne jest to szczególnie podczas pracy z przeglądarką. Zawartość strony przetwarzana jest przez program i tworzony jest jej obraz, który umieszczany jest w buforze. Po zawartości strony przemieszczamy się za pomocą kursorów strzałek góra i dół, a program odczytuje nam porcje informacji, które czasem są zbieżne z obrazem wyświetlanym na ekranie, a czasem nie. Kursory strzałek w lewo i prawo pozwalają na przemieszczanie się pomiędzy najmniejszymi porcjami informacji, na przykład literami. Program informuje użytkownika o typie elementu, który właśnie odczytuje, na przykład “nagłówek”, “link” czy “tabela”. Już po chwili można się zorientować, że dostęp do zawartości strony jest sekwencyjny. Można go nieco przyśpieszyć używając klawisza Tab, który przesuwa punkt uwagi pomiędzy elementami aktywnymi, to znaczy linkami lub elementami formularzy. Do wcześniejszych elementów można dotrzeć używając skrótu Shift + Tab. Tutaj można sprawdzić pierwszy element dostępności: czy punkt uwagi (fokus) jest zawsze widoczny. Można też sprawdzić drugi element – czy do każdego elementu interfejsu da się dotrzeć za pomocą klawiatury i czy punkt uwagi nie blokuje sięę na którymś z elementów.

### Skróty wspomagające nawigację po stronach

W trybie przeglądania możemy posługiwać się wieloma skrótami, które służą przede wszystkim do odnajdowania elementów określonego rodzaju. W tym celu wystarczy nacisnąć pojedynczy klawisz, a program przeniesie punkt zainteresowania na kolejny element danego rodzaju lub poinformuje o braku takich obiektów. W drugą stronę, to znaczy w kierunku początku strony, przemieszczać się można za pomocą tych samych skrótów z jednoczesnym naciśnięciem klawisza Shift. Poniżej wykaz kilku najważniejszych skrótów:

- G – grafiki umieszczone na stronie,
- L – listy,
- K – linki,
- H – nagłówki,
- X – pola wyboru,
- E – pola edycyjne,
- C – pola list w formularzach,
- B – przyciski.

Skrótów jest więcej i można je znaleźć w pomocy do NVDA. Pojawia się w tym momencie pytanie, jak można w takim razie wpisać jakiś tekst, skoro litery są używane do nawigowania? Tutaj ujawnia się właśnie różnica w korzystaniu ze stron internetowych za pomocą czytników ekranu. Trzeba bowiem przejść w tryb formularzy, do czego służy skrót Ctrl + Spacja.

### Tryb formularzy

W trybie formularzy strona internetowa zachowuje się jak okno aplikacji, na przykład dialogowe. Klawiszem Tab przemieszczamy się pomiędzy elementami interfejsu – łączami i kontrolkami formularzy. Nie mamy dostępu do każdej treści na stronie, a jedynie do aktywnych elementów. W tym momencie możemy się dowiedzieć, czy elementy formularzy mają prawidłowe etykiety i czy są one prawidłowo połączone z kontrolkami. Nawigując za pomocą klawisza Tab po elementach formularza usłyszymy komunikaty opisujące rodzaj kontrolki, jej etykietę i ewentualnie stan lub wartość. Na przykład coś w rodzaju “Format HTML, pole wyboru, nie zaznaczone”. za pomocą spacji można takie pole zaznaczyć, a program poinformuje “pole zaznaczone”. Jeżeli jednak mamy informację jedynie o rodzaju kontrolki i jej stanie, to znaczy że etykieta jest błędnie przypisana lub nie ma jej wcale.

### Elementy superaktywne

Prawdziwym wyzwaniem jest przetestowanie elementów oprogramowanych za pomocą JavaScriptu lub wręcz w technologii Ajax. Różnego rodzaju rozwijalne menu czy aktywne formularze mogą zachowywać się wyjątkowo dziwnie w kontakcie z programem odczytu ekranu. Przy testowaniu trzeba sprawdzić, czy da się za pomocą klawiatury do nich dotrzeć i czy użytkownik otrzymuje odpowiednią informację o ich funkcjonalnościach. Jeżeli w serwisie znajduje się jakiś zaawansowany formularz, na przykład rejestracyjny, to może posłużyć za poligon doświadczalny. Na szczególną uwagę zasługują listy wyboru, które uruchamiają jakieś akcje związane z formularzem, na przykład zmianę innych elementów.

### Zastrzeżenie

Przeglądania stron za pomocą programu do odczytu ekranu nie można uznać za pełny test dostępności strony, chociaż może być elementem bardzo ważnym. Pokazuje bowiem najpoważniejsze problemy z serwisem, na przykład brak możliwości korzystania z klawiatury czy źle poetykietowane elementy formularzy czy grafiki. Z pewną ostrożnością można powiedzieć, że jeżeli serwis przejdzie pozytywnie test za pomocą NVDA, to serwis jest z grubsza dostępny dla osób niewidomych. To jest jednak tylko jedna z wielu grup odbiorców, chociaż napotykająca na najwięcej problemów. Zachęcam także do dokonywania dotacji dla twórców NVDA, bo każde 10 dolarów przekazane na rozwój tego rewelacyjnego programu, to krok w stronę większego uczestniczenia osób niewidomych w społeczeństwie cyfrowym.