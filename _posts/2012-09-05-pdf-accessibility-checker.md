---
id: 217
title: 'PDF Accessibility Checker'
date: '2012-09-05T07:56:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=217'
permalink: /2012/09/05/pdf-accessibility-checker/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - dokumenty
    - grafika
    - OpenOffice
    - PDF
    - tekst
    - Word
---

Zasoby internetowe to nie tylko HTML, CSS i Flash. To także dokumenty przygotowane w wielu różnych formatach, na przykład DOC, ODT czy PDF. Ten ostatni można testować za pomocą specjalnego narzędzia o nazwie PDF Accessibility Checker.

Program można pobrać [z tego miejsca](http://www.xymedia.ch/downloads/PAC_EN.zip) w postaci archiwum ZIP. Archiwum wystarczy rozpakować i uruchomić plik wykonywalny i to już właściwie koniec instrukcji, bo program jest dziecinnie łatwy w użyciu. Wystarczy wskazać plik PDF, a następnie nacisnąć przycisk “start check”. Potem możemy obejrzeć raport.

Raport prezentuje wyłącznie informacje o dostępności o charakterze technicznym, to znaczy takie, jakie da się wyciągnąć z pliku wprost. Dotyczy to zatem tagowania dokumentu, oznaczenia języka, stosowanych nagłówków lub zabezpieczeń, które mogłyby uniemożliwić dostęp do treści dokumentu. Nie pozwala oczywiście na sprawdzenie dostępności językowej, ale i tak robi bardzo dużo. Warto szczególnie uważnie przyjrzeć się plikom PDF publikowanym w biuletynach informacji publicznej naszej administracji.

Problem z plikami PDF polega na tym, że powstają one przy użyciu bardzo różnych narzędzi. Część z nich tworzy pliki poprawne pod względem dostępności, a inne zupełnie niedostępne lub dostępne w małym stopniu. O dostępności pliku PDF decydują bbowiem dwa elementy:

1. Źródło danych, którym **nie może być** zeskanowany obraz tekstu, ale informacja przygotowana już w formie dostępnej.
2. Konwerter do formatu PDF potrafiący przetworzyć dostępną informację źródłową do dostępnego pliku PDF.

Optymalnym rozwiązaniem jest przygotowywanie dokumentu w programie do edycji, a następnie zapisanie do formatu PDF w tym samym programie. Pozwala na to coraz więcej edytorów tekstu. Z kolei zawsze złe efekty dają narzędzia oparte o biblioteki Ghost Script, z których większość to wirtualne drukarki instalowane w różnych systemach operacyjnych.

Sprawdzone dobre efekty daje użycie edytora Microsoft Word, OpenOffice i pochodnych oraz TextEdit dla OS X. Z nieznanych mi powodów na teście poległ edytor Pages, który nie potrafił zaimportować pliku DOC z osadzoną tabelą. Mierne efekty dają narzędzia z rodziny TeX i LaTeX, które mają poważne problemy z polskimi diakrytykami. Jednak najgorsze są aplikacje, których zadaniem jest skanowanie dokumentów i zapisywanie ich od razu do formatu PDF. Pliki wynikowe są kontenerami zawierającymi wyłącznie obrazy, które są niedostępne właściwie dla wszystkich. A są – trzeba to z żalem podkreślić – masowo stosowane w polskich urzędach.