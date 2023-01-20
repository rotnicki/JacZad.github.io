---
title: "Opis koncepcji aplikacji do tworzenia planu"
author: Jacek Zadrożny
date: 2023-01-20
---

# Tablica

Całość narzędzia oparta jest o koncepcję kanban. W tablicy znajdują się 4 kolumny danych, które roboczo nazywam tu "rekomendacje"
. Są to:

1. Rekomendacje
2. Zaplanowane
3. W realizacji
4. Zrobione

Użytkownik dodaje rekomendacje w każdej kolumnie i mają one te same właściwości.

# Rekomendacje

W tej kolumnie jest wszystko wrzucane jak leci. Jakiekolwiek rekomendacje się pojawią, z różnych źródeł. Porządkowanie polega na dodaniu priorytetu, o czym dalej. Każda z rekomendacji ma swoje właściwości i aplikacja wymaga ich uzupełnienia. Są to:

1. Priorytet (krytyczny, wysoki, średni, niski)
2. Czas realizacji w miesiącach i kwartałach.
3. koszt realizacji.
4. Podmiot odpowiedzialny za realizację (jednostka lub osoba)

Po wypełnieniu tych właściwości pojawia się możliwość przeniesienia do kolejnej kolumny Zaplanowane.

# Zaplanowane

W tej kolumnie znajdują się rekomendacje, które zostaną włączone do planu. Właściwości powinny być przeniesione z pierwszej kolumny. Do uzupełnienia jest data rozpoczęcia. Narzędzie powinno podpowiadać poprawne daty, uwzględniając rok budżetowy i ewentualne dotacje.


# W realizacji

Ta kolumna przeznaczona jest do monitorowania postępów. Rekomendacje są przesuwane z kolumny Zaplanowane przez koordynatora. Aplikacja podpowiada, kiedy powinna być przesunięta na podstawie daty rozpoczęcia i czasu trwania.

# Zrobione

W tej kolumnie znajdują się już zrealizowane rekomendacje. Mogą być dodane ręcznie, z uwzględnieniem właściwości rekomendacji. Znajdą się tam także rekomendacje przesunięte z kolumny W realizacji, gdy zostaną zrealizowane.

# Właściwości rekomendacji

## Nazwa

Nazwa powinna być opisowa, a aplikacja powinna podpowiadać gotowe schematy. Być może wręcz gotowe produkty, jeżeli liczba dostawców jest ograniczona. Przykład:

**Usługa tłumaczenia na język migowy online**

## Obszar dostępności

Do wyboru:

- cyfrowa
- architektoniczna
- informacyjno-komunikacyjna
- inny obszar

Do rozważenia, czy jednokrotny, czy wielokrotny wybór.

## Priorytety

- [ ] krytyczny (złamanie przepisów, zagrożenie)
- wysoki (brak dostępu)
- średni (dostęp ograniczony)
- niski (rozwiązania podnoszące dostępność ponad minimalny)

## Harmonogram

Składają się na niego:

- data rozpoczęcia (miesiąc)
- czas trwania (miesiące, kwartały)

## Podmiot odpowiedzialny

Podana jest nazwa komórki, stanowiska lub konkretna osoba. Na przykład:

- wydział komunikacji społecznej
- inspektor BHP
- Agata Gawska

Podmiot odpowiedzialnyo trzymuje dodatkowe pole na adres email. Wypełniający może wysłać informację o aktualnym kształcie rekomendacji z prośbą o komentarz. Podmiot odpowiedzialny nie edytuje treści, tylko otrzymuje podgląd zawartości. Może ją skomentować i zatwierdzić. Zatwierdzone rekomendacje są umieszczane na górze kolumny i oznaczone wizualnie.


## Budżet

Koszt realizacji powinien być podanyw rozbiciu na elementy, zgodnie z planowanym działaniem. Na przykład przy planowaniu budowy windy:

- koszt projektu
- koszt pozwoleń
- koszt budowy windy
- koszt utrzymania (konserwacja)

# Plan

Plan jest generowany na podstawie kanbana. Elementy składowe:

1. Strona tytułowa z danymi metryczkowymi.
2. Opis stanu aktualnego. Dane z kolumny Zrobione i W realizacji.
3. Plan z harmonogramem i budżetem z kolumny Zaplanowane.
4. Rekomendacje do późniejszego wdrożenia z kolumny Rekomendacje. Bez harmonogramu i budżetu
