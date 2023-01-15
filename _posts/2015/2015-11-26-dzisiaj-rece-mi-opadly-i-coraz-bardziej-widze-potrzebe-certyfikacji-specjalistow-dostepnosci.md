---
id: 1466
title: 'Dzisiaj ręce mi opadły i coraz bardziej widzę potrzebę certyfikacji specjalistów dostępności.'
date: '2015-11-26T14:50:49+01:00'
layout: post
guid: 'http://informaton.pl/?p=1466'
permalink: /2015/11/26/dzisiaj-rece-mi-opadly-i-coraz-bardziej-widze-potrzebe-certyfikacji-specjalistow-dostepnosci/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - audyt
    - błędy
    - certyfikacja
    - PDF
    - publikacje
    - 'WCAG 2.0'
---

Dzisiaj natknąłem się na prawdziwe curiosum w dziedzinie dostępności. Jest to [Poradnik WCAG](http://audytwcag.squiz.pl/), który warto pobrać, by dołączyć do mnie w rozpaczy. Materiał ten ma za zadanie uwiarygodnić firmę reklamującą audyty dostępności i jest tak zły, że coraz bardziej widzę potrzebę certyfikowania specjalistów dostępności. Poradnik napisał bowiem ktoś, kto na temat dostępności nie wie nic. Większość materiału jest przepisana z [polskiego tłumaczenia WCAG 2.0](http://fdc.org.pl/wcag2) i to są jedyne fragmenty z sensem. Dalej niemal wyłącznie brednie.

Autor nie jest w stanie nawet napisać prawidłowo nazwy specyfikacji, ani podać daty rozporządzenia. To jednak są wpadki świadczące tylko o niechlujstwie, a jeszcze niekoniecznie o niekompetencji. To można znaleźć później i zaczyna się od razu z grubej rury. Poniżej podam kilka cytatów w pisowni oryginalnej, chociaż zdaję sobie sprawę, że niektóre będą bardzo hermetyczne i niezrozumiałe dla osób, które dopiero szukają informacji o dostępności. Dlatego dodam wszędzie krótkie wyjaśnienie. Przeklejam wprost z pliku PDF, abyście mogli docenić także jego dostępność i polubić czytanie tekstu długim ciurkiem.

> Rekomendacje Wszystkie grafikipowinnyposiadaćopisalternatywnywpostaciatrybutu&lt;alt&gt;,ale wartośćtego atrybutupowinnabyćpusta— &lt;alt=””&gt;.Wówczastakielement graficznybędzie całkowicie pomijanyprzezczytnikiekranu.

Wyjaśnienie ode mnie: to dotyczy tylko i wyłącznie grafiki nie niosącej żadnej informacji, czyli ornamentowej. W ten sposób skonstruowana rekomendacja oznaczać będzie dużo niższą dostępność dla osób niewidomych.

> Rekomendacje Należyunikaćprezentowaniatreścizapomocąsymboligraficznychnp.lupajako przyciskwyszukiwanialubikonaRSSjako linkdo kanałuRSS.Istnieje możliwość umieszczaniagrafiknp.wkształcie lupy,jednakpowinnyone pełnićtylko rolędekoracyjną.

Wyjaśnienie ode mnie: ta rekomendacja jest nie tylko głupia, ale przypisana do kryterium sukcesu 1.3.3, które traktuje o czymś zupełnie innym. Ewidentnie ktoś nie doczytał nawet wyjaśnienia zawartego w samych WCAG 2.0. Można spokojnie stosować ikonki RSS i inne, o ile spełnione są inne wymagania, na przykład tekst alternatywny. Jednak poprzednia rekomendacja to wyklucza…

> Rekomendacje Wszystkie linkitekstowe zamieszczone wserwisie powinnyodróżniaćsięwyraźnie odtekstu,zarówno poprzezzmianękolorujakiformatowania.Jednymze standardów sieciowychjest stosowanie podkreśleniado wyróżnienialinkówizalecamydo stosowaniasiędotego rozwiązania.Prawidłowo oznaczonylinktekstowypowinienmiećkolorinnyniżtekst ikontrast do tła  
> napoziomie minimum4,5:1orazbyćpodkreślony.Po wskazaniukursoremmyszyna  
> linktekstowypodkreślenie powinno znikać. W przypadku braku możliwościzastosowaniazmianyformatowaniadlalinku tekstowego,kolorlinkutekstowego powinienmiećkontrast do kolorutłanapoziomie minimum4,5:1irównocześnie kontrast do kolorutekstunapoziomie minimum3:1

Wyjaśnienie ode mnie: ta rekomendacja jest już tak karkołomna, że nie wiem w co klawisze włożyć… Do tego jest przyczepiona do kryterium sukcesu 1.4.1, które mówi o tym, by informacja nie była wyróżniana tylko kolorem. Dlaczego podkreślenie ma znikać? Z czym ma być ten kontrast 3:1, a z czym 4.5:1? Tu nawet trudno o jakieś wyjaśnienia, bo ja nawet nie rozumiem, co autor miał na myśli.

> Rekomendacje Zastosowanie przycisków“play/pause”orazsuwakaregulacjigłośności.

Wyjaśnienie ode mnie: to jest rekomendacja do kryterium sukcesu 1.4.2 mówiącego o możliwości kontrolowania dźwięku, jeżeli uruchamiany jest automatycznie. Ponownie autor w ogóle nie rozumie problemu, bo ten dźwięk trzeba wyłączyć prostym mechanizmem, na przykład klawiszem Esc, bo on zakłóca syntezę mowy, więc niewidomy użytkownik nie znajdzie tego całego przycisku lub suwaka.

Jesteśmy dopiero przy pierwszej zasadzie, a mi się nie chce dalej wycinać i wklejać. Poza tym prawo cytatu mówi o 30% materiału źródłowego, a ja pewnie bym przekroczył 80%. Dlatego w tym miejscu zakończę podsumowaniem – to jest bardzo zły materiał, z którego nie wolno korzystać. Jakość audytu będzie zatem równie zła, bo skoro autor nie zna się na dostępności i jej nie rozumie, to jak ma zrobić audyt?

Od pewnego czasu dyskutujemy nad jakąś formą certyfikacji ekspertów dostępności – audytorów, projektantów, programistów. Gdy czytam bzdety napisane w tym “poradniku” to mam poczucie, że trzeba się z tym śpieszyć. Skąd firma lub urząd ma wiedzieć, kto potrafi zrobić dobry audyt? Skoro napisali, że robią, dali cenę i jeszcze udostępnili “poradnik”, to znaczy że się znają.

Co jakiś czas polecam publikacje poświęcone dostępności, gdy uznam że są dobre. Po raz pierwszy polecam coś, co z pewnością dobre nie jest. I wcale nie jestem pewien, czy dobrze robię. Jak jednak inaczej mam przestrzec przed popełnieniem błędu i skorzystaniem z usług tej firmy? Powoli tworzy się rynek na dostępność i pojawiają się podmioty chcące z tego skorzystać, bo luka jest wciąż duża. Z rozmysłem wybierajcie i nie sugerujcie się tylko ceną. Są darmowe publikacje o wysokim poziomie i takie gnioty, jak ten opisywany. Są i będą usługi tanie i drogie, ale cena nie powie nic o jakości. Dlatego trzeba coś z tym zrobić i to w miarę szybko.