---
id: 971
title: 'TinyMCE 4.0 &#8211; trochę zachwytu i trochę rozczarowania'
date: '2014-03-07T11:27:53+01:00'
layout: post
guid: 'http://informaton.pl/?p=971'
permalink: /2014/03/07/tinymce-4-0-troche-zachwytu-i-troche-rozczarowania/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - multimedia
    - semantyka
    - tekst
    - TinyMCE
    - Wordpress
---

TinyMCE to popularny edytor WYSIWYG online, napisany w JavaScript i używany w wielu systemach CMS, na przykład WordPress. Jest on w pewnym stopniu dostępny, ale jest to raczej poziom akceptowalny, niż zadowalający. Dlatego z przyjemnością odnotowałem informację, że autorzy zadbali o podwyższenie tego poziomu. Sprawdziłem i w pierwszej chwili wpadłem w euforię. Potem poprzyglądałem się bliżej i emocje opadły.

Pierwsze testy zrobiłem przy pomocy przeglądarki Firefox i czytnika ekranu NVDA. Pole edycyjne na stronie [TinyMCE](http://tinymce.com/), czyli demo edytora, było obsługiwane dobrze. Skasowałem domyślny tekst i zacząłem eksperymentować. Pisałem i formatowałem tekst na różne sposoby, dodawałem i usuwałem łącza i w ogóle robiłem to, co robiłbym edytując prawdziwy wpis. Do paska narzędzi można się dostać za pomocą klawisza F10, a do rozwijalnego menu – klawiszem F9. Szczególnie ujęła mnie świetna obsługa klawiatury, którą poprawiono w wersji 4.0.17, jak informuje [plik o zmianach.](http://www.tinymce.com/develop/changelog/index.php?type=tinymce). W samym oknie edycji anonsowany był rodzaj formatowania, na przykład “lista”, “nagłówek” z numerem poziomu itp. Działało niemal perfekcyjnie, chociaż czasem nie czytane były linki lub typ formatowania w rodzaju cytatu. To jednak jest do przełknięcia.

Potem sprawdziłem, jak to wszystko działa w innych przeglądarkach. W Chrome nie działało w ogóle, a w Internet Explorerze – jako tako. Przełączyłem się na Window-Eyes 8.4 i też smuteczek – działa słabiutko. To znaczy, że pozostaje mi pierwotny tandem NVDA/Firefox. Wielka szkoda.

Kiedy już nacieszyłem się formatowaniem tekstu i tworzeniem linków, zachciało mi się pokombinować bardziej. Dodam sobie tabelę i zobaczę, co z tego wyjdzie. Okazało się jednak, że już samo dodanie tabelki jest problematyczne z poziomu klawiatury, a jak już się udało, to jej edytowanie okazało się być mocno uciążliwe. Jeszcze gorzej było z multimediami, do których użyto MoxieManagera, który jest słabo dostępny i nie udało mi się za jego pomocą dodać ani grafiki, ani filmu. Mam nadzieję, że w WordPress będzie do tego inne rozszerzenie, bo to się w tym momencie nie nadaje.

Tak więc krzywa emocji opadła i nie mam zamiaru TinyMCE stawiać za wzór dostępności. Jednak robią postępy i z przyjemnością powitam tą wersję edytora na pokładzie WordPressa 3.9. Do tego czasu jakoś sobie będę radził.