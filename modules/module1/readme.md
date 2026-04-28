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
   Najlepiej wybierz coś, co rzeczywiście Cię ciekawi, będzie to dla Ciebie ciekawe oraz łatwiejsze w doborze filtrów.

---

2. Analiza globalna (świat)  

   Wyszukaj publikacje dla wybranego tematu.

   Zanotuj:
   - liczbę wszystkich rekordów (bez filtrów)

---

3. Analiza dla Polski  

   Zmodyfikuj zapytanie, dodając filtr:
   - afiliacja: Poland lub Polska (najlepiej użyj odpowiedniego operatora logicznego)

   Zanotuj:
   - liczbę rekordów  

---

4. Analiza dla UWM w Olsztynie  

   Spróbuj zawęzić wyniki do afiliacji związanych z Uniwersytetem Warmińsko-Mazurskim w Olsztynie.

   W tym celu przetestuj różne warianty zapytań (np. nazwa uczelni, miasto, skróty, różne wersje językowe).

   Zanotuj:
   - wszystkie użyte warianty zapytań  
   - liczbę rekordów dla każdego wariantu  

---

5. Analiza krytyczna afiliacji  

   Odpowiedz na pytania:

   - Czy zapis afiliacji w bazie danych jest jednoznaczny i czy zapis „UWM in Olsztyn” jest wystarczający? 
   - Czy wszyscy naukowcy/autorzy używają tej samej nazwy instytucji?  
   - Jakie problemy pojawiają się przy wyszukiwaniu po afiliacji?  
   - Jak wpływa to na wiarygodność wyników i jak można to zoptymalizować?  

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

- Jak wygląda udział Polski w globalnej efektywności publikowania w wybranej dziedzinie?  
- Jak wygląda aktywność publikacyjna UWM na tle Polski?  
- Czy można łatwo zidentyfikować badaczy z konkretnej uczelni?  
- Jakie są ograniczenia wyszukiwania po afiliacji?  
- Czy liczba publikacji odzwierciedla realną aktywność badawczą?  

---

### Zadanie dodatkowe 1 – dynamika publikacji w czasie  

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

#### Wnioski:

- Czy liczba publikacji rośnie, maleje czy jest stabilna?  
- Czy można wskazać momenty gwałtownego wzrostu?  
- Jak można interpretować te zmiany w kontekście rozwoju nauki?  

### Zadanie dodatkowe 2 – znajdż swojego promotora

Spróbuj znaleźć konkretnego naukowca z UWM pracującego w wybranej dziedzinie.  

- Jakie ma publikacje?  
- Czy jego afiliacja jest zapisana/zapisywana spójnie?



### Pytanie otwarte do dyskusji ( dodatkowe 3 ) 

Czy uważasz, że liczba publikacji jest dobrym wskaźnikiem rozwoju danej dziedziny? Uzasadnij swoją odpowiedź.


================================================================================
## Zadanie 1.2 – Analiza sekwencji nukleotydowych: struktura danych i ograniczenia wyszukiwania

### Cel  
Poznanie struktury bazy sekwencji nukleotydowych oraz rozwinięcie umiejętności krytycznej analizy danych biologicznych w zależności od zastosowanych filtrów.

---

### Wprowadzenie  

Bazy danych sekwencji nukleotydowych zawierają ogromne ilości informacji o DNA i RNA organizmów żywych. Dane te są podstawą analiz bioinformatycznych – od identyfikacji genów po badania ewolucyjne.

Jednak liczba rekordów w bazie nie jest prostą miarą „ilości biologii”. Wyniki zależą od:
- sposobu zdefiniowania zapytania  
- zastosowanych filtrów  
- definicji rekordu (gen, fragment, genom, transkrypt)  

W tym zadaniu spróbujesz zrozumieć, co tak naprawdę oznaczają liczby, które widzisz w wynikach wyszukiwania.

---

### Wykonaj  

1. Wybór organizmu  

   Wybierz jeden organizm do analizy:
   - człowiek (human lub *Homo sapiens*)
   - mysz (mouse lub *Mus musculus*)
   - świnia (pig lub *Sus scrofa*)
   lub  
   - inny organizm najlepiej związany z Twoimi zainteresowaniami (np. bakteria, roślina, pasożyt)

