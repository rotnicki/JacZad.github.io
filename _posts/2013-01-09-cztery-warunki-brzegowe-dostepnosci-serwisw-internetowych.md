---
id: 491
title: 'Cztery warunki brzegowe dostępności serwisów internetowych'
date: '2013-01-09T12:53:39+01:00'
layout: post
guid: 'http://informaton.pl/?p=491'
permalink: /2013/01/09/cztery-warunki-brzegowe-dostepnosci-serwisw-internetowych/
restapi_import_id:
    - 5ca8405547793
geo_public:
    - '0'
amp_status:
    - enabled
categories:
    - artykuły
tags:
    - czas
    - dźwięk
    - epilepsja
    - fokus
    - klawiatura
---

Stwierdzenie zgodności serwisu z wymaganiami WCAG 2.0 na konkretnym poziomie wymaga zbadania spełnienia **wszystkich** kryteriów sukcesu dla danego poziomu. Są jednak cztery kryteria sukcesu, od których warto zacząć badanie dostępności, ponieważ brak ich spełnienia czyni bezsensownym dalsze badania. Po prostu występowanie tego typu zakłóceń uniemożliwia korzystanie z serwisu. Można przyjąć, że jest to zerowy poziom dostępności.

Dobór tych krytycznych elementów może nieco dziwić, ale po zastanowieniu wydaje się być dosyć sensownym. Oparty jest o przesłankę, że brak spełnienia pewnych warunków może uniemożliwić dotarcie do jakiejkolwiek treści w serwisie, więc dalsze badanie jest zbędne. Tak jak zbędne jest badanie przejezdności autostrad na Księżycu, gdyby nawet były, bo przecież nikt nie będzie po nich jeździł.

## Kontrola nad dźwiękiem

Pierwszym z warunków brzegowych jest spełnienie [SC 1.4.2](http://informaton.pl/?p=123), który dotyczy dźwięku odtwarzanego na stronie w sposób automatyczny. Nie jest to praktyka powszechna, ale zdarza się, że projektant umyśli sobie podkład dźwiękowy mający umilić czas użytkownikowi. Takie rozwiązanie sprawia, że użytkownicy syntezatorów mowy są odcięci od informacji, która jest zagłuszana przez dźwięk emitowany ze strony internetowej. Częściej się zdarza, że takie efekty są generowane przez reklamy w postaci wideoklipów, trwających zazwyczaj około pół minuty, co opisałem kiedyś w [notatce o panu Komorowskim i Seacie](http://informaton.pl/?p=126). WCAG 2.0 dopuszcza dźwięki trwające do trzech sekund, a nawet dłuższe, pod warunkiem zapewnienia mechanizmu do wyciszania lub regulowania głośności niezależnie od głośności systemowej. Jednak generalnie należy takich rozwiązań raczej unikać w ogóle.

## Pułapka na klawiaturę

Drugim warunkiem brzegowym jest [SC 2.1.2](http://informaton.pl/?p=188), który zabrania tworzenia pułapek na klawiaturę. W skrócie chodzi o to, że jeżeli do jakiegoś elementu da się dotrzeć za pomocą klawiatury i taki element uzyska fokus, to taki element można także opuścić za pomocą klawiatury. Istnienie takiej pułapki sprawia, że użytkownik nie jest w stanie zapoznać się z pełną treścią strony, bo w pewnym momencie zostaje zablokowany i nie może nawigować dalej. Może się wydawać dziwne, że takie sytuacje się zdarzają, ale potwierdzam – niektóre kontrolki formularzy potrafią uwięzić fokus i nie da się go przesunąć do następnego lub poprzedniego elementu. Fokus przesuwany jest za pomocą klawisza Tab oraz niekiedy klawiszami strzałek. Można sprawdzić zgodność z tym warunkiem posługując się klawiaturą do wykonania wszystkich możliwych operacji w obrębie interfejsu nawigacji i formularzy. Jednak nie da się tego sprawdzić używając screen readera, bo ten operuje nie na samej stronie, ale na informacjach odpowiednio przetworzonych w buforze. Może się zatem zdarzyć, że pułapka będziezastawiona tylko na użytkowników nie korzystających z czytnika ekranu.

## Migotanie wywołujące ataki epileptyczne

Trzecim warunkiem brzegowym jest brak migotania i rozbłysków, jak to zostało opisane w [SC 2.3.1](http://informaton.pl/?p=229). Treści migające i błyskające mogą wywołać u użytkowników z padaczką atak, co uniemożliwi im dalsze korzystanie z treści. Może to brzmi zabawnie, ale atak epilepsji jest bardzo nieprzyjemny i może też być groźny dla zdrowia. W poprzedniej wersji WCAG zabronione było stosowanie treści mogących wywoływać ataki, ale w WCAG 2.0 nieco to złagodzono przez dopuszczenie elementów o niskim ryzyku wywołania ataku. Określenie tego, czy dana treść spełnia te wymagania, jest na tyle trudne technicznie, że lepiej po prostu unikać ich w ogóle.

## Treść poruszająca się

Wreszcie czwartym warunkiem brzegowym jest możliwość zatrzymania, wstrzymania lub ukrycia treści poruszających się, opisana w [SC 2.2.2](http://informaton.pl/?p=208). Od razu jest oczywiste, że tego rodzaju informacja może umknąć wielu użytkownikom, a zatem bez odpowiednich mechanizmów jest niedostępna. Jest niedostępna także w znaczeniu availability, a nie tylko accessibility, szczególnie jeżeli znika bezpowrotnie. Jest to też informacja ciekawa z innego powodu – użytkownik może wcale nie mieć świadomości, że takowa się pojawiła i zniknęła. Jest to zatem treść podwyższonego ryzyka, której najlepiej w ogóle nie stosować.

## I to jest dopiero początek

Potem trzeba badać dalej i przechodzić wszystkie kryteria sukcesu na zaplanowanym poziomie dostępności. Powyższe cztery warunki brzegowe są dosyć łatwe do weryfikacji, chociaż żadnego nie da się sprawdzić w sposób automatyczny. Automatyczny dźwięk, treści migające i poruszające najlepiej po prostu wyeliminować z serwisu, a pułapkę na klawiaturę sprawdzić ręcznie. Potem będzie z górki.