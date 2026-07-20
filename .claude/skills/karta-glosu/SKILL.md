---
name: karta-glosu
description: Buduje kartę głosu (tone of voice) użytkownika z jego własnego materiału - nagrań, transkrypcji rozmów, contentu albo maili. Jeśli materiału nie ma, przeprowadza wywiad i buduje kartę z odpowiedzi. Efekt to plik karta-glosu.md, który leży w projekcie i sprawia, że AI pisze tonem użytkownika zamiast medianą internetu. Wywołaj, gdy użytkownik mówi "karta głosu", "tone of voice", "chcę żeby AI pisało jak ja", "moje teksty brzmią jak AI", "/karta-glosu", albo gdy prosi o tekst i widać, że nie ma w projekcie pliku z jego głosem.
---

# Karta głosu

## Po co to jest

AI nie pisze źle. AI pisze **medianą internetu**, czyli średnią z tego, co przeczytało. Średnia nie ma głosu.

Polecenie "pisz swobodnie i przyjaźnie" nic nie zmienia, bo to dalej opis, a nie dowód. Karta głosu ma zawierać **konkretne słowa, zdania i konstrukcje** użytkownika. Wtedy AI ma się do czego odwołać zamiast zgadywać.

Twoja rola: wydobyć te dowody i zapisać je w pliku, którego użytkownik będzie realnie używał.

---

## Zasady, których nie łamiesz

1. **Nie wymyślasz głosu użytkownika.** Wszystko, co trafia do karty, musi pochodzić z jego materiału albo z jego odpowiedzi w wywiadzie. Zero "typowych zwrotów dla trenera".
2. **Cytujesz dosłownie.** Marker to konkretne słowo, które padło, nie parafraza. Jeśli ktoś mówi "co nie?", w karcie jest "co nie?", nie "zwrot potwierdzający".
3. **Materiał mówiony bije pisany.** Gdy ktoś pisze, wygładza się do średniej, zanim ktokolwiek to przeczyta. Gdy mówi, nie ma na to czasu. Zawsze preferuj nagrania i transkrypcje nad tekstami.
4. **Jeśli czegoś nie widzisz w materiale, zostawiasz puste** i oznaczasz `[do uzupełnienia]`. Nie wypełniasz sekcji dla kompletności.
5. **Nie oceniasz sposobu mówienia.** Wypełniacze, urwane zdania i dygresje to nie wady. To materiał, z którego część zachowujesz, a część wycinasz w sekcji 8.
6. Polskie znaki wszędzie. Zero długich myślników w tekstach, jakie generujesz.

---

## Krok 1: sprawdź, co użytkownik ma

Zacznij od jednego pytania, nie od listy:

> Zanim zaczniemy: masz gdzieś nagrania albo transkrypcje, w których mówisz o swojej pracy? Nagrania głosowe, zapisy spotkań, live'y, cokolwiek. Jeśli nie, zbudujemy kartę z wywiadu i to też zadziała.

Cztery miejsca, o których warto przypomnieć, jeśli użytkownik mówi "chyba nic nie mam":

- **Refleksje głosowe** - pięć minut do telefonu. Najszybsza droga, jeśli zaczynasz od zera.
- **Transkrypcje rozmów** - Fireflies, Zoom, Google Meet. Konsultacje i spotkania z klientami. Tam mówisz najbardziej sobą, bo nie myślisz o tym, jak brzmisz.
- **Twój content** - posty, rolki, live'y, webinary. Godzina nagrania to setki Twoich zdań.
- **Twoje maile** - setki wiadomości pisanych Twoim tonem, na które ktoś realnie odpisał.

Dalej idziesz jedną z dwóch ścieżek.

---

## Ścieżka A: użytkownik ma materiał

**1. Zbierz pliki.** Poproś o wskazanie ścieżek albo wklejenie treści. Przy transkrypcjach z rozmów wielu osób **analizuj wyłącznie wypowiedzi użytkownika**, resztę pomijasz. Powiedz mu, że tak robisz.

**2. Przeczytaj wszystko, zanim zaczniesz pisać kartę.** Nie streszczaj w locie.

**3. Zliczaj, nie szacuj.** Przy markerach podawaj kolejność według realnej częstotliwości. Jeśli masz dużo materiału, policz wystąpienia (grep, prosty skrypt), zamiast zgadywać.

**4. Wypełnij osiem sekcji** wzorując się na strukturze poniżej.

**5. Pokaż użytkownikowi, co znalazłeś, zanim zapiszesz plik.** Krótko, w punktach. Zapytaj: "rozpoznajesz się w tym?". Ludzie często nie wiedzą, że mówią jakieś słowo, i to jest właśnie ten moment, w którym karta staje się ich.

---

## Ścieżka B: brak materiału, robisz wywiad

Zadawaj pytania **pojedynczo**, nie hurtem. Po każdej odpowiedzi notuj nie tylko treść, lecz także **jak** została powiedziana: jakie słowa wracają, jak długie są zdania, czy pojawiają się analogie.

To jest kluczowe: w tej ścieżce materiałem są **odpowiedzi użytkownika w tej rozmowie**. Im dłużej pisze, tym lepszą kartę dostanie.

Pytania, w tej kolejności:

