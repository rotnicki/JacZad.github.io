---
id: 1089
title: 'Dostępność treści zależy także od platformy systemowej'
date: '2014-08-01T11:53:05+02:00'
layout: post
guid: 'http://informaton.pl/?p=1089'
permalink: /2014/08/01/dostepnosc-tresci-zalezy-takze-od-platformy-systemowej/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - Android
    - dokumenty
    - EPUB
    - iOS
    - Linux
    - 'OS X'
    - PDF
    - semantyka
    - Windows
    - Word
---

Cierpliwe i staranne przygotowanie materiału w dostępnej formie może nie zostać docenione, gdy jako kontener użyty zostanie format słabo obsługiwany przez technologie asystujące. Na przykład dokument w formacie Word z odpowiednimi nagłówkami, tabelami, tekstami alternatywnymi i całą resztą szykan będzie zwykłym płaskim tekstem pod systemem OS X lub Linux. Podobnie może się zdarzyć z formatem PDF. Zwrócił mi na to uwagę właśnie przeczytany artykuł [MS Word not an accessible alternative.](https://webtoolkit.govt.nz/blog/2014/07/ms-word-not-an-accessible-alternative/) Dlaczego tak jest?

System operacyjny Windows jest najlepiej zaprojektowanym pod względem dostępności dla osób niewidomych ze wszystkich na rynku. Bardzo bogate API oraz starannie projektowane interfejsy sprawiają, że zarówno sam system, jak i aplikacje firmy Microsoft zazwyczaj doskonale współpracują z każdym czytnikiem ekranu. Tak jest także z edytorem MS Word, który udostępnia nie tylko samą treść dokumentu, ale także jego strukturę i precyzyjne informacje kontekstowe, na przykład o użytym stylu, rodzaju i kroju czcionki, czy kolorach. Nieco mniej doskonały, ale wciąż bardzo dobry jest interfejs Adobe Readera, czyli czytnika plików PDF. W obu przypadkach kluczowe jest staranne przygotowanie treści pod kątem semantycznym, a w wypadku formatu PDF także zastosowanie tagowania treści, a jeszcze lepiej – użycie standardu PDF/A. Można zatem powiedzieć, że pod tym systemem formaty DOCX i PDF są dobrym nośnikiem

Jednak pod innymi systemami już tak dobrze nie jest. Właściwie pod żadnym nie da się osiągnąć porównywalnego poziomu dostępności tego rodzaju treści. Często zaś zdarza się, że dostępność ogranicza się do samego tekstu, bez informacji semantycznej. Nie wiadomo zatem, czy dany tekst jest nagłówkiem i którego poziomu, gdzie zaczyna się i kończy lista lub notatka na marginesie. Te informacje nadal są zaszyte w dokumencie, ale przeglądarki i czytniki ekranu nie są w stanie do niej dotrzeć. W przypadku formatu Word wynika to w dużej mierze z faktu, że format ten musi być otwierany w alternatywnej przeglądarce lub edytorze, bo pod OS X Word jest niemal całkowicie niedostępny, a pod Linuksem w ogóle go nie ma. Czytniki Adobe Reader dostępne są na wszystkie platformy, ale na żadnej obsługa czytników ekranu nie jest tak doskonała, jak pod Windows.

Sam problemu do tej pory nie zauważyłem, bo korzystam właśnie z systemu Windows, a na urządzeniach mobilnych niezbyt często czytałem formaty DOCX lub PDF. Jednak problem jest poważny, bo w Polsce coraz większą popularnością cieszą się komputery firmy Apple, a i Linux powolutku zaczyna być używalny dla osób niewidomych. Warto zatem zastanowić się, co zamiast tych ryzykownych formatów Word i PDF.

Wbrew pozorom odpowiedź jest stosunkowo prosta – alternatywą jest format HTML. Na każdej platformie systemowej, o ile posiada interfejs dostępnościowy, elementy semantyczne są prawidłowo interpretowane. Tak jest zarówno pod Windows, jak pod OS X, Linux, iOS i Androidem. Można też przyjrzeć się formatowi EPUB, który w środku ma i tak dokument HTML. Jednak ten ostatni nie doczekał się jeszcze w pełni dostępnych czytników. Dlatego ja zachęcam, by z dobrze sformatowanego i dostępnego pliku DOCX eksportować dokument HTML i to właśnie ten dokument umieszczać na stronach internetowych.