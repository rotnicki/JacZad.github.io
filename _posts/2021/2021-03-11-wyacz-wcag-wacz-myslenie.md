---
id: 2108
title: 'Wyłącz WCAG, włącz myślenie'
date: '2021-03-11T18:50:08+01:00'
excerpt: 'Takie moje rozważania na temat dostępności i WCAG, a także odpowiedzialności audytorów.'
layout: post
guid: 'http://informaton.blog/?p=2108'
permalink: /2021/03/11/wyacz-wcag-wacz-myslenie/
publicize_linkedin_url:
    - ''
publicize_twitter_user:
    - jaczad
timeline_notification:
    - '1615485009'
categories:
    - artykuły
tags:
    - audiodeskrypcja
    - audyt
    - CAPTCHA
    - multimedia
    - 'tekst alternatywny'
    - WCAG
---

Tytuł tego wpisu od dawna chodził mi po głowie. Mam bowiem coraz częściej wrażenie, że w tym całym zamieszaniu z dostępnością zagubiła się gdzieś sama dostępność. Są szkolenia, WCAG, listy sprawdzające, walidatory, audyty, metodyki. A przecież to jest takie proste i wystarczy na chwilę wyłączyć WCAG.

Wyłączmy go jednak tylko na chwilę, bo generalnie jest to bardzo dobry dokument, tylko jakoś źle czytany. To jest zbiór dobrych rad, jak zrobić, żeby strona internetowa była dostępna. Dokument ma charakter ogólny, a co za tym idzie – pasuje do wielu sytuacji, ale nie do wszystkich. Tymczasem jakoś wszyscy się uwzięli, by stawiać znak równości między dostępnością i spełnianiem WCAG. Czasem jednak może być tak, że spełnienie wymagań jest sprzeczne z dostępnością. Posłużę się tu konkretnymi przykładami.

## Tekst alternatywny

Pierwsza i bodajże najważniejsza wytyczna WCAG mówi, że każdy element nie będący tekstem powinien posiadać alternatywę tekstową. W powszechnym przekonaniu stosowanie ALTów jest zawsze konieczne. Wydaje się jednak, że tak nie jest zawsze.

