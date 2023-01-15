---
id: 1604
title: 'Kody QR, pudełka na mleko i testowanie aplikacji mobilnych'
date: '2017-01-20T15:22:49+01:00'
layout: post
guid: 'http://informaton.pl/?p=1604'
permalink: /2017/01/20/kody-qr-pudelka-na-mleko-i-testowanie-aplikacji-mobilnych/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - iPhone
    - 'kody QR'
    - mobilne
    - niewidomi
    - pomysły
---

Zainspirowała mnie dyskusja na liście osób niewidomych, która zaczęła się od opisów brajlem na opakowaniach, a potem skręciła w kierunku kodów QR. Chodziło o to, czy robić na opakowaniach produktów żywnościowych napisy w brajlu, by pomóc w kupowaniu w sklepach samoobsługowych. Pominę tu wątki główne, chociaż mam na ten temat swoje zdanie, a skupię się na czymś innym. Otóż dla większości osób ważniejsze było rozpoznawanie produktów w domu, niż w sklepie. Opisywano różne domowe sposoby oznaczania produktów w lodówce i spiżarce, aż wreszcie pojawił się temat oznaczania ich kodami QR. Jest to temat interesujący mnie już od kilku lat i teraz to zainteresowanie odżyło. Chcę się zatem poniżej podzielić moimi poszukiwaniami, odkryciami i pomysłami na wykorzystanie kodów QR na potrzeby osób niewidomych.

### Kody QR i kreskowe

Po pierwsze wyjaśnienie, czym są kody QR. Są to kwadratowe grafiki, wydrukowane lub wyświetlane na ekranie, zawierające zakodowaną informację tekstową. Zakodowaną, a nie zaszyfrowaną. Wymyślono je w Japonii do znakowania elementów i opakowań, aby można było je szybko i bezbłędnie identyfikować. Ponieważ były na ten temat wątpliwości, to upewniam, że to nie jest nic w rodzaju kodów CAPTCHA. Czysty tekst jest kodowany specjalnym algorytmem do wzorku składającego się z czarnych i białych kwadracików tworzących duży kwadrat. Algorytm jest dosyć elastyczny i ma 4 poziomy korekcji błędów, a zakodować w pojedynczym kodzie QR można do ok. 4000 znaków. Inne źródła podają 7000 znaków, ale nie wgłębiałem się, na czym polega różnica, bo na tym etapie nie jest to dla mnie ważne.

Różnica pomiędzy kodem QR a kodem kreskowym znanym z opakowań jest istotna. W obu zakodowana jest konkretna informacja, ale kod paskowy zawiera tylko dosyć krótki ciąg cyfr, a kod QR zawierać może niemal dowolną informację tekstową. Dlatego kody kreskowe są zawsze unikalne i muszą być centralnie dystrybuowane, by unikać oznaczania tym samym kodem różnych produktów. Do tego ciąg cyfr trzeba jakoś powiązać z produktem, a zatem skorzystać z bazy danych. Czasami taka baza istnieje, a czasem nie lub jest niedostępna dla postronnych użytkowników. Kody QR działają inaczej, bo zawierają informacje w sobie i nie jest potrzebna żadna zewnętrzna baza danych. Można jednak podejść do nich podobnie jak do kodów kreskowych, o czym za chwilę.

### Dekodowanie informacji w kodzie QR

Do odczytania kodu QR potrzebna jest aplikacja, najlepiej mobilna. Operacja polega na skierowaniu obiektywu kamery na kod QR, a reszty dokonuje już sam program. Tu pojawiają się problemy dotyczące korzystania z kodów QR przez osoby niewidome. Po pierwsze – muszą wiedzieć, że taki kod jest gdzieś umieszczony, a najlepiej jeżeli wiedzą w miarę dokładnie, w którym miejscu. Nawet wtedy nakierowanie obiektywu nie jest bardzo proste, ale już całkiem wykonalne. Po drugie – aplikacja musi działać jak najbardziej automatycznie. Nie może wymagać, by kod QR znajdował się dokładnie pomiędzy liniami wyrysowanymi na ekranie lub by trzeba było zrobić mu zdjęcie. Musi działać jak skaner, któremu podsuwa się obiekt, aon sam analizuje obraz i z radością odkrywa wydrukowany na nim kod i przyjaźnie wibruje informując, że już można sobie przeczytać tekst w nim zaszyty.

Do testów potrzebowałem własnego kodu QR, aby mieć pewność, że dekodowanie jest bezbłędne. Narzędzi do generowania kodów jest ogromnie dużo, w tym generatory online. Są też takie wbudowane w aplikacje odczytujące. Ja musiałem przekombinować, więc poszukałem rozszerzenia do LaTeXa. Tak! Jestem strasznie stary i znam LaTeXa osobiście. Znalazłem bardzo eleganckie rozwiązanie odpowiadające moim potrzebom o nazwie QRCode. Całe użycie to wstawienie w kodzie dokumentu komendy i podania w nawiasach klamrowych tekstu do zakodowania. Działa świetnie i już po chwili miałem kartkę z tajemniczym kwadracikiem ukrytym pomiędzy kilkoma rzędami tekstu. Teraz należało znaleźć odpowiednią aplikację, oczywiście na iPhone.

### Poszukiwanie i testowanie aplikacji

