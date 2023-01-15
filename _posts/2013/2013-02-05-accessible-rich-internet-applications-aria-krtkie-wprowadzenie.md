---
id: 579
title: 'Accessible Rich Internet Applications (ARIA) &#8211; krótkie wprowadzenie'
date: '2013-02-05T15:41:03+01:00'
layout: post
guid: 'http://informaton.pl/?p=579'
permalink: /2013/02/05/accessible-rich-internet-applications-aria-krtkie-wprowadzenie/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - fokus
    - formularze
    - 'HTML 5'
    - niewidomi
---

Zamierzam kontynuować wpisy na temat tworzenia dostępnych interfejsów webowych, ale zdałem sobie sprawę, że do tej pory nie wyjaśniłem pojęcia ARIA. Czas nadrobić tą zaległość i jednocześnie wskazać możliwości i zagrożenia związane z jej stosowaniem. Coraz bardziej przekonuję się, że ARIA, która miała za zadanie zwiększyć dostępność interfejsów, może ją w praktyce zmniejszać. Szczególnie gdy jest źle używana.

## Trochę historii

Język HTML powstał w celu budowania hipertekstowych dokumentów. To znaczy dokumentów, które są ze sobą powiązane i dają możliwość przechodzenia z jednego do drugiego za pomocą aktywnego tekstu, czyli łącza. Specyfikacja HTML przez długi czas była zupełnie wystarczająca, bo dosyć dobrze opisywała semantycznie dokumenty, w tym ich zawartość. Wprowadzono nawet znaczniki INPUT, których celem było tworzenie interfejsów do wprowadzania danych przez użytkowników. Potem te interfejsy zaczęły się coraz bardziej komplikować i przypominać aplikacje instalowane na komputerach. Programiści stosowali mieszanki technologii HTML, JavaScript i CSS. Na początku był to dynamiczny HTML (DHTML), a potem poszło to jeszcze dalej w stronę Ajax, gdzie dodano jeszcze XML oraz mieszanie przetwarzanie na serwerze i w przeglądarce użytkownika. Wszystko po to, by upodobnić sposób działania i wygląd aplikacji webowej do tej na komputerze.

## Okienka w przeglądarce