Kilka lat temu zastanawiałem się nad plikiem z tekstem łatwym do czytania (ETRT). To taki specjalny sposób tworzenia materiałów tekstowych dla osób z niepełnosprawnością intelektualną. Tu [możesz zobaczyć przykładowy materiał](https://psoni.org.pl/wp-content/uploads/2016/10/Moj-CHLOPAK-Moja-DZIEWCZYNA-wydanie-II-do-internetu.pdf), żeby zrozumieć, na czym to polega. Tekst jest specjalnie zredagowany, uproszczony i uzupełniony obrazkami, które wspomagają zrozumienie i zapamiętanie. No i teraz zagwozdka, czy powinny one mieć teksty alternatywne?

Na pozór tak, bo nie są to grafiki ornamentowe, ale mają określoną funkcję. Czy jednak tą funkcję można przenieść do tekstu alternatywnego? Po długim namyśle muszę powiedzieć, że nie. Ten dodatkowy tekst nie tylko nie pomoże, ale wręcz zaburzy odbiór informacji. Osoba niewidoma z równoczesną niepełnosprawnością intelektualną straci na takiej dostępności.

## Audiodeskrypcja i audiotekst

Przyjrzyjmy się teraz multimediom, do których należy dodawać napisy i audiodeskrypcję. Odmianą audiodeskrypcji jest audiotekst, gdy lektor odczytuje napisy, a nie opisuje obrazy. Są to doskonałe techniki udostępniania filmów, ale nie zawsze. Zapraszam do obejrzenia filmu. znalezionego w Internecie

<https://youtu.be/IYehPLJfddU>

Autorzy bardzo się postarali i audiodeskrypcja i audiotekst są super. Tylko że nie pozwala na odbiór głównej treści, jaką jest śpiew. W tej sytuacji lepszy byłby opis tekstowy, z którym można się zapoznać na spokojnie przed lub po odsłuchaniu. Tylko wtedy nie będzie spełnione kryterium sukcesu 1.2.5 WCAG.

## Wiele dróg

Jest takie wymaganie w WCAG, żeby dać użytkownikowi możliwość znalezienia treści na różne sposoby. Można stosować menu, wyszukiwarkę, mapę serwisu, chmury tagów i pewnie coś tam jeszcze. Jednak nie zawsze jest to potrzebne. Jeżeli przyjrzeć się choćby panelowi administracyjnemu WordPressa, to tam jest zasadniczo tylko jedna ścieżka docierania do poszczególnych funkcji – przez menu. Wyszukiwarka jest obecna tylko w miejscach, gdzie mamy do czynienia z wieloma podobnymi elementami, na przykład wpisami lub wtyczkami. I jest to dobre rozwiązanie, które nie spełnia wymagań zawartych we WCAG. A dodawanie takich dodatkowych dróg na siłę jest jedynie sztuką dla sztuki.

## Etykiety dla pól formularzy

Formularze zawierają w sobie czasem wiele kontrolek: pól tekstowych, wyboru, opcji, list. Każda powinna mieć przypisaną i widoczną etykietę, dzięki czemu każdy użytkownik będzie dokładnie wiedział, co wpisać lub co zaznacza. Ponownie jednak – nie można tej zasady traktować jak prawdy objawionej, której naruszenie strąci projektanta do piekła. Co bowiem zrobić z wyszukiwarką? Czy to pole tekstowe naprawdę zawsze musi mieć etykietę? Obok jest przecież przycisk „SzukaJ”. Jest w warstwie z rolą „search”. No i użycie etykiety wydaje się zbędne. Cóż z tego, gdy walidator – ten automatyczny, jak i żywy – wytknie tu błąd. No więc spotykam czasem taką etykietę dodaną dla świętego spokoju i ukrytą wizualnie, żeby nie psuła projektu.

## CAPTCHA

Na koniec przykładów moja ulubiona CAPTCHA. Na pewno spotykacie wciąż takie rozmazane obrazki, z których trzeba przepisać litery lub cyfry. Obecnie człowiek coraz gorzej sobie radzi z ich odcyfrowaniem, a za to algorytmy nie mają z tym problemu. Zerknijmy jednak, co na temat tego rozwiązania mówi WCAG. Otóż w opisie kryterium sukcesu 1.1.1 wspomniano CAPTCHA i sposób na zapewnienie jej dostępności. Trzeba dostarczyć inną metodę zabezpieczenia opartą o możliwości zmysłowe. Wygląda to na to, że chodzi o słuch, bo interfejsy węchowe, smakowe i dotykowe są wciąż mało rozpowszechnione. I tak właśnie jest to zazwyczaj robione: zamiast rozmazanych liter możemy usłyszeć zaszumiony głos wypowiadający słowa lub cyfry.

Sęk w tym, że to jest prymitywne rozwiązanie, które często nie działa. O ile bowiem litery i cyfry mamy raczej wspólne, przynajmniej w naszym kręgu kulturowym, to języki są przecież różne. A tu w nagraniu pośród szumu ktoś niewyraźnie mówi po angielsku. Ja z trudem rozumiem, a jeżeli ktoś w ogóle nie zna tego języka? To przecież tak, jakby kazać przepisywać znaki alfabetu hebrajskiego lub pismo klinowe. Wreszcie – jest to rozwiązanie niedostępne dla osób głuchoniewidomych. A kryterium WCAG jest spełnione.

## WCAG to nie szwajcarski scyzoryk

Włączmy WCAG z powrotem. To dobry dokument i warto z niego korzystać. Jednak to nie zwalnia z myślenia o celu, jakim jest stworzenie dostępnej treści elektronicznej. WCAG nie mogą opisywać wszystkich możliwych sytuacji i wyjątków, bo to po prostu nie jest możliwe. WCAG pokazują kierunek działania, różne techniki wspomagające dostępność, a równocześnie wskazują, że każdy sposób jest dobry, by osiągnąć cel.

Zachęcam zatem do myślenia, jak zapewnić dostępność, a nie jak spełnić wymagania WCAG lub – co jeszcze gorsze – te z raportów niedouczonych audytorów. Błędy mają także różną wagę, czego nie widać w raportach, zwłaszcza automatycznych. Na ten problem próbuje odpowiedzieć szkic WCAG 3.0, ale na razie dość nieporadnie.

Mam wrażenie, że to w wielu przypadkach bierze się z lęku. Audytorzy boją się wziąć odpowiedzialność za swoje opinie i zasłaniają się listą błędów. Boją się, że ktoś ich sprawdzi i z satysfakcją wskaże na uchybienia. Apeluję zatem – przestańcie się bać i pozwólcie sobie myśleć i decydować. Z WCAG w głowie, ale nie zamiast głowy.