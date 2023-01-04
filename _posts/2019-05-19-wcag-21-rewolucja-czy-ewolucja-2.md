---
id: 2014
title: 'WCAG 2.1: rewolucja czy ewolucja?'
date: '2019-05-19T21:06:08+02:00'
layout: post
guid: 'https://informaton531488923.wordpress.com/?p=2014'
permalink: /2019/05/19/wcag-21-rewolucja-czy-ewolucja-2/
timeline_notification:
    - '1558292769'
publicize_twitter_user:
    - jaczad
publicize_linkedin_url:
    - ''
categories:
    - artykuły
---

W czwartek 16 maja 2019 roku byłem w Opolu na zaproszenie Pawła Starościaka. Po raz drugi organizował konferencję z okazji Global Accessibility Awareness Day (GAAD) i zadał mi temat taki, jak w tytule. Tam opowiedziałem, a tutaj opiszę moje refleksje o WCAG 2.1.

## Trochę historii

Trudno jest znaleźć konkretną datę powstania internetu, ale jedną z powszechniej uznawanych jest 12 marca 1989 roku. Tego dnia Tim Berners-Lee przyszedł do swojego szefa w CERN i pokazał mu swój pomysł na wygodne tworzenie i używanie treści w sieci. Krótko mówiąc – opisał hipertekst i języki z tym związane. Dyrektor dał zielone światło i historia ruszyła. Pojawił się HTML, pierwsza przeglądarka i organizacja pilnująca standardów o nazwie World Wide Web Consortium.

Hasłem tej organizacji jest „internet jest dla wszystkich”. Jednak okazało się, że niektórzy mają problemy w używaniu internetu ze względu na różnego rodzaju ograniczenia fizyczne. W ten sposób Tim Berners-Lee odkrył osoby niepełnosprawne w roku 1993. Zorganizował natychmiast grupę roboczą pod nazwą Web Accessibility Initiative i zobowiązał do znalezienia recepty. Grupa pracowała kilka lat, by w 199 roku przedstawić tą receptę w postaci dokumentu Web Content Accessibility Guidelines 1.0.

WCAG 1.0 to był standard na tamte czasy. Dane były wprowadzane za pomocą klawiatury i myszki, a przekazywane użytkownikowi poprzez wyświetlenie ich na ekranie monitora CRT. Jednak postęp w technologii był tak szybki, że bardzo szybko zauważono, że WCAG 1.0 nie odpowiada na problemy dostępności generowane przez technologie inne, niż HTML, CSS lub JavaScript.

Pojawienie się Flasha, ActiveX, PDF, Silverlight i innych technologii webowych uświadomiło ludziom z WAI, że standard WCAG musi się drastycznie zmienić. Musieli napisać go tak, aby był możliwy do uniwersalnego stosowania, niezależnie od technologii. Już wiedzieli, że nie przewidzą tego, co przyniesie przyszłość czająca się tuż za rogiem. No i napisali, chociaż nie spodziewali się, że napotkają tak duży opór ze strony producentów oprogramowania. Oni dopiero co ogarnęli stosowanie WCAG 1.0, a tu nagle przychodzi taka rewolucja i konieczność dostosowania się do kolejnego, bardziej abstrakcyjnego standardu. Roma locuta – causa finita i standard 2.0 opublikowano w 2008 roku. Ponownie za późno.

Za późno, bo rok wcześniej Steve Jobs pokazał pierwszy model iPhone. Zaczęła się gigantyczna rewolucja mobilna, a w jej ramach wojny pomiędzy systemami operacyjnymi i producentami. Rozkwit Apple, Samsunga i chińskich firm, a jednocześnie schyłek Nokii, RIM i producentów europejskich. Okazało się, że ekran może mieć tylko 3 cale, a do wprowadzania danych może służyć niemal wszystko, co technologia może tylko wymyślić. Poza tym pojawiły się nowe technologie asystujące i coraz lepiej poznawano możliwości i ograniczenia osób z problemami poznawczymi. WCAG trzeba było zaktualizować i to w miarę szybko, a jednocześnie nie wywracając ich do góry nogami, jak zrobiono to wcześniej. Pojawiła się aktualizacja do WCAG 2.1, chociaż wcale nie tak szybko, bo dopiero po kolejnej dekadzie, bo na początku 2018 roku. I z całą pewnością nie była to rewolucja.

## Co przynosi WCAG 2.1?

