---
id: 983
title: 'Poradnik na temat tworzenia alternatywnych wersji dla grafiki'
date: '2014-03-10T10:28:00+01:00'
layout: post
guid: 'http://informaton.pl/?p=983'
permalink: /2014/03/10/poradnik-na-temat-tworzenia-alternatywnych-wersji-dla-grafiki/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - DAISY
    - e-podręcznik
    - EPUB
    - grafika
    - 'grafika dotykowa'
    - 'tekst alternatywny'
---

Przygotowanie wersji alternatywnych dla grafiki jest niekiedy sporym wyzwaniem. Zmierzyć się z nim muszą na przykład autorzy e-podręcznika. Ciekawym materiałem pomocniczym może być opisana poniżej publikacja, niestety – po angielsku. Za to podejmuje temat grafik trudnych do opisania i w kontekście edukacyjnym.

Poradnik to [Accessible Image Sample Book](http://diagramcenter.org/standards-and-practices/accessible-image-sample-book.html), czyli w wolnym tłumaczeniu – “Księga przykładowych dostępnych grafik”.. Dostępny jest w trzech formatach: [archiwum HTML](http://diagramcenter.org/wp-content/uploads/2014/02/samplebook_html_020420141.zip), [EPUB 2](https://dl.dropboxusercontent.com/u/104703039/samplebook_epub2_final_02142014.epub) oraz [EPUB 3](https://dl.dropboxusercontent.com/u/104703039/samplebook_epub3_final_02142014.epub). Każdy może zatem wybrać coś odpowiedniego dla siebie. A co w środku?

W środku odpowiedzi na pytania, jak tworzyć teksty alternatywne, grafikę dotykową, a nawet wersje dźwiękowe informacji wizualnej. Przykłady zaś są różnorodne: schemat budowy serca, mapa historyczna, wykres funkcji kwadratowej i kilka innych. Każdy opatrzony jest wyjaśnieniami, w jaki sposób technicznie osadzić taki opis alternatywny w HTML, EPUb i DAISY. Oprócz tego sugestie co do materiałów dotykowych i ciekawostka – dźwiękowa interpretacja wykresu funkcji kwadratowej, czyli paraboli. Na temat użyteczności się nie wypowiem, ale pomysł jest ciekawy.

W przykładzie z funkcją kwadratową rozważany też jest problem zapisu wzorów matematycznych. Jak widać – MathML jest raczej trudny do zrozumienia dla osoby niewprawionej i zastosowany jest opis liniowy. Ciekawe jest podejście do opisu mapy historycznej, gdzie omówiono pokrótce poziomy szczegółowości, czyli podstawowy opis alternatywny oraz rozszerzony, zawierający wszystkie niezbędne informacje.

Zupełnie przy okazji dowiedziałem się, że w EPUB 3 stosuje się ARIA. Tu w przykładach używany jest atrybut aria-describedby, ale być może w innych sytuacjach stosuje się także inne elementy. Nigdy nie interesowałem się tym standardem, a może trzeba. Samą publikację zaś polecam, tym bardziej że jest dosyć krótka i treściwa.