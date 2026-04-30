# Ćwiczenie 2 – Format danych biologicznych i reprezentacja informacji

## Wprowadzenie

Dane biologiczne w bioinformatyce są przechowywane i analizowane w postaci plików tekstowych.  
Sekwencje DNA, RNA i białek nie są „obiektami biologicznymi” w komputerze — są zapisane jako ciągi znaków.

Sposób zapisu danych ma kluczowe znaczenie dla:
- możliwości ich analizy,
- kompatybilności między narzędziami,
- wielkości plików,
- szybkości przetwarzania.

W tym ćwiczeniu skupisz się na zrozumieniu:
- czym jest format danych,
- jak reprezentowane są sekwencje biologiczne,
- jakie są różnice między formatami tekstowymi i binarnymi,
- dlaczego ten sam zestaw danych może zajmować różną ilość miejsca.

---

## Zadanie 2.1 – Sekwencja biologiczna jako tekst

### Cel  
Zrozumienie, jak reprezentowana jest struktura biologiczna w najprostszym możliwym formacie.

---

### Wprowadzenie  

Białko to obiekt fizyczny o złożonej strukturze przestrzennej.  
W bioinformatyce jego najprostsza reprezentacja to **sekwencja aminokwasów**, czyli ciąg liter.

Twoim zadaniem jest zaprojektowanie możliwie najprostszego i najbardziej uniwersalnego sposobu zapisu takiej informacji.

---

### Wykonaj  

1. Wybierz dowolne białko:
   - z bazy NCBI Protein  
   - lub inne źródło  

2. Zapisz jego sekwencję:
   - w pliku tekstowym `.txt`  
   - w możliwie najprostszym formacie  

3. Zaprojektuj sposób zapisu tak, aby:
   - łatwo było określić długość sekwencji  
   - zapis był czytelny dla człowieka  
   - zapis był możliwy do przetworzenia przez program  

4. (Opcjonalnie) porównaj swój zapis z formatem FASTA

---

### Wyniki  
- treść pliku (wklejona w raporcie)  
- nazwa pliku  
- długość sekwencji  

---

### Wnioski  
- dlaczego wybrany sposób zapisu jest dobry?  
- jakie ma ograniczenia?  
- czym różni się od formatu FASTA?  

---

## Zadanie 2.2 – Format FASTA jako standard bioinformatyczny

### Cel  
Poznanie struktury formatu FASTA i jego znaczenia w analizie danych biologicznych.

---

### Wykonaj  

1. Pobierz kilka (3–5) sekwencji białkowych z bazy NCBI.

2. Zapisz je w formacie FASTA:
   - jako jeden plik  
   - jako osobne pliki  

3. Przeanalizuj strukturę FASTA:
   - linia nagłówkowa  
   - sekwencja  

4. Otwórz plik:
   - w edytorze tekstu  
   - w przeglądarce  
   - w innym programie (np. Excel)

---

### Wyniki  
- pliki FASTA  
- opis struktury pliku  

---

### Wnioski  
- dlaczego FASTA jest uniwersalnym formatem?  
- jakie informacje zawiera nagłówek?  
- jakie są ograniczenia tego formatu?  

---

## Zadanie 2.3 – Format pliku a jego interpretacja

### Cel  
Zrozumienie różnicy między zawartością pliku a jego rozszerzeniem.

---

### Wykonaj  

1. Utwórz 3 pliki:
   - plik tekstowy (.txt)  
   - plik dokumentu (.doc / .docx)  
   - plik graficzny (.bmp lub .png)  

2. Skopiuj każdy plik i zmień jego rozszerzenie tak, aby powstało 9 plików:
   - np. tekst.txt → tekst.doc → tekst.bmp  

3. Spróbuj otworzyć każdy plik.

---

### Wyniki  
- opis efektów otwierania każdego pliku  

---

### Wnioski  
- czy zmiana rozszerzenia zmienia format pliku?  
- dlaczego niektóre pliki są nieczytelne?  
- jak system operacyjny interpretuje pliki?  

---

## Zadanie 2.4 – Wielkość pliku a ilość informacji

### Cel  
Zrozumienie, od czego zależy rozmiar pliku.

---

### Wykonaj  

1. Utwórz pliki zawierające:
   - 0 znaków  
   - 10 znaków  
   - 100 znaków  
   - 1000 znaków  
   - 10000 znaków  

2. Zapisz je w różnych formatach:
   - .txt  
   - .doc/.docx  
   - (opcjonalnie) .rtf  

3. Sprawdź ich rozmiar (w bajtach).

---

### Wyniki  
- tabela: liczba znaków vs rozmiar pliku  

---

### Wnioski  
- dlaczego pliki mają różne rozmiary?  
- od czego zależy wielkość pliku tekstowego?  
- dlaczego plik .doc jest większy niż .txt?  

---

## Zadanie 2.5 – Tabela jako model bazy danych

### Cel  
Zrozumienie, jak dane biologiczne mogą być reprezentowane w formie tabelarycznej.

---

### Wykonaj  

1. Utwórz tabelę zawierającą minimum 5 rekordów (np. sekwencji).

2. Każdy rekord powinien zawierać:
   - identyfikator  
   - nazwę  
   - organizm  
   - typ cząsteczki  
   - sekwencję  

3. Zapisz tabelę:
   - w formacie .doc/.docx  
   - w formacie .csv lub .tsv  

4. Otwórz pliki w różnych programach.

---

### Wyniki  
- tabela  
- zapis w różnych formatach  

---

### Wnioski  
- czym różni się zapis tabeli w .doc i .csv?  
- który format jest bardziej „uniwersalny”?  
- dlaczego bazy danych używają struktur tabelarycznych?  

---

## Pytanie otwarte (do dyskusji)

Czy dane biologiczne są bardziej „danymi tekstowymi” czy „danymi liczbowymi”?  
Uzasadnij swoją odpowiedź, odnosząc się do przykładów z ćwiczenia.