Specyfikacja HTML nie zawierała w sobie większości z niezbędnych elementów. Nic dziwnego, skoro wymyślono ją do opisywania dokumentów, a nie graficznych interfejsów użytkownika. W [World Wide Web consortium](http://www.w3.org/) dostrzegano ten problem i pracowano nad jego rozwiązaniem. Pierwszym problemem było stworzenie odpowiedniej semantyki dla tego typu elementów, a drugim – ich dostępność. Można było dodawać kolejne znaczniki, na przykład WINDOW, MENU, TREE i w ten sposób wyłatać HTML, ale to byłoby ograniczanie projektantów. Wymyślono zatem coś znacznie bardziej elastycznego – dodano zestaw atrybutów, których zadaniem było deklarowanie ról dla poszczególnych elementów oraz ich właściwości.

Tak więc zamiast nowego znacznika MENUITEM, czyli elementu menu wprowadzono atrybut, który można zastosować do różnych znaczników. Analogicznie – zakładkami w oknie mogą być linki, przyciski lub inne gotowe elementy, dając w ten sposób większą swobodę projektowania. Do tego dodano atrybuty właściwości elementów, z których część powielono w HTML 5. Można zatem przeglądarce wprost powiedzieć, że dany element jest zaznaczony, rozwinięty lub wciśnięty.

## Dostępność w ARIA

Jak sugeruje sama nazwa – [Accessible Rich Internet Applications (ARIA)](http://www.w3.org/TR/wai-aria/) została zaprojektowana przede wszystkim z myślą o dostępności. Te wszystkie role i właściwości – oprócz roli semantycznej – dawały możliwość współpracy z programami odczytu ekranu. Bo to właśnie niewidomi użytkownicy mieli największe kłopoty z zaawansowanymi aplikacjami webowymi. Teraz mogli się dowiedzieć, że dany link jest rozwijanym menu i wchodzić z nim w interakcje analogicznie do menu w oknie aplikacji na komputerze. ARIA stanowiła zatem dodatkowy interfejs pomiędzy stroną internetową i czytnikiem ekranu. Jednak jej użyteczność zaczęła zależeć od kolejnego czynnika. Można wylistować teraz następujące:

1. Strona internetowa wykorzystująca ARIA.
2. Przeglądarka internetowa interpretująca elementy ARIA.
3. Interfejs dostępnościowy wykorzystujący przeglądarkę.
4. Czytnik ekranu interpretujący ARIA.
5. Użytkownik potrafiący korzystać z dynamicznych elementów.

Najtrudniejsze jest to, by spotkały się przeglądarka i czytnik ekranu interpretujące ARIA. Jeżeli jeden z elementów tego nie potrafi, to drugi nie ma z czego korzystać. Na szczęście większość najpopularniejszych przeglądarek już sobie radzi, a otwartoźródłowy [NVDA](http://nvda-project.org) także nadąża. Użytkownicy także zaczynają posługiwać się dynamicznymi elementami, a zatem największe wyzwanie stoi przed programistami, by tworzyli interfejsy w sposób prawidłowy.

## ARIA – szanse i zagrożenia

Stosowanie ARIA daje ogromne możliwości prezentowania nowoczesnych interfejsów użytkownika, które będą jednocześnie dostępne dla niewidomych użytkowników. Można budować rozwijalne menu, drzewa, aktywne formularze i wiele innych obiektów, które będą się prawidłowo komunikować z użytkownikiem. To jest ogromna szansa. Po drugiej stronie jest zagrożenie, bo źle przygotowane interfejsy będą znacznie mniej dostępne, niż przygotowywane w DHTML. Elementy wykorzystujące ARIA i pewne elementy HTML 5 zmieniają bowiem sposób komunikacji czytnika ekranu z przeglądarką. Zamiast tworzenia własnego bufora z treścią, czytnik ekranu przekazuje część kompetencji komunikacyjnych do przeglądarki. To rozwiązanie działa bardzo dobrze, gdy elementy są przygotowane prawidłowo. Jeżeli jednak zrobione są niestarannie lub wręcz wbrew zasadom – obniżają dostępność interfejsu.

Za przykład niech nam posłuży proste okno dialogowe, w którym system zadaje proste pytanie w rodzaju “Czy jesteś pewien, że chcesz usunąć tego użytkownika?” Do tego mamy dwa przyciski “tak” i “nie”. W standardowym HTML nie ma żadnego problemu, bo użytkownik ma dostęp do treści komunikatu oraz obu przycisków. W momencie użycia roli “window” sterowanie komunikacją przekazywane jest do przeglądarki przez interfejs ARIA. Przyciski są elementami aktywnymi, które przechwytują fokus, więc są na pewno dostępne. Jednak treść komunikatu jest elementem nieaktywnym, a zatem fokus nigdy do niego nie trafi. Użytkownik może do woli przemieszczać fokus za pomocą klawiatury i nigdy tam nie trafi. Projektant musi przewidzieć taką sytuację i zastosować mechanizm anonsujący treść komunikatu (pytania), żeby użytkownik nie musiał zgadywać. Stosowanie ARIA musi być kompleksowe, aby było skuteczne.

Wadliwe stosowanie ARIA jest coraz powszechniejsze. Zdarza się przy tym nawet największym graczom na rynku, jak Facebook, google czy Microsoft. A ponieważ to właśnie u nich programiści podglądają nowe rozwiązania, to przejmują te złe nawyki. Przestrzegam zatem przed bezrefleksyjnym kopiowaniem fragmentów kodu, bo nawet najlepszym zdarzają się poważne błędy.