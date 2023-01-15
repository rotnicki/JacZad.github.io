---
id: 2346
title: 'Kilka łączy na piątek (EPUB)'
date: '2021-06-04T10:32:30+02:00'
excerpt: 'Piątkowe łącza traktują o publikacjach elektronicznych w formacie #EPUB. Specyfikacje, cyfrowa dostępność, narzędzia i krótka refleksja nad niechlujnością.'
layout: post
guid: 'http://informaton.blog/?p=2346'
permalink: /2021/06/04/kilka-aczy-na-piatek-epub/
timeline_notification:
    - '1622795554'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - DAISY
    - EPUB
    - indesign
    - Sigil
    - standard
    - 'Wolne Lektury'
    - Word
---

Ostatnio zgłębiałem tematykę dostępnych dokumentów elektronicznych. Koncentrowałem się przy tym na formacie EPUB, który ma otwartą specyfikację i został wymyślony do dystrybucji e-książek, czego nie da się powiedzieć o PDF. Chcę się podzielić z Wami moimi znaleziskami, które wydają mi się użytecznymi.

1. Specyfikacja formatu EPUB znajduje się na stronie World Wide Web Consortium. Powstał także odrębny dokument [EPUB Accessibility 1.1](https://www.w3.org/TR/epub-a11y-11/) opisujący dostępność tego formatu. Tekst nie jest zbyt łatwy do przyswojenia, więc najważniesze jest to, by zapewnić dostępność plików HTML zaszytych w EPUB na poziomie przynajmniej A wytycznych WCAG. No i warto dodać metadane dotyczące dostępności.
2. Początkujący twórcy książek elektronicznych mogą poćwiczyć eksportowanie pliku wprost z Worda. Ja rzekłbym, że jest to metoda o wiele lepsza od składania publikacji w Indesign. Okazuje się jednak, że to nie jest wszystko jedno, jakiego narzędzia do konwersji użyjesz. Marek Tankielun podpowiedział mi [Save As DAISY—MS Word Add-In](https://daisy.org/activities/software/save-as-daisy-ms-word-add-in/) i to był celny strzał. Sami wypróbujcie. Wtyczka instaluje się w edytorze Word i można ją wywołać z paska narzędzi.
3. Powyższa wtyczka to tylko jedno z narzędzi oferowanych przez DAISY Consortium. Organizacja powstała w celu promowania formatu DAISy stworzonego specjalnie do dystrybucji książek dla osób niewidomych. W pewnym momencie większość funkcji trafiła do specyfikacji EPUB i obecnie są jego integralną częścią.DAISy oferuje kilka bardzo przydatnych [narzędzi](https://daisy.org/activities/software/), w tym walidator, narzędzia do masowej konwersji, edytory audiobooków.
4. Najpopularniejszym edytorem plików EPUB jest [Sigil](https://sigil-ebook.com/). Jest w pełni funkcjonalnym i dojrzałym narzędziem, którego największą wadą jest słaba dostępność dla czytników ekranu. Jednak można w nim przygotować dostępną publikację, a sprawdzić można za pomocą wtyczki do tego edytora pod nazwą [Access-Aide](https://github.com/kevinhendricks/Access-Aide). Wtyczka jest bezpłatna i działa dość podobnie do inspektora dostępności w edytorze Word.
5. A jeżeli do składania książek używany jest Indesign, co jest raczej standardem, to warto wiedzieć, jak zapewnić tam dostępność Proponuję zacząć od [Leveraging InDesign for Accessible EPUB Creation](https://inclusivepublishing.org/blog/leveraging-indesign-for-accessible-epub-creation-w/). Można obejrzeć film, prezentację, przeczytać transkrypcję – jak kto woli. A potem zerknąć do polecanych źródeł, bo tam też możesz znaleźć fajne rzeczy.

Zapewnienie cyfrowej dostępności książkom zawierającym tylko tekst lub niewielkie ilości materiału graficznego jest dość proste. Kluczem jest semantyka i metadane. Problemy pojawiają się wówczas, gdy trzeba osadzić wzory matematyczne, chemiczne, zapis nutowy, diagramy itp. Czyli dokładnie tak, jak na stronach internetowych.

W ramach moich poszukiwań, zaglądałem do wnętrzności książek z różnych wydawnictw. To, co tam zastałem, napawa mnie obawą, że do dostępności jeszcze długa droga. W środku jest niechlujnie, a metadane traktowane są po macoszemu. Najczęściej ograniczają się do tytułu, autora i wydawnictwa. Często nie ma daty, numeru ISBN i innych danych. Na tym tle pozytywnie wyróżniają się książki z [biblioteki wolnych lektur](https://wolnelektury.pl), chociaż szkoda, że nie dodawany jest ISBN.