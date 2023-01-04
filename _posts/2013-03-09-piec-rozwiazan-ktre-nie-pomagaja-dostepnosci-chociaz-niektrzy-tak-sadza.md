---
id: 627
title: 'Pięć rozwiązań, które nie pomagają dostępności, chociaż niektórzy tak sądzą'
date: '2013-03-09T10:57:21+01:00'
layout: post
guid: 'http://informaton.pl/?p=627'
permalink: /2013/03/09/piec-rozwiazan-ktre-nie-pomagaja-dostepnosci-chociaz-niektrzy-tak-sadza/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - CAPTCHA
    - IVONA
    - IWR
    - nagłówki
    - 'WCAG 2.0'
---

Mity dotyczące dostępności stron internetowych są różnorodne, a ich pochodzenie jest dla mnie czasem zagadką. Jest jednak kilka, które szczególnie mocno tkwią w świadomości webmasterów i manifestują się stosowaniem złych rozwiązań w serwisach internetowych. Postanowiłem zatem je opisać i wyjaśnić, dlaczego są one mitami, a nie faktami.

## Specjalna wersja serwisu

Webmaster tworzy specjalny serwis internetowy, pozbawiony grafiki, z tekstem wyświetlonym bardzo dużymi czcionkami, w kolorystyce przyprawiającej o palpitację serca internetowych estetów. Do takiego serwisu prowadzi link oznaczony ludzikiem na wózku, znaczkiem WAI, lub po prostu – wersja tekstowa lub wersja dla niepełnosprawnych. Mitem jest to, że z takiego serwisu korzystają niepełnosprawni użytkownicy, szczególnie słabowidzący. To znaczy – czasem korzystają, jeżeli z podstawowego nie da się żadną miarą skorzystać. Jednak zdecydowanie preferują serwis podstawowy, bo ten ma pełną funkcjonalność i aktualne informacje.

Pochodzenie tego mitu jest dla mnie jasne – ktoś zobaczył osobę słabowidzącą korzystającą ze strony z powiększonymi czcionkami i dziwną kolorystyką. Jednak ten użytkownik zastosował swoje własne ustawienia, które dopasował do swoich indywidualnych potrzeb korzystając z możliwości systemu operacyjnego lub przeglądarki. Ustawienia zaproponowane na “specjalnej wersji” serwisu mogą mu zwyczajnie nie odpowiadać. Dlatego serwis należy zaprojektować tak, by wyłączenie stylów, zadeklarowanych kolorów lub zmiana wielkości czcionek była możliwa na **podstawowej** stronie internetowej.

## Duża liczba nagłówków pomaga w nawigacji

Webmaster projektuje serwis internetowy i edytor treści w taki sposób, żeby każdy element dodawany przez redaktora był umieszczony w nagłówku. Od tej pory w nagłówkach są wszystkie akapity, linki nawigacyjne, grafiki i inne elementy są umieszczone w nagłówkach różnego poziomu. Niewidomy użytkownik jest od tej pory bombardowany informacjami o nagłówkach i ich poziomach, aż w końcu zirytowany wyłącza odczyt informacji i przechodzi na inny sposób nawigacji po serwisie internetowym.

Mit ten wziął się prawdopodobnie z obserwacji poczynionych podczas prezentacji prowadzonych przez niewidomych użytkowników Internetu. Pokazywali oni, że do treści da się dojść szybciej, jeżeli jest ona podzielona na logiczne części oznaczone tytułami wstawionymi w nagłówki. I to jest ta prawdziwa część mitu, do której dorobiono legendę, że w takim razie trzeba wszystko włożyć w nagłówki, żeby ułatwić jeszcze bardziej. Zastosuję tu analogię do książki, po której nawiguje się za pomocą spisu treści, w którym znajdują się tytuły rozdziałów z numerami stron. A teraz proszę sobie wyobrazić spis treści, w którym umieszczony jest każdy akapit i numer strony, na której się on znajduje. Funkcjonalność takiego spisu treści jest zerowa.

## Automat odczytujący zawartość strony

Webmaster dokłada do serwisu rozszerzenie, którego zadaniem jest odczytanie treści artykułu. Po kliknięciu w odpowiedni link lub użyciu skrótu klawiaturowego odzywa się syntezator mowy, czytający tekst. Użytkownicy niewidomi **nigdy** z takich rozwiązań nie korzystają. No chyba, że z ciekawości.

