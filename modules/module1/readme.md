# Ćwiczenie 1 – Wprowadzenie do baz danych NCBI i informacji biologicznej

## Wprowadzenie

Współczesna bioinformatyka opiera się na analizie ogromnych zbiorów danych biologicznych: sekwencji DNA, RNA, białek oraz publikacji naukowych. Dane te są przechowywane w wyspecjalizowanych bazach danych, które umożliwiają ich przeszukiwanie, filtrowanie oraz analizę.

Jednym z najważniejszych systemów tego typu jest NCBI (National Center for Biotechnology Information), który udostępnia m.in.:

- bazę publikacji naukowych (PubMed),
- bazę sekwencji nukleotydowych (Nucleotide),
- bazę sekwencji białkowych (Protein).

Celem ćwiczenia jest:
- zapoznanie się z interfejsem i możliwościami baz danych NCBI,
- nauka formułowania zapytań (kwerend),
- zrozumienie, jak filtrowanie wpływa na wyniki wyszukiwania,
- interpretacja liczby rekordów w kontekście biologicznym.

[![Watch the video](https://img.youtube.com/vi/QIZ8QH6JcC8/0.jpg)](https://youtu.be/QIZ8QH6JcC8?v=QIZ8QH6JcC8)

---

## Zadanie 1.1 – Analiza publikacji naukowych: świat, Polska i UWM w Olsztynie

### Cel  
Zapoznanie się z mechanizmem wyszukiwania literatury naukowej oraz krytyczną analizą danych bibliograficznych w kontekście geograficznym i instytucjonalnym.

---

### Wprowadzenie  

Wyobraź sobie, że chcesz rozpocząć badania naukowe w dziedzinie, która szczególnie Cię interesuje.  

Zanim wybierzesz temat pracy dyplomowej lub projekt badawczy, chcesz odpowiedzieć na kilka kluczowych pytań:

- Jak duży jest zasób wiedzy w tej dziedzinie na świecie?  
- Jak wygląda aktywność publikacyjna w Polsce?  
- Czy w Twoim mieście lub na Twojej uczelni prowadzone są badania w tym obszarze?  
- Czy możesz znaleźć potencjalnego promotora lub zespół badawczy?  

Do tego celu wykorzystasz bazę PubMed.

---

### Wykonaj  

1. Wybór tematu  

   Wybierz samodzielnie temat badawczy (jedno słowo lub krótka fraza), który Cię interesuje.  
   Unikaj korzystania z przykładów innych osób – wybierz coś, co rzeczywiście Cię ciekawi.

---

2. Analiza globalna (świat)  

   Wyszukaj publikacje dla wybranego tematu.

   Zanotuj:
   - liczbę wszystkich rekordów (bez filtrów)

---

3. Analiza dla Polski  

   Zmodyfikuj zapytanie, dodając filtr:
   - afiliacja: Poland  

   Zanotuj:
   - liczbę rekordów  

---

4. Analiza dla UWM w Olsztynie  

   Spróbuj zawęzić wyniki do afiliacji związanych z Uniwersytetem Warmińsko-Mazurskim.

   W tym celu przetestuj różne warianty zapytań (np. nazwa uczelni, miasto, skróty, różne wersje językowe).

   Zanotuj:
   - wszystkie użyte warianty zapytań  
   - liczbę rekordów dla każdego wariantu  

---

5. Analiza krytyczna afiliacji  

   Odpowiedz na pytania:

   - Czy zapis afiliacji w bazie danych jest jednoznaczny?  
   - Czy wszyscy naukowcy używają tej samej nazwy instytucji?  
   - Jakie problemy pojawiają się przy wyszukiwaniu po afiliacji?  
   - Jak wpływa to na wiarygodność wyników?  

---

6. Rozszerzenie zapytania  

   Dodaj drugi termin biologiczny (tworząc bardziej szczegółowe zapytanie).

   Powtórz analizę dla:
   - świata  
   - Polski  
   - UWM  

---

7. Zestawienie danych  

   Utwórz tabelę zawierającą:

   - zapytanie  
   - liczba publikacji (świat)  
   - liczba publikacji (Polska)  
   - liczba publikacji (UWM – różne warianty)  

---

8. Wizualizacja danych  

   Wykonaj wykres przedstawiający:

   - porównanie liczby publikacji: świat vs Polska vs UWM  

   Wybierz odpowiednią formę (np. wykres słupkowy).

---

### Wyniki  

- wszystkie użyte zapytania (kwerendy)  
- liczby rekordów  
- tabela porównawcza  
- wykres  

---

### Wnioski  

- Jak wygląda udział Polski w globalnej produkcji naukowej w wybranej dziedzinie?  
- Jak wygląda aktywność publikacyjna UWM na tle Polski?  
- Czy można łatwo zidentyfikować badaczy z konkretnej uczelni?  
- Jakie są ograniczenia wyszukiwania po afiliacji?  
- Czy liczba publikacji odzwierciedla realną aktywność badawczą?  

---

### Zadanie dodatkowe – dynamika publikacji w czasie  

Spróbuj przeanalizować, jak zmieniała się liczba publikacji w czasie.

#### Wykonaj:

1. Podziel zakres lat:
   - od roku Twojego urodzenia do roku bieżącego  

2. Zbierz dane:
   - liczba publikacji dla wybranego tematu w kolejnych latach  
   (możesz użyć filtrów dat lub zapytań z zakresem lat, np. 2010:2015)

3. Utwórz tabelę:
   - rok / zakres lat  
   - liczba publikacji  

4. Wykonaj wykres:
   - liczba publikacji w funkcji czasu  

---

#### Wnioski:

- Czy liczba publikacji rośnie, maleje czy jest stabilna?  
- Czy można wskazać momenty gwałtownego wzrostu?  
- Jak można interpretować te zmiany w kontekście rozwoju nauki?  

---

### Pytanie otwarte  

Czy uważasz, że liczba publikacji jest dobrym wskaźnikiem rozwoju danej dziedziny? Uzasadnij swoją odpowiedź.
---

## Zadanie 1.2 – Analiza ilościowa sekwencji w bazie Nucleotide

### Cel  
Poznanie struktury bazy sekwencji nukleotydowych oraz wpływu filtrów na wyniki wyszukiwania.

---

### 🔧 Wykonaj  

1. Wejdź do bazy NCBI Nucleotide.  

2. Wyszukaj wszystkie rekordy dla organizmu:
   - *Homo sapiens*

3. Zanotuj:
   - liczbę wszystkich rekordów  

4. Zawęź wyszukiwanie:
   - długość sekwencji < **XXXX**  
     (XXXX = cztery ostatnie cyfry Twojego numeru indeksu)

5. Wyszukaj osobno:
   - sekwencje kodujące białka  
   - sekwencje niekodujące  

6. Dodaj filtr:
   - rekordy opublikowane od roku Twojego urodzenia  

---

### Wyniki  
- liczba rekordów dla każdej kombinacji filtrów  
- dokładne zapytania (zakładka „Advanced” lub „Search details”)  

---

### Wnioski  
- czym różnią się sekwencje kodujące i niekodujące?  
- dlaczego liczba rekordów zależy od długości sekwencji?  
- jakie znaczenie biologiczne mają sekwencje niekodujące?  

---

## Zadanie 1.3 – Wyszukiwanie i zapis sekwencji białkowych (Protein)

### Cel  
Nauczenie się selekcji danych biologicznych oraz ich zapisu w standardowych formatach.

---

### Wykonaj  

1. Wejdź do bazy NCBI Protein.  

2. Wyszukaj białka zawierające wybrane słowo kluczowe  
   (np. „kinase”, „hemoglobin”, „cytochrome”).

3. Zanotuj:
   - liczbę wszystkich rekordów  
   - liczbę rekordów w bazie RefSeq  

4. Ogranicz wyniki:
   - do maksymalnie 10 rekordów (używając filtrów i operatorów logicznych)

5. Wybierz:
   - 1 rekord  
   - 2 rekordy  
   - wszystkie (max 10)

6. Zapisz dane w formacie FASTA:
   - plik z 1 sekwencją  
   - plik z 2 sekwencjami  
   - plik ze wszystkimi sekwencjami  

7. (Dodatkowo) zapisz te same dane jako pliki `.txt` i porównaj je.

---

### Wyniki  
- liczba rekordów (pełna i ograniczona)  
- zastosowane zapytania  
- zapisane pliki FASTA  

---

### Wnioski  
- czym różni się baza RefSeq od pozostałych danych?  
- dlaczego ograniczenie liczby wyników jest ważne?  
- czym różni się zapis FASTA od zwykłego tekstu?  

---

## Zadanie 1.4 – Analiza pojedynczego rekordu biologicznego

### Cel  
Zrozumienie struktury rekordu biologicznego i jego znaczenia w analizie bioinformatycznej.

---

### Wykonaj  

1. Wybierz jeden rekord z zadania 1.3.  

2. Otwórz go w pełnym widoku (np. GenPept).

3. Zidentyfikuj i opisz:
   - numer akcesyjny  
   - nazwę białka  
   - organizm  
   - długość sekwencji  
   - funkcję (jeśli dostępna)  

4. Znajdź:
   - powiązane publikacje  
   - odnośniki do innych baz danych  

5. Przepisz dane:
   - do tabeli (np. CSV lub Excel)

---

### Wyniki  
- opis rekordu (minimum 10–15 zdań)  
- tabela z danymi  

---

### Wnioski  
- czym różni się rekord od samej sekwencji?  
- które informacje są kluczowe dla analizy bioinformatycznej?  
- które dane powtarzają się między rekordami?  

---

## Zadanie 1.5 – Operatory logiczne i strategia wyszukiwania

### Cel  
Nauczenie świadomego formułowania zapytań w bazach danych.

---

### Wykonaj  

1. W bazie NCBI Protein wyszukaj rekordy zawierające:
   - `cytochrome`

2. Wykonaj wyszukiwania z użyciem operatorów:
   - `cytochrome AND human`  
   - `cytochrome OR hemoglobin`  
   - `cytochrome NOT bacteria`

3. Porównaj:
   - liczbę rekordów  
   - charakter wyników  

4. Stwórz własne zapytanie:
   - zawierające minimum 3 warunki  
   - ograniczające wyniki do maksymalnie 20 rekordów  

---

### Wyniki  
- wszystkie użyte zapytania  
- liczba rekordów dla każdego przypadku  

---

### Wnioski  
- który operator najbardziej zawęża wyniki?  
- dlaczego konstrukcja zapytania ma znaczenie?  
- jakie błędy można popełnić przy wyszukiwaniu danych biologicznych?  

---