Upewnij się, że wyszukiwanie dotyczy rzeczywiscie nazwy organizmu, czy prawidłowo zastosowałeś ograniczenie do tego pola rekordu?

Sprawdż:
 - czy użycie nazwy organizmu po łacinie i po angielsku daje te same wyniki? Jak to uzasadnisz?

---

2. Analiza podstawowa  

   W bazie NCBI Nucleotide wyszukaj wszystkie rekordy dla wybranego organizmu.

   Zanotuj:
   - liczbę wszystkich rekordów  

---

3. Ograniczenie długości sekwencji  

   Zawęź wyniki do sekwencji krótszych niż:  

   **XXXX nukleotydów**  
   (XXXX = cztery ostatnie cyfry Twojego numeru indeksu)

   Zanotuj:
   - nową liczbę rekordów  

---

4. Sekwencje kodujące vs niekodujące  

   Spróbuj rozdzielić wyniki na:
   - sekwencje kodujące białka  
   - sekwencje niekodujące  

   (wykorzystaj dostępne filtry, słowa kluczowe lub pola wyszukiwania - bardzo ważny jest sposób zastosowania tego kryterium!)

   Zanotuj:
   - liczbę rekordów w każdej kategorii
   - kompletne kwerendy obrazujące jednoznacznie sposób wyszukiwania

---

5. Ograniczenie czasowe  

   Dodaj filtr:
   - rekordy opublikowane dokładnie od dnia Twojego urodzenia  

   Powtórz analizę dla:
   - wszystkich sekwencji  
   - sekwencji kodujących  
   - sekwencji niekodujących  

---

6. Analiza typu rekordu  

   Spróbuj sprawdzić, jakie typy danych dominują w wynikach, np.:
   - pełne genomy  
   - fragmenty genów  
   - mRNA  
   - regiony regulatorowe  

   (na podstawie opisów rekordów)

---

7. Zestawienie danych  

   Utwórz tabelę zawierającą:

   - wariant zapytania  
   - liczba rekordów  

   Przykładowe wiersze:
   - wszystkie rekordy  
   - długość < XXXX  
   - kodujące  
   - niekodujące  
   - z filtrem daty  

---

8. Wizualizacja danych  

   Wykonaj wykres przedstawiający:

   - wpływ filtrów na liczbę rekordów  
   (np. wykres słupkowy)

---

### Wyniki  

- wszystkie użyte zapytania (Search details / Advanced)  
- liczby rekordów  
- tabela porównawcza  
- wykres  

---

### Wnioski  

- Co oznacza „rekord” w bazie nukleotydowej?  
- Dlaczego liczba rekordów zmienia się tak znacząco po zastosowaniu filtrów?  
- Czy krótkie sekwencje dominują w bazie? Dlaczego?  
- Jakie są różnice między sekwencjami kodującymi i niekodującymi?  
- Czy dane w bazie są jednorodne (czy wszystkie rekordy są porównywalne)?  

---

### Zadanie dodatkowe 1 – dynamika przyrostu danych  

Spróbuj przeanalizować, jak zmieniała się liczba rekordów w czasie.

#### Wykonaj:

1. Podziel zakres czasu:
   - od roku Twojego urodzenia do dziś  
   - na kilka okresów (np. 5–10 przedziałów)

2. Dla każdego okresu:
   - wyszukaj liczbę rekordów spełniających Twoje kryteria  

3. Utwórz tabelę:
   - okres czasu  
   - liczba rekordów  

4. Wykonaj wykres:
   - liczba rekordów w funkcji czasu  

---

#### Wnioski:

- Czy baza danych rośnie liniowo, wykładniczo czy nieregularnie?  
- Jakie czynniki mogą wpływać na tempo przyrostu danych?  
- Czy rozwój technologii (np. sekwencjonowania) może mieć tu znaczenie?  

---

### Pytanie otwarte (do dyskusji)

- Czy liczba rekordów w bazie nukleotydowej jest dobrą miarą naszej wiedzy o genomach organizmów? Uzasadnij odpowiedź. 

============================================================================

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