Ten mit powstał w wyniku działalności marketingowej firm oferujących takie rozwiązania, a żerującej na niewielkiej wiedzy na temat dostępności. Wystarczy jednak postawić kilka prostych pytań w rodzaju:

- Jak niewidomy użytkownik ma wejść na stronę internetową, jeżeli nie ma swojego własnego oprogramowania czytającego?
- Skąd ma wiedzieć, że akurat dana strona internetowa posiada takie rozszerzenie?
- Jeżeli już ma program do odczytu, to po co ma go wyłączać i włączać wtyczkę na stronie?

Dochodziły do mnie opinie, że z tego rozwiązania mogą korzystać inne osoby, na przykład dyslektycy lub po prostu osoby, którym nie chce się czytać. Nawet jeżeli to prawda, chociaż chętnie poznałbym statystyki, to nie ma to nic wspólnego z dostępnością. Może wręcz wstrzymać pozytywne zmiany w dostępności, bo przecież strona jest “udźwiękowiona”

## Omnipotentny atrybut TITLE

Webmaster skądś wie, że kluczowy dla dostępności jest atrybut TITLE, który jest odczytywany niewidomym użytkownikom. Dlatego umieszcza go we wszystkich elementach nawigacyjnych, w szczególności graficznych, a także w innych elementach, byle jakoś zapewnić tą dostępność. Tymczasem programy odczytu ekranu nie korzystają z tego atrybutu i niewidomy użytkownik nie jest świadomy jego istnienia. W niektórych programach można nawet włączyć jego obsługę, ale domyślnie ta opcja jest wyłączona i wielu użytkowników nie wie o jej istnieniu. Wtyczka [WP Accessibility](http://informaton.pl/?p=588)ma nawet możliwość usuwania tego atrybutu ze skórek WordPressa, żeby w razie czego nie tworzyć nadmiarowej, zupełnie zbędnej informacji.

Pochodzenie tego mitu jest dla mnie nieznane. W żadnej specyfikacji technicznej, tutorialu czy podręczniku nie znalazłem takiego zalecenia. Snując domysły mogę podejrzewać, że może zawiniło tu lenistwo osób, którym nie chciało się doczytać i uznali, że atrybut TITLE, który można aplikować do każdego elementu, wystarczy na zapewnienie informacji tekstowej. W każdym razie jest pewne – nie wystarczy. Do tego służą specjalne elementy, jak na przykład atrybuty ALT i LABEL oraz znacznik LABEL.

## Dźwiękowe kody CAPTCHA

Webmaster czasem musi bronić swojego serwisu internetowego przed złymi programami napisanymi przez złych ludzi. Wymyślono do tego celu zabezpieczenia typu CAPTCHA, czyli najczęściej przepisywanie zamazanych liter z obrazka. Dla podniesienia dostępności i w zgodzie z WCAG 2.0 webmaster wybrał system, który oferuje alternatywę w postaci nagrania dźwiękowego, które niewidomy użytkownik może odsłuchać i przepisać literki. Jednak niewidomi użytkownicy niemal nigdy nie korzystają z tego rozwiązania. Po pierwsze – programy odczytu ekranu generują własne informacje dźwiękowe, które bardzo często nakładają się na już zakłócone nagrania kodów. Po drugie – kody dźwiękowe niezbyt często są skorelowane z językiem użytkownika, co utrudnia lub uniemożliwia ich zrozumienie. Litera “A” jest taka sama dla Polaka i Anglika, ale wymowa tej litery jest już zupełnie inna. Jeszcze gorzej jest z innymi znakami, na przykład cyframi. To trochę tak, jakby kazać przepisywać Polakowi ideogramy chińskie lub litery arabskie. Po trzecie – niewidomi użytkownicy mają inne sposoby na łamanie zabezpieczeń CAPTCHA.

Ten mit pochodzi wprost ze specyfikacji WCAG 2.0, gdzie zaleca się stosowanie zabezpieczeń typu CAPTCHA w kilku wersjach opartych o zmysły, w tym wypadku wzrok i słuch. Osobiście uważam ten zapis WCAG za błędny, a jednocześnie usprawiedliwiający webmasterów, którzy nie chcą poszukać innych rozwiązań. Ja postuluję, by [zrezygnować z tego typu zabezpieczeń w ogóle](http://informaton.pl/?p=143), bo są one zupełnie nieskuteczne.