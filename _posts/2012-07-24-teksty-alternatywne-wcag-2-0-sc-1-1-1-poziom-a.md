---
id: 19
title: 'Teksty alternatywne (WCAG 2.0 SC 1.1.1, poziom A)'
date: '2012-07-24T13:09:27+02:00'
layout: post
guid: 'http://informaton.pl/?p=19'
permalink: /2012/07/24/teksty-alternatywne-wcag-2-0-sc-1-1-1-poziom-a/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - CAPTCHA
    - grafika
    - multimedia
    - 'tekst alternatywny'
---

Chociaż serwisy internetowe są bardzo multimedialne, to jednak tekst stanowi ich bardzo ważny element. Poniżej opis kryterium sukcesu 1.1.1, którego spełnienie jest niezbędne dla uzyskania poziomu A dostępności.

<div id="extendedEntryBreak"></div>Każda treść nie będąca tekstem powinna być uzupełniona o informację tekstową. Do takich treści nietekstowych należą obrazy, dźwięki, filmy, animacje, aplikacje i podobne elementy. Dzięki tekstowi alternatywnemu, użytkownik korzystający w alternatywny sposób z serwisu internetowego może mieć pełny dostęp do jego treści. Skorzystają z tego:

- osoby niewidome;
- osoby słabowidzące;
- użytkownicy przeglądarek mobilnych;
- użytkownicy przeglądarek tekstowych;
- użytkownicy łącz o niskiej przepustowości;
- roboty internetowe, na przykład wyszukiwarki;
- właściciel serwisu, który będzie się lepiej indeksował.

Jak widać – beneficjentów tekstów alternatywnych jest dużo, więc dziwi mocno, że tak często ich brakuje. Na podstawie WCAG 2.0 oczekiwać należy dostarczania tekstów alternatywnych do każdej treści, chociaż czynione są pewne wyjątki.

Każda treść nietekstowa powinna posiadać tekst alternatywny, który stanowi ekwiwalent informacji wizualnej lub dźwiękowej. Tekst alternatywny dla obrazu musi informować użytkownika o tym, co przedstawia, a nie jedynie komentować. Bardzo powszechnym błędem jest wstawianie podpisu do fotografii w miejsce opisu alternatywnego. Osoba układająca podpis do obrazu zazwyczaj zakłada, że użytkownik go zobaczy, więc podpis ma za zadanie jedynie go skomentować. Tymczasem opis alternatywny ma za zadanie **opisać** treść obrazu. W ten sposób nawet osoba, która go nie zobaczy, będzie miała informację o tym, co przedstawia.

Dobrym przykładem może być odnaleziony kiedyś na stronach Prezydenta RP fotos, którego opis alternatywny ograniczył się właśnie do skopiowania podpisu o treści "Najważniejsze osoby w państwie podczas wręczania odznaczeń w Belwederze". Jeżeli użytkownik nie zobaczy obrazu, to nadal nie będzie wiedział, kogo przedstawia fotografia, chociaż dowie się o miejscu i sytuacji. Prawidłowo skonstruowany opis alternatywny powinien zawierać informacje kluczowe, w tym wypadku stanowiska i nazwiska osób widocznych na fotografii, wraz z informacją o tym, że wszystko to dzieje się w Belwederze podczas wręczania odznaczeń.

Każdy może przeprowadzić prosty test, wyłączając w swojej przeglądarce wyświetlanie grafiki. Wiele serwisów będzie po tej informacji wyglądało ubogo graficznie, ale co gorsza – będą o wiele mniej użyteczne.

1. Poniżej sześć wyjątków od zasady ogólnej, nakazującej dostarczanie ekwiwalentnego tekstu alternatywnego. Jeżeli treść nietekstowa (najczęściej obraz) jest elementem aktywnym, a w szczególności elementem formularza, to tekst alternatywny powinien informować o funkcji, zamiast o wyglądzie. Zatem jeżeli przyciskiem do wysłania wiadomości jest obrazek z kopertą, to opis alternatywny powinien brzmieć raczej "wyślij", a nie "koperta". Analogicznie – jeżeli mamy na stronie kilka flag narodowych pozwalających na wybranie języka interfejsu, to lepiej polską flagę opisać "język polski" niż "flaga Polski" lub "flaga biało-czerwona".
2. W wypadku multimediów w rodzaju nagrań audio, filmów i animacji, tekst alternatywny ma za zadanie jedynie opisać ogólnie, co znajduje się w tym zasobie. Nie oznacza to oczywiście, że to już wystarczy, ale takie multimedia udostępnia się zazwyczaj inaczej. Należy zatem dostarczyć krótki opis, dzięki któremu użytkownik będzie miał możliwość oceny, czy dane multimedia go interesują, czy też nie. Wystarczy na przykład "film instruktażowy na temat instalacji WordPressa", "Nagranie wykładu o logice rozmytej" czy "screencast na temat korzystania z Bloggera".
3. Poważny problem powstaje, gdy obiekty nietekstowe stanowią podstawę testu lub ćwiczenia. Umieszczenie tekstu alternatywnego w tym wypadku mogłoby prowadzić do sytuacji absurdalnej. Zatem należy tworzyć opis w taki sposób, by – w miarę możności – dostarczyć informację tekstową, a nie zaburzyć testu. Jeżeli zatem zadaniem jest wskazanie francuskiej flagi, to ten obraz nie może mieć opisu "flaga francuska". Dopuszczalne może być opisanie "flaga numer 1", ale lepszym pomysłem byłoby "flaga składająca się z trzech pionowych pasów w kolorach niebieskim, białym i czerwonym". W tym ostatnim wypadku nawet użytkownik niewidomy będzie mógł zdać taki test.
4. Czasem jako informacji używa się obrazów, które mają jedynie oddziaływać na zmysły, a nie dostarczać konkretnej informacji. Tak jest w wypadku graficznych punktorów poprzedzających elementy listy. W takiej sytuacji nie ma oczywiście sensu opisywać ich kształtu czy koloru, bo ich jedyną funkcją jest wyróżnienie , a zatem opis w tym wypadku może brzmieć na przykład "bullet" lub "punktor". Nie należy za to stosować opisów typu "czarne kółko z czerwoną obwódką" lub "pięcioramienna gwiazdka".
5. Kolejnym wyjątkiem od obowiązku tworzenia precyzyjnego opisu alternatywnego są kody obrazkowe CAPTCHA. Podobnie, jak w wypadku obrazków w testach, umieszczenie takiego opisu spowodowałoby bezsensowność tego mechanizmu. W takim wypadku opis powinien się ograniczać do czegoś w rodzaju "kod obrazkowy", ale niezbędne jest zapewnienie alternatywnego sposobu przejścia zabezpieczenia. Warto przy tym dodać, że tzw. kody dźwiękowe nie spełniają tego wymogu, ponieważ nie zapewniają odpowiedniego oddzielenia informacji od szumu. Generalnie najlepiej jest rezygnować z tego typu zabezpieczeń w ogóle.
6. Wreszcie ostatni wyjątek, który obejmuje wszelkiego rodzaju ozdobniki graficzne i multimedialne. Paski, narożniki, i podobne elementy występujące na stronach internetowych nie powinny posiadać tekstów alternatywnych. Ich odczytywanie poważnie utrudniałoby pracę użytkownikom niewidomym i stanowiłoby problem dla robotów sieciowych. Jednak przejście przez proces walidacji wymaga, by stosować niezbędne techniki, w tym puste opisy alternatywne.