1. Opowiedz, czym się zajmujesz, tak jakbyś tłumaczył to koledze przy stole. Nie jak na stronie internetowej.
2. Jaki problem najczęściej przynoszą Ci klienci? Powiedz to ich słowami, nie swoimi.
3. Opowiedz o kliencie, któremu ostatnio realnie pomogłeś. Co było na wejściu, co na wyjściu.
4. Czego w swojej branży nie znosisz? Co Cię wkurza w tym, jak inni to robią?
5. Jak zaczynasz rozmowę z kimś nowym? A jak ją kończysz?
6. Masz jakieś swoje określenia, których używasz na to, co robisz? Rzeczy, które nazywasz po swojemu?
7. Kiedy piszesz do klienta, a kiedy do znajomego z branży, co się zmienia w Twoim tonie?

Po siódmym pytaniu zaproponuj: *jeśli chcesz mocniejszą kartę, nagraj teraz pięć minut o tym, co dziś robiłeś, i wklej transkrypcję. Wtedy dołożę do niej Twój prawdziwy rytm mówiony.*

---

## Struktura karty: osiem sekcji

Zapisujesz do `karta-glosu.md` w katalogu głównym projektu.

### 1. Rdzeń: markery, które są podpisem

Lista słów i zwrotów wracających w każdym źródle, **posortowana według częstotliwości**. Przy każdym krótko: co ta osoba tym robi.

Przykład zapisu:
```
1. "co nie?" - domknięcie myśli, szuka potwierdzenia
2. "na zasadzie" - wprowadza przykład albo scenariusz
3. "koniec końców" - wprowadza puentę, realizm
```

### 2. Składnia i rytm

Jak zbudowane są zdania. Konkretnie:
- Długość i sposób budowania (kaskadowe doklejanie czy krótkie cięcia)
- Czy jest rytm naprzemienny (długie tłumaczenie, potem krótkie przybicie)
- Czy urywa i restartuje myśl
- Czy strukturyzuje liczbami ("to jest raz", "po pierwsze")

### 3. Otwarcia, przejścia, zamknięcia

Dosłowne cytaty. Jak wita, jak przechodzi między tematami, jak kończy. To sekcja, która najbardziej ratuje pierwsze i ostatnie zdanie tekstu.

### 4. Własny słownik

Autorskie pojęcia, metafory i nazwy, których używa na swoje rzeczy. Jeśli ktoś nazwał coś po swojemu, to jest złoto: nikt inny tak nie mówi.

### 5. Jak tłumaczy

Czy zaczyna od definicji, czy od analogii. Czy pokazuje na ekranie. Czy sprawdza zrozumienie i jak ("czy to brzmi sensownie?", "na jakim jesteśmy etapie?").

### 6. Jak sprzedaje

Czy naciska, czy pokazuje dowód. Czy odradza rzeczy. Jak mówi o cenie. Ta sekcja decyduje o tonie ofert i maili, więc nie pomijaj jej, nawet jeśli materiał jest skąpy.

### 7. Rejestr

Gdzie luźno, gdzie formalnie. Co się zmienia między rozmową z klientem, postem publicznym a mailem do partnera biznesowego.

### 8. Destylacja: mowa na pismo

**Sekcja, której prawie nikt nie robi, i bez której karta nie zadziała.**

Dwie kolumny:

**Zachowaj** - rytm, analogie, własny słownik, szczerość o wątpliwościach, sposób domykania.

**Wytnij** - wypełniacze (wypisz konkretnie, które i jak często padają), urwane zdania, poprawki w locie, powtórzenia z mowy.

Bez tej sekcji AI zwróci transkrypcję udającą tekst. Z nią zwraca tekst, który brzmi jak ta osoba w dobrym dniu.

---

## Krok ostatni: test A/B

Po zapisaniu karty **zaproponuj test**, nie kończ na pliku:

> Zrobimy jedno sprawdzenie. Daj mi temat, o którym mógłbyś napisać post albo maila.

Potem:
1. Napisz tekst **bez odwoływania się do karty**. Zwykły, generyczny prompt.
2. Napisz ten sam tekst **z kartą**, wskazując konkretną sekcję, na przykład destylację.
3. Połóż oba obok siebie i zapytaj, który brzmi jak on.

Dopóki użytkownik nie zobaczy różnicy obok siebie, nie uwierzy, że to działa.

---

## Jak używać karty na co dzień (powiedz to użytkownikowi)

Źle:
```
Napisz post o tone of voice.
```
Dostaje medianę internetu z emoji i trzema przykładami.

Dobrze:
```
Napisz akapit do newslettera na podstawie tej refleksji.
Trzymaj się mojej karty głosu, sekcja destylacja mowa na pismo.
Jedno zdanie na linię, bez wypełniaczy.
```

Kartę robisz raz. Materiał nagrywasz co tydzień. Na tym polega różnica między pisaniem a redagowaniem.

---

## Odświeżanie karty

Karta nie jest wieczna. Zaproponuj powrót do niej, gdy:
- uzbiera się kilka nowych godzin nagrań,
- użytkownik zmienia odbiorcę albo ofertę,
- zauważy, że teksty zaczynają brzmieć obok niego.

Wtedy nie piszesz karty od zera. Dokładasz nowe cytaty i usuwasz te, które przestały wracać.
