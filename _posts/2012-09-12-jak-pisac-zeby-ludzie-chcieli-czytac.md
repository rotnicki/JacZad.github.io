---
id: 235
title: 'Jak pisać, żeby ludzie chcieli czytać'
date: '2012-09-12T18:02:18+02:00'
layout: post
guid: 'http://informaton.pl/?p=235'
permalink: /2012/09/12/jak-pisac-zeby-ludzie-chcieli-czytac/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - easy-to-read
    - język
    - nagłówki
    - tekst
---

Treść w Internecie to przede wszystkim obraz i tekst. O obrazie pisałem już wcześniej, a teraz kilka zdań na temat tekstu. I tym razem (prawie) nie będę pisał o wyglądzie.

## Różnorodność odbiorców

Autorzy tekstów umieszczanych w Internecie powinni pamiętać o tym, że ich odbiorcy różnią się od nich. Czasem są mniej, a czasem bardziej inteligentni. Ich znajomość tematu może być znikoma lub ogromna, a stosowany język specjalistyczny (żargon) zrozumiały lub nie. Najważniejsze jednak jest to, że odbiorca nie siedzi w głowie autora, ale na drugim końcu sieci (choćby nawet było to sąsiednie biurko) i nie zna jego myśli. Dlatego tekst powinien być napisany w sposób zrozumiały dla jak największej grupy odbiorców.

Napisanie tekstu będącego prawidłowym komunikatem dla odbiorcy nie jest trudne, o ile autor będzie przestrzegał kilku podstawowych zasad:

- tekst powinien być napisany prostym językiem,
- słowa i wyrażenia obce i żargonowe powinny być wyjaśnione,
- skróty i akronimy powinny posiadać rozwinięcie,
- formatowanie powinno wspomagać czytanie.

Niby tego sporo, ale wiele z tych elementów robi się odruchowo. Tutaj umieszczam je dla usystematyzowania.

## Prosty język

Niektórzy autorzy piszą tak, jak mówią. Po prostu zapisują w sposób mechaniczny swoje myśli lub wypowiedzi. Czasem taka forma sprawia, że tekst czyta się łatwo, a czasem – wręcz przeciwnie. Tekst łatwy do czytania może wymagać krytycznego przyjrzenia się swojemu stylowi. Ponieważ trudno jest krytycznie patrzeć na swoje dzieło, warto dać to do przeczytania komuś innemu. Najlepiej, jeżeli będzie to osoba dla której temat jest obcy, ponieważ taka osoba wskaże miejsca zupełnie dla niej niezrozumiałe.

Przy tworzeniu tekstu warto przyjąć pewne założenia. Jednym z nich może być maksymalna długość zdania ograniczona do około 18 słów. Jakiś czas temu przeprowadziłem prosty test polegający na tym, że ktoś odczytywał zdanie z pewnego tekstu, a następnie starał się je powtórzyć. Jeżeli nie był w stanie przypomnieć sobie początku, to oznaczało że zdanie było za długie. W wypadku tej osoby granica wypadała właśnie w okolicy 18 słów, choć dla języka angielskiego WCAG 2.0 zaleca 25 słów.