Zacząłem od aplikacji zaprojektowanej specjalnie dla osób niewidomych, jaką jest [Seeing Assistant Home](https://itunes.apple.com/pl/app/seeing-assistant-home/id625146680?mt=8). W zestawie narzędzi jest czytnik kodów QR, ale ja nie byłem w stanie zeskanować mojego kwadracika, nawet gdy wiedziałem gdzie jest. Nie wiem dlaczego, ale po prostu nie dałem rady. Zainstalowałem więc inny specjalizowany program, czyli [QR Voice Sticker](https://itunes.apple.com/pl/app/qr-voice-sticker/id1071148575?mt=8), chociaż w jego bezpłatnej wersji. Ten zadziałał perfekcyjnie jeżeli chodzi o znalezienie i rozkodowanie kodu QR. Irytujące było jedynie zachowanie we współpracy z moją słuchawką BlueTooth. Aplikacja przełączała się na głośnik i to nawet nie główny, tylko telefonu. Synteza mowy była niemal niesłyszalna. Ma to pewnie związek z wykorzystywaniem mikrofonu do tworzenia notatek głosowych. Zaś idea działania warta jest dokładniejszego opisu, który popełnię nieco dalej. Potem sprawdziłem aplikację RedLaser, która działała sprawnie, chociaż jej głównym zastosowaniem jest wspomaganie wydawania pieniędzy. Wreszcie QR Reader Pro, którą posiadam od kilku lat i nadal sprawdza się dobrze w rozpoznawaniu kodów QR, chociaż dostępność interfejsu pozostawia wiele do życzenia. Kilka innych aplikacji nie dało rady, więc ich nazw tu nie wymieniam.

Wrócę teraz na chwilę do aplikacji QR Voice Sticker polskiej firmy Pirs Creative Lab. Jest ona właśnie odpowiedzią na problem rozpoznawania produktów przez osoby niewidome. Idea jest prosta: drukujemy arkusz z kodami QR na papierze samoprzylepnym, wydzieramy pojedyncze kody i naklejamy na opakowanie. Każdy kod jest unikalny, zupełnie jak kody kreskowe, ale nie zawiera żadnej istotnej informacji. To użytkownik dołącza do niego informację nagrywając notatkę głosową przypisaną do konkretnego kodu. W ten sposób aplikacja, napotykając konkretny kod QR, oznajmia nagrany wcześniej komunikat.

Takie podejście ma swoje zalety, a jedyną wadą jest konieczność dodawania własnych komunikatów, czyli tworzenia bazy na własny użytek.

### Co można jeszcze zrobić z kodami QR?

Kody QR interesują mnie od dawna, bo są ciekawym połączeniem pomiędzy światem analogowym i cyfrowym. Mały kwadracik pozwala na wtłoczenie do smartfona informacji, które w innej sytuacji należałoby wpisywać ręcznie. Dają też dostęp osobom niewidomym do materiałów drukowanych, jeżeli sprytnie się ich użyje. Poniżej kilka scenariuszy, jakie mi przyszły do głowy.

1. Konferencje mają to do siebie, że każdy uczestnik dostaje program i inne materiały. Taki papier jest dla osoby niewidomej mało przydatny, więc może brajl… A może umieścić w prawym dolnym rogu programu kod QR zawierający ten sam tekst. Pyk i jest już w smartfonie. Materiały są zbyt obszerne? Nic prostszego – dajemy kod QR z linkiem do strony, gdzie można je przeczytać online. I najważniejsze na konferencjach! Zamiast wyświetlać dane do Wi-Fi na ekranie i prosić o przepisanie sobie hasła “Qx12%zAA2!&amp;PrEv345z” umieszczamy kod z danymi do sieci i już. Jak ktoś chce – może sobie oczywiście kod przepisać.
2. Biurowiec z kilkoma piętrami i ponad setką pokojów. Warto coś zrobić, żeby osoba niewidoma nie plątała się bez sensu. Oczywiście w pierwszej kolejności tabliczka z numerem pokoju wykonana wypukłymi cyframi arabskimi. Robienie pełnego opisu w ten sposób nie ma wielkiego sensu, bo będzie nieczytelnie. Jednak można spokojnie dołożyć kwadratową naklejkę, w której zakodowana będzie informacja, że tu mieści się pokój głównej księgowej Ewy Wittenberg oraz jej dwóch asystentek Anny Szczygielskiej i Moniki Błaszczak. No i oczywiście, że pracują od godziny 8:00 do godziny 18:00.
3. Katalog produktów zawiera fotografie i opisy gadżetów elektronicznych. W prawym dolnym rogu każdej strony mały kod QR kieruje do strony internetowej z produktem. Każdy może skorzystać, nie tylko osoba niewidoma, chociaż ta najbardziej.
4. Formularze urzędowe są udręką dla każdego, ale dla niewidomego przedsiębiorcy są piekłem. Stosik papieru, który pod dotykiem palców nie informuje o swojej zawartości. A trzeba znaleźć druk DRA-1 za czerwiec 2012 roku. Na szczęście w prawym dolnym rogu każdego formularza jest malutki kwadracik, w którym zakodowano symbol formularza oraz datę jego złożenia. Zatem smartfon w garści i przekładamy stos w drugi róg biurka arkusz po arkuszu. Trzeba tylko słuchać i nie narobić nadmiernego bałaganu. Ten pomysł nie jest mój i został wdrożony w drukach związanych z dofinansowaniami do wynagrodzeń niepełnosprawnych pracowników.
5. Kod QR na wizytówce to już rzecz dosyć rozpowszechniona. Sam mam taki na swoich, co bardzo ułatwia życie tym, którzy rozpoznają kwadrat w kropki. Jeden ruch kamerą nad wizytówką i już można dodać wszystkie dane do książki adresowej w smartfonie.

Tak można jeszcze długo. Kody na okładkach książek, pudełkach z płytami, koordynaty GPS na zaproszeniach, spersonalizowane linki do formularzy głosowania, kopertach z dokumentami urzędowymi, a nawet banknotach i biletach. Możliwości są ogromne i tylko je wykorzystywać.