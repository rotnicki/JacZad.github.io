---
title: 'Authoring Tool Accessibility Guidelines (ATAG) 2.0 jest oficjalnym standardem'
date: '2015-09-27T10:01:01+02:00'
layout: post
categories:
    - artykuły
tags:
    - 'ATAG'
    - standardy
    - W3C
---

Dużo piszę tutaj na temat WCAG 2.0, a niepostrzeżenie dojrzał większy brat tej specyfikacji, czyli [ATAG 2.0](http://www.w3.org/TR/ATAG20/). Jest to dokument mało znany, a niesłusznie, bo opisuje dostępność na pewnego rodzaju metapoziomie. Można znaleźć tam wytyczne na temat tworzenia dostępnych narzędzi służących do tworzenia dostępnych treści. ATAG 2.0 jest specyfikacją nawiązującą do WCAG 2.0 i ma w wielu miejscach zbliżoną strukturę. Nie jest jednak po prostu rozbudowaną kopią z wyjaśnieniami, ale czymś dużo bardziej ogólnym.

Do czytania ATAG powinni się brać przede wszystkim autorzy edytorów treści w rodzaju TinyMCE, Live Writer, a nawet Word i Libre Writer. Nawiasem mówiąc – może czytają, bo akurat te edytory całkiem nieźle implementują ATAG, chociaż pewnie raczej dzięki intuicji i praktycznym potrzebom autorów, a nie dogłębnemu studiowaniu specyfikacji. Jednak większość edytorów w ogóle nie wspiera tworzenia dostępnych treści, co skutkuje naruszeniem wytycznych WCAG. A przecież w dzisiejszym internecie wszyscy jesteśmy autorami. Pisząc post na Facebooku, wstawiając fotkę na Instagrama lub Twittera, pisząc artykuł dla popularnego portalu technologicznego. Wszędzie tam autor powinien być zachęcany, a może czasem zmuszany, do dodawania tekstów alternatywnych, wyróżniania informacji semantycznie, stosowania nagłówków i list.

Dlaczego powinien być zmuszany? Choćby dla edukacji, bo przecież cały czas się uczymy. W YouTube dodając film jesteśmy pytani, co z napisami i należy zaznaczyć powód, dla którego ich nie ma. Niektóre edytory treści w systemach zarządzania treścią przy wstawianiu obrazka cisną redaktora o wpisanie tekstu alternatywnego, a czasem po prostu nie pozwalają na dodanie go do artykułu.

Są też rozwiązania z drugiej strony, na przykład automatycznie generowane teksty alternatywne dla grafik ilustrujących aktualności. Skrypt zapożycza sobie tytuł aktualności i wkleja go do atrybutu ALT. Jest to rozwiązanie niemal zawsze złe i nie spełniające wymagań dostępności, chociaż nie do wychwycenia przez automaty walidujące. To też jest kolejnym dowodem na to, że dostępności nie da się zbudować na automatyzowaniu procesów testowania czy generowania treści. Dlatego ludziom potrzebne są proste i wygodne narzędzia, dzięki którym dostępność nie będzie ich bolała. Na początek proponuję, by przy dodawaniu zdjęć na Facebooka dodać także pole edycyjne do tekstu alternatywnego oraz prostą instrukcję, do czego służy. W ten sposób można zaimplementować kryterium sukcesu B.2.3.1 ATAG 2.0.
