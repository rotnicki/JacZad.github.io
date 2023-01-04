---
id: 379
title: 'Dostępne skórki dla WordPressa'
date: '2012-11-18T10:56:03+01:00'
layout: post
guid: 'http://informaton.pl/?p=379'
permalink: /2012/11/18/dostepne-skrki-dla-wordpressa/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - CMS
    - formularze
    - grafika
    - 'open source'
    - tekst
    - Wordpress
---

WordPress jest bardzo popularnym systemem do zarządzania treścią (CMS) rozwijanym w modelu Open Source. Od pewnego czasu twórcy kładą duży nacisk na jego dostępność (accessibility) i właśnie uczynili kolejny krok. Zaproponowali kryteria dostępności dla skórek, a spełniające je zostaną oznaczone tagiem “accessibility-ready”.

Informacje na ten temat opublikowano na [blogu na temat dostępności w WordPress](http://make.wordpress.org/accessibility/2012/11/12/weve-now-completed-the-draft-theme-accessibility-audit/). Kluczowym elementem ma być [zestaw kryteriów dostępności](http://make.wordpress.org/accessibility/theme-accessibility-audit-draft-proposal/), które powinny być spełnione, by autor mógł dodać znacznik “accessibility-ready” do swojej skórki. Dokument ma na razie charakter szkicu i można do niego zgłaszać uwagi. W skrócie obejmuje takie elementy jak:

- dekoracyjne grafiki mają być wyświetlane za pomocą stylów,
- nagłówki powinny być stosowane w prawidłowy sposób,
- nie można stosować linków w rodzaju “czytaj dalej” czy “więcej”,
- fokus powinien być widoczny, a nawigacja powinna być możliwa za pomocą klawiatury,
- zastosowany kontrast pomiędzy tłem i tekstem powinien wynosić przynajmniej 4,5:1,
- skórka powinna zawierać linki do przeskakiwania do treści (skip links),
- formularze powinny zawierać odpowiednie etykiety,
- niedopuszczalne jest stosowanie zaburzających logikę atrybutów TABINDEX, ACCESSKEY oraz nieoczekiwanego otwierania nowych stron lub zakładek.

Dokument faktycznie jest jeszcze niedopracowany, ale może zostaną uwzględnione inne ważne elementy, na przykład zakaz stosowania migających elementów. Ale początek jest dobry.