Co prawda do tekstu pisanego można wrócić i od początku przeczytać zdanie, ale tego właśnie należy unikać. Jeżeli czytelnik musi wracać do początku zdania, a czasem nawet musi to zrobić kilka razy, to czytanie go męczy i zniechęca. Z pewnością intuicyjnie każdy odczuwa, że jakiś tekst jest łatwy, a inny trudny i nie zawsze wie dlaczego. Powodem może być właśnie zbyt skomplikowana składnia. Warto zatem popracować i rozbić zdanie złożone na dwa lub więcej prostych. Zaś o tym, jak **nie należy pisać** można przeczytać w [felietonie Jacka Wesołowskiego](http://esensja.pl/varia/publicystyka/tekst.html?id=4767)

## Słowa i wyrażenia obce i żargonowe

Drugim ważnym elementem mającym wpływ na odbiór tekstu jest stosowane słownictwo. Tutaj szczególnie ważne jest zdefiniowanie odbiorców tekstu. Jeżeli tekst jest skierowany do prawników, to zakładamy, że pojęcia w rodzaju "oświadczenie woli" czy "zapytanie prejudycjalne" są im znane. Jeżeli jednak tekst kierowany jest do szerokiego odbiorcy, to nie może być hermetyczny. Wzorem do naśladowania jest tutaj [Wikipedia](http://pl.wikipedia.org), w której stosowane są odnośniki do innych haseł, które objaśniają lub rozszerzają podlinkowany fragment.

## skróty i akronimy

Nie będę się silił na wytłumaczenie, na czym polega różnica pomiędzy skrótowcem (akronimem) i skrótem (abrewiaturą), ale odsyłam do definicji zawartych w Wikipedii. W tym miejscu pojawią się jedyne w tym szkicu kody HTML. Opiszę zaś sposób, w jaki można i należy oznaczać ciągi znaków będące skróconymi wersjami dłuższych ciągów tekstu.

W wielu tekstach stosuje się skrócone wersje zapisów nazywane skrótowcami i skrótami. Stosowanie ich jest wygodne i pożyteczne, ale warto czytelnikom wyjaśnić ich znaczenie przynajmniej przy ich pierwszym wystąpieniu. Do tego celu służą dwa znaczniki języka <acronym title="HyperText Markup Language">HTML</acronym>: &lt;abbr&gt; i &lt;acronym&gt;, zaś deskryptor umieszcza się w atrybucie title, na przykład tak:

 `<abbr title="złoty">zł</abbr>`

Od razu też przepraszam za trywialny przykład, który jednak dość jasno pokazuje zastosowanie i sposób realizacji. Drugi będzie podobnie trywialny, choć z podtekstem politycznym:

 `<acronym title="Platforma Obywatelska">PO</acronym>.`

Teraz kilka słów o tym, dla kogo tak się należy męczyć. Po pierwsze istnieją sposoby na prezentację takiego objaśnienia w przeglądarkach internetowych, na przykład za pomocą dymka. Po drugie programy do odczytu ekranu dla osób niewidomych mogą odczytywać rozwinięcia innym głosem lub pomijać te informacje – zależnie od konfiguracji i preferencji użytkownika. Wreszcie po trzecie – automaty (na przykład translatory) będą miały jasną informację, że tego elementu nie należy tłumaczyć.

## Formatowanie wspomagające czytanie

Na koniec warto wspomnieć jeszcze o stronie wizualnej tekstu. Dla jego większej czytelności warto wykonać dwie rzeczy: podzielić go na mniejsze fragmenty i wyróżnić to, co najważniejsze. Jedno i drugie należy robić w zgodzie z zasadami dostępności oraz uwzględniając strukturę dokumentu.

Dzielenie tekstu na mniejsze kawałki może odbywać się co najmniej na trzy sposoby:

- dzielenie tekstu na fragmenty i nadawanie im tytułów,
- wydzielanie akapitów, czyli mniejszych logicznych fragmentów tekstu,
- listowanie tego, co da się wylistować.

Do wydzielania dużych fragmentów (rozdziałów, podrozdziałów itp.) należy stosować nagłówki odpowiedniego poziomu. Język HTML pozwala na oznaczenie tytułów nagłówkami stopni od pierwszego (H1) do szóstego (H6). Należy przy tym pamiętać, że ważna jest kolejność zagnieżdżania, a więc nagłówek poziomu pierwszego ma najwyższy priorytet, po którym następują nagłówki poziomu drugiego i tak dalej aż do szóstego. Domyślnie stopnie te są wyświetlane coraz mniejszą czcionką, co dostarcza informacji wizualnej o ich ważności.

Długie teksty powinny być dzielone na akapity, przy czym trzeba mieć na uwadze, że akapit to logiczna porcja tekstu, a nie (jak sądzą niektórzy) wcięcie pierwszego wiersza. Prawidłowy podział na akapity dokonywany jest za pomocą znacznika &lt;p&gt;…&lt;/p&gt; i nie należy do przełamywania linii stosować znacznika &lt;br&gt;, ponieważ stanowi to błąd logiczny. Znacznik &lt;br&gt; stosowany jest tylko wówczas, gdy **nie chcemy tworzyć** nowego akapitu, a jedynie przenieść dalszą treść do nowej linii.

Czasem tekst można i należy podzielić na jeszcze mniejsze elementy, na przykład stosując wyliczenia. I ponownie HTML przynosi ze sobą odpowiednie mechanizmy dla dwóch rodzajów wyliczeń: numerowanych i punktowanych. Warto z nich korzystać w sposób ogólnie przyjęty, bo poważnie zwiększają czytelność tekstu. Listy można zagnieżdżać jedne w drugich i przeglądarki internetowe radzą sobie dobrze z takimi sytuacjami. Jednak ponownie muszę ostrzec przed formatowaniem wyłącznie wizualnym: akapity z doklejonymi przed nimi ikonkami **nie są listami, a jedynie je udają!** Formatowanie i ozdabianie list powinno być realizowane przez arkusze stylów.

Wyróżnianie najważniejszych fragmentów tekstu, w szczególności ostrzeżeń może być wykonane za pomocą specjalnych znaczników HTML: &lt;strong&gt; i &lt;em&gt;. Ten pierwszy jest mocniejszy,  
 a drugi (ang. emphasis) słabszy. Na stronie internetowej te fragmenty są wyświetlane inną czcionką, co wyróżnia je z reszty tekstu. Ten sposób jest wygodniejszy niż ręczne formatowanie, ponieważ można dużo łatwiej zarządzać sposobem formatowania wyróżnionych elementów.

## Na zakończenie

Niestety, nie znam sposobu, by napisać tekst interesujący. Jednak powyższe wskazówki pozwolą na napisanie tekstu w sposób bardziej dostępny dla czytelników, a to już sporo. Teksty w Internecie tworzy się bardzo łatwo i często zapomina się o ich jakości. Sam też muszę o tym pamiętać i szkice o dostępności bardzo mi w tym pomagają.