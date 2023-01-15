---
id: 687
title: 'Web Content Accessibility Guidelines (WCAG) 2.0 &#8211; zasady i wytyczne nieco inaczej'
date: '2013-04-29T10:15:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=687'
permalink: /2013/04/29/web-content-accessibility-guidelines-wcag-2-0-zasady-i-wytyczne-nieco-inaczej/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - TL-DR
    - 'WCAG 2.0'
---

Korzystać z WCAG 2.0 można w sposób mechaniczny, stosując listy sprawdzające i techniki zapisane w różnych dokumentach. Wydaje się jednak, że skuteczniejsze będzie zrozumienie celu, któremu służy ta specyfikacja, czyli udostępnieniu informacji użytkownikom z różnymi niepełnosprawnościami. A sposób myślenia odzwierciedlony jest w strukturze WCAG 2.0 i ten właśnie tok myślenia postaram się poniżej przedstawić. Mam nadzieję, że pozwoli on lepiej zrozumieć, a w konsekwencji stosować, zapisy wytycznych.

WCAG 2.0 oparte są o cztery zasady, w ramach których zawarto 12 wytycznych. Każdą z wytycznych można realizować poprzez spełnienie kryteriów sukcesu, które przyporządkowane są do trzech poziomów dostępności. W tym momencie zajmiemy się jednak tylko zasadami i wytycznymi.

## Zasada 1: postrzegalność

Informację dostępną w Internecie odbieramy za pomocą zmysłów. Chociaż mamy takich zmysłów do dyspozycji aż pięć (wzrok, słuch, węch, smak i dotyk), to przy konsumpcji treści w Internecie korzystamy tylko z dwóch pierwszych. Autorzy WCAG zwracają uwagę na fakt, że nie wszyscy użytkownicy informację mogą zobaczyć lub usłyszeć i dla nich trzeba podać ją w inny sposób. Jest to zatem zasada dotycząca głównie użytkowników z niepełnosprawnością wzroku i słuchu.

### Wytyczna 1.1: tekst alternatywny

W dawnych czasach, gdy Internet był narzędziem naukowców i wojskowych, to znaczy na początku lat dziewięćdziesiątych, obecny był w nim tylko tekst. Potem zaczęły pojawiać się grafiki, filmy, animacje, aplikacje, mapy i inne obiekty, które tekstem nie były. Wszystkie były oparte o odbiór wzrokowy oraz słuchowy, a nie nadawały się do przetworzenia przez technologie asystujące. Taki element był po prostu niewidzialny dla osób niewidomych lub niesłyszalny dla osób głuchych. Aby tą sytuację zmienić trzeba zrobić prostą rzecz – przypisać do takiego obiektu tekst, który go opisuje. W ten sposób jego obecność nie umknie użytkownikom niepełnosprawnym sensorycznie, bo można go odczytać wzrokiem (osoby niesłyszące) i słuchem (synteza mowy) lub dotykiem (alfabet brajla).

### Wytyczna 1.2: multimedia

Tekst alternatywny nie sprawdzi się w wypadku mediów zmiennych w czasie, na przykład filmów, animacji, podcastów. Tekst alternatywny trzeba im przypisać, żeby przekazać krótką informację o ich zawartości, ale dla pełnej dostępności trzeba użyć innych technik. Filmy i nagrania audio mają określony czas trwania, zmieniają się w czasie, a zatem stały tekst alternatywny nie sprawdzi się w pełni. Trzeba zastosować audiodeskrypcję (dla osób nie widzących) i napisy (dla osób nie słyszących). Dla tej drugiej grupy można zastosować także tłumaczenia na język migowy.

### Wytyczna 1.3: adaptowalność

Informację elektroniczną często poddaje się przekształceniu, na przykład konwersji na inne formaty, drukuje, wyświetla w różnych warunkach i na różnych urządzeniach. Szczególnym przypadkiem jest przetwarzanie przez technologie asystujące, czyli pośredniczące pomiędzy informacją i niepełnosprawnym użytkownikiem. Informacja powinna być skonstruowana w sposób, który uniemożliwi lub ograniczy utratę istotnych informacji. Najczęściej oznacza to tworzenie informacji w sposób semantyczny, a nie wizualny oraz unikanie przekazywania informacji wyłącznie za pomocą zmysłów wzroku i słuchu.

### Wytyczna 1.4: rozróżnialność

Informacji zazwyczaj towarzyszy jakieś tło. Tekst wyświetlany jest na tle w jakimś kolorze lub nawet grafice, a nagrania wypowiedzi na tle dźwiękowym. Dla informacji takie tło jest szumem, które zakłóca odbiór. Czasem to zakłócenie jest na tyle duże, że do samej informacji trudno jest dotrzeć. Ta wytyczna opisuje, jak tworzyć informację, którą da się łatwo oddzielić od szumu.

## Zasada 2: funkcjonalność

O ile zasada pierwsza mówiła o biernym odbieraniu informacji, to zasada druga dotyczy interakcji użytkownika z informacją. Różni użytkownicy w różny sposób wchodzą w taką interakcję, a osoby niepełnosprawne mogą mieć specyficzne potrzeby w tym zakresie

### Wytyczna 2.1: klawiatura

Uzależnienie korzystania z interfejsu od możliwości wskazywania obiektów kursorem myszy jest poważnym ograniczeniem dla osób z różnymi rodzajami niepełnosprawności. Niektóre osoby niesprawne ruchowo muszą korzystać z klawiatury, bo nie są w stanie używać myszy lub trackballa. Niewidomi użytkownicy także korzystają z klawiatury, bo nie są w stanie skoordynować ruchu kursora z ruchami ręki. Są jeszcze inne grupy użytkowników, które chcą lub muszą korzystać z klawiatury, a nagminnie zdarza się, że z jakiejś funkcji można skorzystać tylko poprzez kliknięcie myszą.

