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


[![Watch the video](https://img.youtube.com/vi/_UOx5x9eL/0.jpg)](https://youtu.be/QIZ8QH6JcC8?si=DPYXMYf_UOx5x9eL)



---

## Zadanie 1.1 – Wyszukiwanie publikacji i interpretacja danych (PubMed)

### Cel  
Zapoznanie się z mechanizmem wyszukiwania literatury naukowej oraz interpretacją liczby publikacji.

---

### Wykonaj  

1. Wejdź do bazy PubMed.  

2. Wyszukaj publikacje zawierające słowo kluczowe związane z Twoim kierunkiem studiów  
   (np. „gene expression”, „microbiome”, „enzyme”, „cancer”).

3. Zanotuj:
   - liczbę wszystkich rekordów (bez filtrów)

4. Zastosuj filtry:
   - zakres dat: od **dokładnej daty Twojego urodzenia** do dnia dzisiejszego  
   - język: angielski  

5. Dodaj kolejny filtr:
   - afiliacja: „Poland”

6. Zmodyfikuj zapytanie:
   - dodaj drugi termin biologiczny (np. `cancer AND microbiome`)

---

### Wyniki  
- wszystkie użyte zapytania (kwerendy)  
- liczba rekordów dla każdego wariantu  
- tabela porównawcza wyników  

---

### Wnioski  
- dlaczego liczba rekordów zmienia się po zastosowaniu filtrów?  
- które filtry mają największy wpływ?  
- czy liczba publikacji odzwierciedla popularność tematu badawczego?  

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
