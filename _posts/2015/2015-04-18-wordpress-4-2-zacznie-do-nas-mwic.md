---
id: 1305
title: 'WordPress 4.2 zacznie do nas mówić'
date: '2015-04-18T09:51:00+02:00'
layout: post
guid: 'http://informaton.pl/?p=1305'
permalink: /2015/04/18/wordpress-4-2-zacznie-do-nas-mwic/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - ARIA
    - 'czytniki ekranu'
    - mowa
    - opensource
    - Wordpress
---

Troszkę przesadzam, ale miło jest napisać o nowym rozwiązaniu wprowadzanym właśnie do nowej wersji WordPressa. Autorzy skórek i wtyczek oraz programiści głównego rdzenia tego CMSa będą mieli możliwość skorzystania z nowej metody JavaScript wp.a11y.speak(), która doda funkcjonalności związane z [aktywnymi obszarami.](http://informaton.pl/artykuly/aktywne-obszary-i-wsplczynnik-nachalnosci/)

Technologia Ajax i podobne są chętnie stosowane, bo nie wymagają przeładowywania strony za każdym razem, gdy coś się na niej zmieni. Jednak tego typu informacje mogą umknąć niewidomym użytkownikom, a odpowiedzią na ten problem jest ARIA i jej specjalny atrybut aria-live. Zobowiązuje on przeglądarkę do zaanonsowania użytkownikowi zmian na stronie, by nic go nie ominęło. Tak są anonsowane choćby chaty na Facebooku lub komunikaty ostrzegawcze na YouTube. Oczywiście projektanci skórek i wtyczek mogli na własną rękę implementować aktywne obszary, ale wprowadzenie tego rozwiązania do API WordPressa z pewnością im to ułatwi. Więcej szczegółów można znaleźć w notatce na [blogu twórców WordPressa.](https://make.wordpress.org/accessibility/2015/04/15/let-wordpress-speak-new-in-wordpress-4-2/)