### Wytyczna 2.2: wystarczający czas

Niepełnosprawni użytkownicy Internetu często pracują wolniej, niż ci bez niepełnosprawności. Niewidomi muszą w sposób sekwencyjny zapoznać się z treścią, a nie są w stanie przeskanować strony i od razu odnaleźć interesującej informacji lub funkcji. Osoby słabowidzące mają dostęp do niewielkiej części informacji, bo powiększają sobie obraz. Poza tym muszą się wczytywać w informacje, co również trwa dosyć długo. Osoby niesprawne manualnie muszą wykazać się cierpliwością przy nawigowaniu myszą lub klawiaturą, a użytkownicy mający problemy z rozumieniem treści muszą być bardziej skupieni i kilkukrotnie odczytać informacje. Dlatego potrzebują więcej czasu i powinni więcej czasu dostać, by bez stresu i irytacji móc korzystać z sieci.

### Wytyczna 2.3: ataki padaczki

Padaczka (epilepsja) jest chorobą neurologiczną, a ataki mogą być wywoływane przez nadstymulację wzrokową. Migotanie obrazu, czerwone rozbłyski, falowanie obrazu – to wszystko może wywołać atak, który jest nie tylko bardzo nieprzyjemny, ale może też być groźny dla zdrowia i życia.

### Wytyczna 2.4: nawigacja

System nawigacji powinien być przejrzysty, prosty i zrozumiały dla użytkowników. To są banały, które należy wciąż powtarzać, bo prawie nikt ich nie realizuje. Można powiedzieć, że ta wytyczna ma wiele wspólnego z użytecznością (ang. usability), którą wzbogacono o rozwiązania przydatne osobom niepełnosprawnym.

## Zasada 3: zrozumiałość

Trzecia zasada dotyczy tworzenia treści, interfejsów i usług, które są zrozumiałe dla użytkownika. Ta zrozumiałość musi czasem być wspierana dodatkowo dla osób z problemami poznawczymi, ale służy wszystkim użytkownikom sieci.

### Wytyczna 3.1: czytelność

Wytyczna ta dotyczy stosowanego na stronach internetowych języka. Języków jest mnóstwo, a i stosowane w nich sposoby komunikacji są różnorodne. Język powinien być zatem jasno zdefiniowany, prosty, dodatkowo wyjaśniany w trudniejszych miejscach. Po prostu musi być zrozumiały dla odbiorcy.

### Wytyczna 3.2: przewidywalność

Użytkownik powinien rozumieć nie tylko treść, ale także sposób działania serwisu internetowego. Bardzo kłopotliwe są zachowania w rodzaju otwierających się bez uprzedzenia nowych okien, nowych zakładek, czy też zewnętrznych aplikacji. Dotyczy to w szczególności osób, które tego faktu mogą nie zauważyć (niewidzący i słabowidzący) lub nie zrozumieć (osoby mało doświadczone i z problemami poznawczymi). Poważnym problemem mogą być także interaktywne formularze, których treść zmienia się często bez wiedzy użytkownika po zaznaczeniu opcji lub wpisaniu wartości. Trzeba pamiętać, że osoby niesprawne wzrokowo mają dostęp tylko do wycinka informacji, w którym akurat ta zmiana może się nie zamanifestować.

### Wytyczna 3.3: pomoc

Najwięcej interakcji pomiędzy użytkownikiem i serwisem internetowym zachodzi w sytuacji, gdy wprowadza on jakieś dane. Dlatego ze szczególną uwagą należy podejść do udzielania mu wszelkiej pomocy w takich sytuacjach, co sprowadza się do udzielania instrukcji, nadawania odpowiednich etykiet, pomocy w unikaniu błędów oraz możliwości wycofania źle wprowadzonych danych. Spełnienie tej wytycznej będzie z pożytkiem dla wszystkich użytkowników, nie tylko niepełnosprawnych.

## Zasada 4: solidność

Ostatnia zasada dotyczy solidności i rzetelności technicznej, której wymaga się od twórców treści i interfejsów. Tego samego wymaga się od innych fachowców, na przykład hydraulików, prawników i dziennikarzy. Serwis internetowy nie może po prostu jakoś wyglądać i jakoś się wyświetlać w przeglądarce. Musi być tworzony w zgodzie ze standardami technicznymi i z uwzględnieniem aktualnych możliwości technologii asystujących.

### Wytyczna 4.1: kompatybilność

Na tą wytyczną składają się dwa elementy: zgodność stosowanej technologii z oficjalnymi standardami i precyzyjne opisanie interfejsu użytkownika. Pierwszy oznacza po prostu parsowalność źródła, czyli czynność wykonywaną automatycznie przez walidatory kodu. Drugi jest bardziej skomplikowany, bo wymaga nadawania elementom interfejsu ról, nazw i wartości. Wszystko to po to, żeby technologie asystujące mogły prawidłowo z takim interfejsem współpracować. Czasem przycisk widziany przez człowieka nie jest interpretowany jako przycisk przez te technologie i trzeba im to powiedzieć wprost, podobnie jak dać dostęp do jego stanu lub wartości.

Do czterech podstawowych zasad dostępności można też podejść od innej strony. Pierwsza dotyczy osób niepełnosprawnych sensorycznie, druga – manualnie, trzecia – poznawczo, a czwarta dotyczy technologii asystujących. I chociaż w obu podejściach można znaleźć luki, to powinny one rozjaśnić ten skomplikowany dokument, jakim jest WCAG 2.0