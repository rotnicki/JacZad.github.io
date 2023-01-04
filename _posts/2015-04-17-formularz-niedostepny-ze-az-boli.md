---
id: 1303
title: 'Formularz niedostępny, że aż boli.'
date: '2015-04-17T10:22:23+02:00'
layout: post
guid: 'http://informaton.pl/?p=1303'
permalink: /2015/04/17/formularz-niedostepny-ze-az-boli/
restapi_import_id:
    - 5ca8405547793
categories:
    - artykuły
tags:
    - etykiety
    - formularze
    - klawiatura
    - semantyka
    - Warszawa
---

Urząd m. st. Warszawy organizuje co roku konkurs, w którym wybierana jest najlepsza inicjatywa organizacji pozarządowej. Pomysł jest fajny i taka nagroda mile łechce organizacje ze stolicy, gdy zostaną docenione. Ja też chciałem zagłosować na projekt Fundacji Kultury bez barier “Zabierz laskę do kina”, bo dotyczy dostępności, chociaż mało cyfrowej. No i wtedy napotkałem na [formularz](http://ngo.um.warszawa.pl/konkurs/)tak niedostępny, że aż zabolało mnie dostępnościowe serce.

Nie potrafię skopiować tego formularza, a przydałby mi się jako przykład złej praktyki. W zasadzie wszystko jest tam zrobione źle z punktu widzenia dostępności, a do tego jest to praktycznie ograniczające, bo osoba niewidoma **nie jest w stanie tego formularza wypełnić**. Ja zagłosowałem, ale wciąż nie mam pewności, czy na ten projekt, na który chciałem. Formularz pewnie wkrótce zniknie ze strony, więc śpieszcie się oglądać.

Zacznijmy od semantyki. W formularzu trzeba wybrać kategorię, a po jej wybraniu – konkretny projekt. Dlaczego realizowane jest to przez przycisk, a nie listę rozwijaną lub pola radiowe? No bo przecież można zrobić rozwijane menu, co wygląda bardzo nowocześnie. Owszem, ale semantyki w tym za grosz. Teraz klawiatura – elementy menu nie są oczywiście dostępne z jej poziomu, a tylko za pomocą myszki, a zatem poległo [kryterium 2.1.1.](http://informaton.pl/wcag-2-0/dostep-za-pomoca-klawiatury-wcag-2-0-sc-2-1-1-poziom-a/)Czytniki ekranu czasem pozwalają ominąć ten problem i w ten sposób wybrałem kategorię. Jednak o fakcie prawidłowego wyboru mogłem wnioskować tylko przez projekty wyświetlone w kolejnym menu. Gdy wybierałem projekt nie miałem już żadnej podpowiedzi. Zatem [kryterium sukcesu 4.1.2](http://informaton.pl/wcag-2-0/nazwa-rola-i-wartosc-wcag-2-0-sc-4-1-2-poziom-a/)też zostało pominięte. Nie tylko w tym miejscu, bo przyokazji warto wspomnieć o polu wyboru, które należało zaznaczyć wyrażając zgodę na przetwarzanie danych osobowych. Otóż tego pola wyboru wcale nie było! A dokładniej – nie było go w drzewie DOM, a zatem nie było o nim żadnej informacji.

Pojawiły się także bardziej standardowe błędy, to znaczy brak etykiet do pól edycyjnych, których na szczęście nie było zbyt dużo i jakoś dały się ogarnąć. Potem oczywiście okienka modalne, bo przecież robimy nowocześnie, z komunikatami o błędach. Tylko zapomniano o ARIA i okienko trzeba było obmacać. Mógłbym znowu przytoczyć złamane kryteria sukcesu dotyczące etykiet, ale już mi się nie chce. Na koniec nie dano mi możliwości potwierdzenia moich decyzji, chociaż podawałem swoje dane osobowe, choćby za pośrednictwem emaila potwierdzającego. No i już…

Natychmiast zgłosiłem problem na adres ngo@um.warszawa.pl, ale nie doczekałem się odpowiedzi. Za to ktoś inny przesłał mi odpowiedź, jaką uzyskał z tego samego miejsca i w tej samej sprawie. Otóż formularza nie da się już zmienić, a jak ktoś ma problem z jego wypełnieniem – może zadzwonić lub przyjść do Centrum Komunikacji Społecznej, a oni pomogą. Gratuluję podejścia. Może zatem po prostu zdjąć formularz i wszyscy niech dzwonią i przychodzą, by zagłosować. A jeszcze bardziej rozsierdziła mnie deklaracja, że za rok Zrobią dostępny formularz, <q>jeżeli będą możliwości techniczne</q>. Otóż drodzy Państwo – [rozporządzenie o Krajowych Ramach Interoperacyjności](http://informaton.pl/strony-internetowe/dostepnosc-zapisana-w-rozporzadzeniu/)obowiązuje także Was! Możliwości techniczne istnieją od zawsze i trzeba tylko zrobić porządnie, a nie na odwal się. A za rok nikt nie będzie pamiętał o żadnej deklaracji i opublikowany zostanie podobny syf internetowy, bo przecież sprawdził się rok wcześniej. Odcieliście od głosowania niewidomych mieszkańców Warszawy, dla których udostępnianie kultury jest ważne i na pewno nie zagłosują na niego. Na stronie formularza nie ma żadnej informacji o możliwości dzwonienia. I po raz kolejny urzędnicy mają w nosie swoje obowiązki, przepisy prawne i niepełnosprawnych obywateli.