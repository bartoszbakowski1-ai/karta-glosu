# Karta głosu

Twój głos już istnieje. Nie musisz go wymyślać, tylko wydobyć i zapisać.

To repo daje Ci skill do Claude Code, który przeprowadzi Cię przez wywiad i zbuduje **Twoją kartę głosu**: plik, który leży w projekcie i sprawia, że AI przestaje pisać medianą internetu, a zaczyna pisać Twoim tonem.

Materiał z live #6 cyklu "Zbuduj własny system AI" (20.07.2026).

---

## Co dostajesz

| Plik | Do czego służy |
|---|---|
| `.claude/skills/karta-glosu/SKILL.md` | Skill, który przeprowadza wywiad i buduje kartę |
| `szablon-karty-glosu.md` | Pusty szablon 8 sekcji, jeśli wolisz wypełnić ręcznie |
| `przyklad-karty.md` | Skrócony przykład wypełnionej karty |
| `przyklad-przed-po.md` | Ten sam temat napisany bez karty i z kartą |
| `jak-zebrac-material.md` | Cztery miejsca, w których siedzi Twój głos |

---

## Jak zacząć

Uruchomienie zajmuje około 5 minut. Szybka karta startowa powstaje w 10-15 minut, a pełny wywiad zwykle zajmuje 20-40 minut.

**1. Pobierz to repo.**

Jeśli masz Claude Code, po prostu poproś go w folderze, w którym pracujesz:

```
Sklonuj https://github.com/bartoszbakowski1-ai/karta-glosu do katalogu tymczasowego.
Utwórz w moim projekcie brakujące katalogi i skopiuj .claude/skills/karta-glosu do .claude/skills/karta-glosu.
Nie nadpisuj innych skilli. Na końcu sprawdź, czy skill jest widoczny.
Jeśli potrzebny jest restart Claude Code albo brakuje jakiejś funkcji, powiedz mi dokładnie, co mam zrobić.
```

Ręcznie, w terminalu macOS, Linux albo Git Bash:

```bash
git clone https://github.com/bartoszbakowski1-ai/karta-glosu.git
mkdir -p "TWOJ-PROJEKT/.claude/skills"
cp -R karta-glosu/.claude/skills/karta-glosu "TWOJ-PROJEKT/.claude/skills/"
```

**2. Odpal skill w Claude Code:**

```
/karta-glosu
```

Jeśli slash nie zadziała, napisz normalnie: `uruchom skill karta-glosu`.

Jeśli Claude nadal go nie widzi, wklej:

```
Sprawdź, dlaczego skill karta-glosu nie jest widoczny.
Zweryfikuj ścieżkę .claude/skills/karta-glosu/SKILL.md i powiedz mi, czy muszę ponownie uruchomić Claude Code.
```

**3. Odpowiadaj na pytania.**

Skill najpierw przygotuje bazowy tekst do późniejszego porównania, a potem sprawdzi, jaki masz materiał.

- Jeśli masz transkrypcje rozmów, live'ów albo nagrań, użyje ich.
- Jeśli masz tylko plik audio, sprawdzi, czy Twój Claude Code potrafi go przetworzyć. Jeśli nie, powie, czego brakuje i poprosi o transkrypcję.
- Jeśli nie masz materiału, zaproponuje szybki albo pełny wywiad.

**4. Na końcu dostajesz plik `karta-glosu.md`.**

Zostawiasz go w projekcie. Od tej pory przy każdej prośbie o tekst mówisz: *trzymaj się mojej karty głosu*.

---

## Prywatność przed startem

Karta może zawierać cytaty, informacje o klientach i fragmenty prywatnych rozmów.

- Analizuj tylko swoje wypowiedzi.
- Usuń nazwiska, adresy, numery telefonów i poufne informacje.
- Nie używaj rozmów z klientami bez zgody, jeśli zawierają ich dane albo tajemnice biznesowe.
- Surowe materiały trzymaj w folderze `materialy-glosu-prywatne/`.
- Zdecyduj, czy karta ma być prywatna, zanim dodasz ją do GitHuba.

Skill przypomni Ci o tym przed zapisaniem pliku i może pomóc dodać prywatne materiały do `.gitignore`.

---

## Nie masz żadnego materiału? Zacznij od tego

Nagraj trzy razy po pięć minut. Bez planu, bez przygotowania. Możesz użyć dyktafonu, notatki głosowej albo funkcji głosowej w Claude Code.

Tematy, które działają najlepiej:

- Co dziś realnie robiłeś w pracy i co Cię w tym zaskoczyło.
- Wytłumacz swoją usługę tak, jakbyś tłumaczył ją koledze przy piwie.
- Opowiedz o kliencie, któremu ostatnio pomogłeś. Co było jego problemem, co zrobiliście.

To wystarczy. Mówisz swoim głosem codziennie, w każdej rozmowie. Chodzi tylko o to, żeby to nagrać i dostarczyć Claude'owi transkrypcję.

---

## Uczciwy test przed i po

Skill tworzy tekst bazowy **zanim** przeczyta Twoje materiały i przeprowadzi wywiad. Po zbudowaniu karty używa dokładnie tego samego tematu i formatu.

Porównujesz dwa teksty:

1. Bez karty i bez wiedzy z wywiadu.
2. Z gotową kartą głosu.

Dzięki temu różnica nie wynika tylko z tego, że Claude chwilę wcześniej z Tobą rozmawiał. Zobacz też gotowy [`przyklad-przed-po.md`](przyklad-przed-po.md).

---

## Osiem sekcji karty

1. **Rdzeń** - słowa i markery, które są Twoim podpisem
2. **Składnia i rytm** - jak budujesz zdania
3. **Otwarcia i zamknięcia** - jak zaczynasz i kończysz
4. **Własny słownik** - Twoje pojęcia i metafory
5. **Jak tłumaczysz** - analogie, przykłady, sprawdzanie zrozumienia
6. **Jak sprzedajesz** - bez nacisku, dowodem
7. **Rejestr** - gdzie luźno, gdzie formalnie
8. **Destylacja mowa na pismo** - co zachowujesz, co wycinasz

Ósma sekcja jest tą, której prawie nikt nie robi, i tą, bez której karta nie zadziała. Szczegóły w skillu.

---

## Licencja

MIT. Rób z tym, co chcesz.

Zbudowane przez [Bartka Bąkowskiego](https://bartbakowski.com). Cały cykl live: [bartbakowski.com/webinary](https://bartbakowski.com/webinary).
