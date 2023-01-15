---
id: 667
title: 'Kody obrazkowe CAPTCHA są niezgodne z WCAG 2.0'
date: '2013-04-12T08:45:02+02:00'
layout: post
guid: 'http://informaton.pl/?p=667'
permalink: /2013/04/12/kody-obrazkowe-captcha-sa-niezgodne-z-wcag-2-0/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - błędy
    - CAPTCHA
    - grafika
    - słuch
    - 'tekst alternatywny'
    - 'WCAG 2.0'
    - wzrok
---

Jestem zdecydowanym przeciwnikiem kodów zabezpieczających typu obrazkowego i uważam że [należy zapomnieć o przepisywaniu kodów](http://informaton.pl/?p=143)dla udowodnienia swego człowieczeństwa. Jednak te kody są dopuszczalne według specyfikacji WCAG 2.0, chociaż są niezgodne z jej zapisami. Przyczyna jest dla mnie dosyć jasna – te kody są zbyt popularne, by ich po prostu zabronić. Jednak moim zdaniem jest to zwykłe asekuranctwo.

WCAG 2.0 dopuszcza w [kryterium sukcesu 1.1.1](http://informaton.pl/?p=19)stosowanie obrazkowych kodów CAPTCHA. Robi to okrężną drogą, bo nakazuje, by treść zawartą w kodzie dostarczyć za pomocą innych zmysłów. Nie przychodzi mi do głowy inny sposób, niż słuch, bo dotyk, smak i węch raczej odpadają. Jednak dostarczenie zaszumionego nagrania z angielskimi fonemami nie rozwiązuje problemu osób głuchoniewidomych czy obcojęzycznych. Biorąc pod uwagę fakt, że SC 1.1.1 jest obowiązkowe dla podstawowego poziomu dostępności A – jest to raczej błąd w specyfikacji.

Jednak ta forma odróżniania człowieka od komputerów narusza też inne zapisy WCAG, a zatem można spokojnie przyjąć, że jej stosowanie powoduje niezgodność z tą specyfikacją. Nie spełnia na przykład [kryterium sukcesu 1.4.5](http://informaton.pl/?p=150), które umieszczono na poziomie dostępności AA. Zobowiązuje ono do tego, by stosować jawny tekst, a nie obraz tekstu, jeżeli tylko technologia na to pozwala. Tutaj nie ma żadnych przeszkód technologicznych. Są tu oczywiście dwa zastrzeżenia, z których pierwsze mówi o możliwości dostosowania wyglądu obrazkowego tekstu do potrzeb użytkownika, co oczywiście nie zachodzi w wypadku kodów CAPTCHA. Drugi warunek dopuszcza stosowanie obrazów tekstu, o ile sposób prezentacji jest kluczowy dla zrozumienia informacji. Tu zaś zachodzi sytuacja odwrotna – sposób prezentacji **utrudnia** zrozumienie informacji.

Jeżeli przyjrzymy się [kryterium sukcesu 1.3.3](http://informaton.pl/?p=116), to stwierdzimy, że kod obrazkowy nie spełnia także tego kryterium. Informacja kluczowa dla interakcji oparta jest **wyłącznie** na zmysłach. W pierwszej kolejności jest to wzrok, a w drugiej – słuch. Co więcej – to kryterium sukcesu znajduje się na poziomie A dostępności, a zatem jest sprzeczne z SC 1.1.1, które dopuszcza kody CAPTCHA.

Wcale nie jest mi przyjemnie wskazywać sprzeczności we WCAG 2.0, bo to ważny dla dostępności dokument. Pokazuje on jednak, że autorzy uginają się czasem przed zastanymi zwyczajami. Wydaje się jednak, że w następnej wersji WCAG kody obrazkowe i dźwiękowe powinny zostać zabronione.