# Ćwiczenie 3 – BLAST: wyszukiwanie homologii i identyfikacja sekwencji

## Wprowadzenie

Jednym z najważniejszych zadań bioinformatyki jest porównywanie sekwencji biologicznych.  
Jeżeli poznano nową sekwencję DNA lub białka, bardzo często pierwszym pytaniem jest:

- Czy podobna sekwencja została już wcześniej opisana?
- Jaką funkcję może pełnić?
- Z jakiego organizmu pochodzi?
- Czy posiada znane domeny lub regiony konserwatywne?
- Czy istnieje poznana struktura przestrzenna podobnego białka?

Do tego celu wykorzystuje się rodzinę narzędzi BLAST (Basic Local Alignment Search Tool).

BLAST umożliwia:
- wyszukiwanie sekwencji homologicznych,
- identyfikację potencjalnej funkcji biologicznej,
- analizę podobieństwa sekwencji,
- wykrywanie konserwatywnych regionów,
- odnajdywanie podobnych sekwencji w różnych organizmach.

W trakcie ćwiczenia nauczysz się:
- dobierać odpowiedni wariant BLAST,
- interpretować wyniki wyszukiwania,
- analizować alignmenty,
- rozumieć znaczenie parametrów wyszukiwania.

## Wybrane tutoriale
Quick start : https://blast.ncbi.nlm.nih.gov/doc/blast-quick-start-guide/

