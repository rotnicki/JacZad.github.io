---
id: 2603
title: 'Czy też mierzysz węża linijką?'
date: '2021-12-03T17:52:48+01:00'
author: 'Jacek Zadrożny'
layout: post
guid: 'https://informaton.blog/?p=2603'
permalink: /2021/12/03/czy-tez-mierzysz-weza-linijka/
categories:
    - artykuły
tags:
    - audyt
    - badania
    - 'prosty język'
    - 'sztuczna inteligencja'
---

Przeczytałem ostatnio bardzo ciekawy artykuł dotyczący prostego języka i algorytmów jego pomiarów. Uderzyło mnie, jak to jest podobne do badania cyfrowej dostępności. Najpierw zachęcam do [przeczytania całego artykułu](https://www.linkedin.com/pulse/czy-prosty-język-da-się-policzyć-czyliomierzeniu-węża-zandberg-malec/?trackingId=ib3+mUqlQqey0LoVEYyCaA==), a dopiero potem reszty.

Autorka wskazuje, że:

- badania automatyczne są zawodne i służą głównie do potwierdzania wyników pracy,
- dla użytkowników liczy się wskaźnik, a nie prostota języka, a to oznacza że pracują dla niego,
- algorytmy są wciąż bardzo głupie i łatwo je oszukać.

Celnych tez w artykule jest znacznie więcej, a ja tylko wybrałem kilka, żeby pokazać podobieństwa. Bardzo podobnie jest w badaniu cyfrowej dostępności, gdzie często ludzie skupiają się na zaspokajaniu potrzeb walidatorów, a nie celu, jakim jest dostępność. Uruchamiają jakieś narzędzie i są zadowoleni, bo nie zgłosiło żadnych błędów. Tylko co z tego? Przecież brak błędów ortograficznych w tekście nie oznacza, że tekst jest dobry.

Autorka stawia też podobną diagnozę do mojej – problemem jest ludzkie lenistwo. Nie takie lenistwo, że nic nie chcą zrobić, lecz że chcą osiągnąć cel szybko i bez wysiłku. A tu się tak nie da. Audyty dostępności są drogie dlatego, że to nudna i mozolna robota, a nie dlatego, że audytorzy chcą dużo zarabiać. A przecież wystarczy uruchomić Wave, Tenon, SortSite, ANDI lub AXE i ma wyniki. Za darmo i w kilka sekund, najwyżej minut. Więc za co tyle płacić? Ano za pozostałe 80% roboty wykonywanej ręcznie.

Wreszcie – automaty są zawodne. Mają swoje błędy, a to sprawia, że dają błędne wyniki. Tak jest chociażby z walidatorem plików PDF o nazwie PDF Accessibility Checker. Ignoruje prawidłowo osadzone grafiki ornamentowe i zgłasza błąd braku tekstu alternatywnego. Ja wiem, że plik jest poprawny, a walidator – nie. A skoro nie wie walidator, to wprowadzi w błąd także mniej doświadczonego testera.

Bardzo uważnie obserwuję rozwój narzędzi do wykrywania błędów cyfrowej dostępności. Póki co – nie są one zbyt sprytne. Kontynuując analogię z tekstem – nie odróżniają „może” od „morze”, bo oba słowa są w słowniku. Liczy się kontekst. Dlatego prostego języka i cyfrowej dostępności nie da się mierzyć linijką. Dokładnie jak wijącego się węża. Wynik zawsze będzie co najwyżej przybliżony.