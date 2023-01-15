---
id: 2099
title: 'ARIA i naprawianie błędów programistycznych'
date: '2021-02-23T17:42:57+01:00'
excerpt: 'Jak naprawić stronę zepsutą przez #ARIA, chociaż przecież lepiej nie psuć.'
layout: post
guid: 'http://informaton.blog/?p=2099'
permalink: /2021/02/23/aria-i-naprawianie-bedow-programistycznych/
publicize_twitter_user:
    - jaczad
timeline_notification:
    - '1614098579'
publicize_linkedin_url:
    - ''
categories:
    - artykuły
tags:
    - ARIA
    - błędy
    - eskrzynka
    - Mastodon
    - przeglądarki
---

Wadliwe stosowanie ARIA może być naprawdę utrudniające w używaniu stron internetowych. Poskarżył się na to niewidomy użytkownik na Facebooku, szukając rozwiązania problemu wadliwie stosowanych atrybutów ARIA. Konkretnie chodziło o aria-hidden, który ukrywa elementy strony przed czytnikami ekranu. Na Mastodon znalazłem pomoc, którą sprawdziłem i teraz dzielę się poradą.

Zadanie było stosunkowo proste – usunąć ze strony atrybuty aria-hidden, żeby móc dotrzeć do ukrytych elementów. W usłudze [eSkrzynka](https://eskrzynka.poczta-polska.pl/#/) wykonano właśnie taką sztukę, przez co nie mogę zalogować się przez profil zaufany. Opisałem mój problem i bardzo szybko otrzymałem skrypt, który należy użyć. Wygląda tak:

```
<pre class="wp-block-code">```
javascript:document.querySelectorAll('[aria-hidden]').forEach(function(e){e.removeAttribute("aria-hidden")})

```
```

Skopiowałem kod do pola adresowego Chrome i nacisnąłem Enter. Nic się nie wydarzyło. Spróbowałem jeszcze raz i znowu nic. Dopiero gdy próbowałem trzeci raz, zauważyłem, że Chrome obcina początek, czyli „javascript:”. Dopisałem z ręki i bingo! Strona objawiła mi przycisk do logowania się przez profil zaufany.

Trochę jednak bez sensu tak to robić za każdym razem. Postanowiłem zastosować tzw. skryptozakładkę. To taka niby zakładka, ale zamiast adresu strony internetowej ma kod do wykonania. Przygotowałem sobie ją w sposób chałupniczy, ale skuteczny. W Chrome uruchomiłem narzędzie „Menedżer zakładek” i znalazłem sobie jakąś zbędną zakładkę. Z menu kontekstowego wybrałem edycję i już miałem otwarte okienko. Skasowałem nazwę i nadałem nową: „Odkryj zakryte”, a na miejsce adresu do strony wkleiłem kod skryptu. Zapisałem i na tym koniec. Mam zakładkę, która pozwala pozbyć się źle użytego atrybutu ARIA.

Jeszcze raz dziękuję użytkownikowi <https://tupot.pl/@rxb> za pomoc i ponownie żałuję, że sam nie umiem programować. Bo pewnie przydałoby się całe rozszerzenie do przeglądarki usuwające takie przeszkadzajki. A wcześniej – informujące, że takie na stronie się znajdują. Przypomnę bowiem, że użycie aria-hidden całkowicie ukrywa taki obiekt przed niewidomym użytkownikiem, który nawet nie wie o jego istnieniu.