[![Playlista BLAST tutorials](https://img.youtube.com/vi/topBozEJGIk/0.jpg)](https://www.youtube.com/watch?v=topBozEJGIk&list=PL7dF9e2qSW0azL2xOKAtxDW7QI8UU4XZ6&index=2)

---

## Zadanie 3.1 – Identyfikacja homologicznych sekwencji białkowych (BLASTp)

### Cel  
Nauczenie się wyszukiwania sekwencji homologicznych dla białka.

---

### Wprowadzenie  

Sekwencje homologiczne to sekwencje posiadające wspólne pochodzenie ewolucyjne.  
Podobieństwo sekwencji bardzo często sugeruje podobieństwo funkcji biologicznej.

W tym zadaniu wykorzystasz sekwencję białkową jako kwerendę do wyszukania podobnych białek.

---

### Wykonaj  

1. Wybierz jedną sekwencję białkową:
   - z poprzednich ćwiczeń
   - lub pobierz nową sekwencję z NCBI Protein

2. Zapisz sekwencję w formacie FASTA.

3. Uruchom:
   - BLASTp

4. Wyszukaj sekwencje homologiczne:
   - w bazie proteinowej NCBI

5. Ogranicz wyszukiwanie:
   - do wybranego organizmu lub grupy organizmów
   - lub do wybranej bazy danych

6. Zanotuj:
   - liczbę odnalezionych sekwencji
   - najlepszy wynik
   - E-value
   - procent identyczności
   - Query Cover

7. Zapisz:
   - 1 najlepszą sekwencję
   - około 10 wybranych sekwencji
   - pełny zestaw wyników (maksymalnie 100)

---

### Wyniki  

- użyta sekwencja FASTA  
- parametry wyszukiwania  
- liczba homologów  
- zapisane pliki FASTA  
- screenshot lub fragment wyników BLAST  

---

### Wnioski  

- czym jest homologia sekwencji?  
- czy najwyższe podobieństwo zawsze oznacza identyczną funkcję?  
- co oznacza niski E-value?  
- dlaczego ograniczenie organizmów wpływa na wyniki?  

---

## Zadanie 3.2 – Wpływ parametrów BLAST na wyniki wyszukiwania

### Cel  
Zrozumienie wpływu parametrów wyszukiwania na czułość i specyficzność BLAST.

---

### Wprowadzenie  

BLAST wykorzystuje wiele parametrów wpływających na sposób dopasowania sekwencji.  
Zmiana parametrów może znacząco zmienić:
- liczbę wyników,
- jakość alignmentów,
- szybkość wyszukiwania.

---

### Wykonaj  

1. Użyj tej samej sekwencji co w zadaniu 3.1.

2. Wykonaj kilka wyszukiwań zmieniając:
   - wielkość słowa (Word size)
   - macierz substytucji (np. BLOSUM62, PAM30)
   - kary za przerwy (gap penalties)

3. Spróbuj:
   - promować krótkie alignmenty
   - promować długie alignmenty z małą liczbą przerw

4. Porównaj:
   - liczbę wyników
   - E-value
   - długości alignmentów
   - ranking trafień

---

### Wyniki  

- tabela parametrów i rezultatów  
- porównanie wyników wyszukiwania  

---

### Wnioski  

- które parametry najbardziej wpływają na wyniki?  
- czym różnią się macierze BLOSUM i PAM?  
- dlaczego zmiana parametrów może zmienić biologiczną interpretację wyników?  

---

## Zadanie 3.3 – Analiza alignmentu BLAST

### Cel  
Nauczenie się interpretacji alignmentów sekwencji.

---

### Wprowadzenie  

Wynik BLAST nie jest tylko listą rekordów.  
Najważniejszym elementem jest alignment, czyli przyrównanie sekwencji.

Alignment pozwala określić:
- regiony konserwatywne,
- mutacje,
- insercje i delecje,
- potencjalne regiony funkcjonalne.

---

### Wykonaj  

1. Wybierz:
   - najlepszy alignment z zadania 3.1
   - oraz jeden alignment o wyraźnie mniejszym podobieństwie

2. Porównaj:
   - procent identyczności
   - długość alignmentu
   - liczbę przerw
   - regiony konserwatywne

3. Sprawdź:
   - czy sekwencje pochodzą od tego samego organizmu
   - czy opis funkcji jest podobny

4. Zinterpretuj biologicznie:
   - czy są to prawdopodobnie ortologi?
   - czy mogą mieć podobną funkcję?

---

### Wyniki  

- fragmenty alignmentów  
- opis porównywanych sekwencji  
- tabela parametrów alignmentu  

---

### Wnioski  

- co oznacza wysoki procent identyczności?  
- czy krótki alignment może być biologicznie istotny?  
- jak interpretować przerwy (gaps)?  

---

## Zadanie 3.4 – Wyszukiwanie homologii w bazie struktur przestrzennych (PDB)

### Cel  
Powiązanie sekwencji aminokwasowej ze strukturą przestrzenną białka.

---

### Wprowadzenie  

Białka o podobnej sekwencji bardzo często posiadają podobną strukturę przestrzenną.  
BLAST może być używany również do przeszukiwania bazy struktur białkowych PDB.

---

### Wykonaj  

1. Wybierz sekwencję białkową.

2. Uruchom BLASTp przeciwko:
   - bazie PDB

3. Ogranicz analizę:
   - do fragmentu sekwencji (np. wybranego regionu)

4. Spróbuj zmieniać:
   - macierz substytucji
   - gap penalties

5. Znajdź:
   - najlepsze dopasowanie strukturalne

6. Sprawdź:
   - nazwę białka
   - organizm
   - datę zdeponowania struktury
   - rozdzielczość struktury (jeśli podana)

---

### Wyniki  

- identyfikator struktury PDB  
- parametry wyszukiwania  
- alignment  
- informacje o strukturze  

---

### Wnioski  

- czy podobieństwo sekwencji sugeruje podobieństwo struktury?  
- dlaczego struktury białkowe są ważne biologicznie?  
- czy wszystkie białka posiadają znane struktury przestrzenne?  

---

## Zadanie 3.5 – Dobór odpowiedniego wariantu BLAST

### Cel  
Nauczenie się wyboru odpowiedniego rodzaju BLAST dla różnych typów danych biologicznych.

---

### Wprowadzenie  

Rodzina BLAST zawiera wiele wariantów przeznaczonych do różnych analiz:

- BLASTn
- BLASTp
- BLASTx
- tBLASTn
- tBLASTx

Dobór niewłaściwego narzędzia może prowadzić do błędnej interpretacji wyników.

---

### Wykonaj  

1. Zapoznaj się z różnymi wariantami BLAST.

2. Dla każdego wariantu:
   - opisz typ danych wejściowych
   - opisz typ przeszukiwanej bazy

3. Podaj przykładowe zastosowanie biologiczne.

4. Spróbuj odpowiedzieć:
   - kiedy lepiej użyć porównania białek niż DNA?
   - dlaczego sekwencje białkowe są bardziej konserwatywne?

5. (Opcjonalnie) wykonaj krótkie wyszukiwanie:
   - co najmniej dwoma różnymi wariantami BLAST

---

### Wyniki  

- tabela wariantów BLAST  
- przykłady zastosowań  
- porównanie rezultatów  

---

### Wnioski  

- który wariant BLAST jest najbardziej uniwersalny?  
- dlaczego porównywanie białek często daje lepsze wyniki ewolucyjne niż DNA?  
- jakie błędy można popełnić przy wyborze niewłaściwego wariantu BLAST?  

---

## Zadanie dodatkowe 1 – Dynamika homologii

Spróbuj sprawdzić:
- czy ta sama sekwencja daje różne wyniki BLAST przy użyciu różnych baz danych,
- jak zmienia się liczba homologów po ograniczeniu organizmów,
- czy organizmy blisko spokrewnione mają bardziej podobne sekwencje.

---

## Zadanie dodatkowe 2 – Czy BLAST zawsze mówi prawdę?

Znajdź przykład:
- wysokiego podobieństwa bez identycznej funkcji
lub
- podobnej funkcji przy niskim podobieństwie.

Spróbuj biologicznie wyjaśnić taki przypadek.

---

## Pytanie otwarte (do dyskusji)

Czy wysokie podobieństwo sekwencji jest wystarczającym dowodem na identyczną funkcję biologiczną białka? Uzasadnij odpowiedź.