Autorzy wskazują trzy podstawowe grupy użytkowników objętych aktualizacją: osoby słabowidzące, z problemami poznawczymi i użytkowników urządzeń mobilnych. Ja dostrzegam także uwzględnienie nowych technologii asystujących i w ogóle nowoczesnych sposobów na interakcje z urządzeniem i interfejsem.

W sumie w aktualizacji dodano zupełnie nową wytyczną, których jest obecnie 13 oraz 17 nowych kryteriów sukcesu:

- 5 na poziomie A,
- 7 na poziomie AA,
- 5 na poziomie AAA.

Te liczby sprawiły, że się uśmiechnąłem w duchu, bo natychmiast skojarzyły mi się z haiku. Ta forma literacka polega na napisaniu trójwiersza, na który składa się 17 sylab, dokładnie w takim układzie 5, 7 i 5 w każdym wierszu. To zapewne przypadek, chociaż przyjemny.

Wytyczna 3.5: Sposoby wprowadzania danych, uwzględnia zupełnie nowe sposoby na wprowadzanie danych. Szerzej – chodzi o interakcje użytkownika z interfejsem, zwłaszcza dotykowym. Kilka lat doświadczeń pokazało, gdzie mogą tkwić problemy, zwłaszcza dla osób mających problemy z koordynacją dotyku, wykonywaniem skomplikowanych gestów itp. Jednak urządzenia mobilne to także zupełnie nietypowe metody na obsługę, wykorzystujące różne czujniki, na przykład akcelerometry, żyroskopy, kamery. A przecież informacje można wprowadzać także głosem i ruchami ciała. Tekst można wprowadzać nie tylko za pomocą klawiatury fizycznej i wirtualnej oraz głosem, ale także za pomocą wirtualnej klawiatury Braille’a i pismem ręcznym.

Dla osób słabowidzących przewidziano obowiązek tworzenia tekstu, który będzie się poprawnie zawijał, powiększał, a grafika posiada odpowiedni kontrast.

Ograniczenia poznawcze uwzględniane są między innymi przez takie projektowanie formularzy, by poprawiały wprowadzane dane, o ile to tylko możliwe. Wprowadza też nowy poziom semantyki, to znaczy określanie funkcji danego elementu interfejsu, by odpowiednie oprogramowanie miało możliwość wstawienia ikon wspomagających rozumienie.

Rozwiązania mobilne to konieczność zadbania, by interfejs można było obsługiwać zarówno w układzie poziomym, jak i pionowym. Do tego wykorzystanie dodatkowych czujników powinno dawać się wyłączać, by komuś ze spastycznościami nie uruchamiała się funkcja wymagająca potrząsania. Wreszcie kilka wskazówek dla tworzących interfejsy, by pamiętali o użytkownikach mających mniej sprawne rece.

Technologie asystujące są uwzględnione w kilku kryteriach sukcesu. Sterowanie komendami głosowymi, wymaga tego, by etykiety graficzne były tożsame z etykietami zawartymi w kodzie interfejsu. Dodano też kryterium odnoszące się niemal wprost do technologii ARIA, a zobowiązujące do informowania użytkowników o zmianie stanu w interfejsie, na przykład dodaniu produktu do koszyka. No i wreszcie trzeba pamiętać, by nie pozbawiać użytkowników możliwości korzystania z alternatywnych form korzystania z interfejsu, na przykład pozwalać na pisanie Braillem w polach edycyjnych. To jest szczególnie ważne, gdy programiści podmieniają klawiatury systemowe na własne.

## WCAG 2.1 to ewolucja

Odpowiadając na tytułowe pytanie: WCAG 2.1 to ewolucja, a nie rewolucja. Rewolucję trudno byłoby znowu przeprowadzić. Z drugiej strony – technologia rozwija się tak szybko i w tak nieoczekiwanych kierunkach, że trudno przewidywać wytyczne na przyszłość. W obecne wytyczne słabo wpisują się choćby asystenci głosowi, którzy będą prawdopodobnie przyszłością interfejsów. Czy wpiszą się inne technologie, jak wirtualna i rozszerzona rzeczywistość, internet rzeczy? Nie mam pojęcia i zapewne już głowią się nad tym w konsorcjum i grupie roboczej. Historia pokazuje, że WCAG zawsze są nieco w tyle za aktualnymi technologiami i pewnie już tak zostanie.