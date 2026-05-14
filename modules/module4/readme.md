# Ćwiczenie 4 – Pairwise alignment i analiza podobieństwa sekwencji

## Wprowadzenie

Jednym z najważniejszych zadań bioinformatyki jest porównywanie sekwencji biologicznych.  
Porównując sekwencje DNA lub białek można:

- identyfikować geny i białka homologiczne,
- przewidywać funkcję nieznanych sekwencji,
- analizować ewolucję organizmów,
- wykrywać mutacje,
- identyfikować regiony konserwatywne,
- badać zależności między strukturą i funkcją białek.

Najprostszą formą takiej analizy jest **pairwise sequence alignment** — dopasowanie dwóch sekwencji do siebie.

Wyróżniamy dwa podstawowe typy alignmentów:

- **global alignment** – porównanie całych sekwencji,
- **local alignment** – wyszukiwanie najlepiej dopasowanych fragmentów.

Alignmenty wykorzystują:
- macierze substytucji (np. PAM, BLOSUM),
- system punktacji (score),
- kary za przerwy (gap penalties).

W praktyce bioinformatycznej pairwise alignment stanowi podstawę działania takich narzędzi jak:
- BLAST,
- FASTA,
- Clustal,
- COBALT,
- MUSCLE,
- HMMER.

W ćwiczeniu wykorzystasz internetowe narzędzia Europejskiego Instytutu Bioinformatycznego (EMBL-EBI) oraz serwisy NCBI.

---

## Materiały i tutoriale

### EMBL-EBI Pairwise Sequence Alignment
https://www.ebi.ac.uk/jdispatcher/psa

### Tutorial EMBL-EBI – Pairwise sequence alignment
https://www.ebi.ac.uk/training/online/courses/guide-to-sequence-analysis-tools/sequence-alignment/pairwise-sequence-alignment/

### Guide to sequence analysis tools
https://www.ebi.ac.uk/training/online/courses/guide-to-sequence-analysis-tools/

### NCBI BLAST
https://blast.ncbi.nlm.nih.gov/

---

# Zadanie 4.1 – Global alignment vs local alignment

## Cel

Poznanie różnic między globalnym i lokalnym dopasowaniem sekwencji.

---

## Wprowadzenie

Dwie sekwencje biologiczne mogą być podobne:
- na całej długości,
- tylko w wybranych fragmentach,
- lub zawierać jedynie krótkie regiony homologiczne.

Dlatego stosuje się różne strategie alignmentu.

### Global alignment
Próbuje dopasować:
- całą długość obu sekwencji.

Najlepiej sprawdza się dla:
- bardzo podobnych białek,
- ortologów,
- sekwencji o podobnej długości.

Najczęściej wykorzystuje algorytm:
- Needleman-Wunsch.

---

### Local alignment
Wyszukuje:
- najlepiej dopasowane regiony.

Najlepiej sprawdza się dla:
- odległych homologów,
- wspólnych domen,
- krótkich motywów funkcjonalnych.

Najczęściej wykorzystuje algorytm:
- Smith-Waterman.

---

## Wykonaj

1. Wybierz dwa białka:
   - najlepiej homologiczne,
   - pochodzące z różnych organizmów.

2. Pobierz ich sekwencje FASTA z NCBI Protein.

3. Wykonaj:
   - global alignment,
   - local alignment.

4. Wykorzystaj:
   - EMBOSS Needle (global),
   - EMBOSS Water (local),
   dostępne na:
   https://www.ebi.ac.uk/jdispatcher/psa

5. Porównaj:
   - długość alignmentów,
   - liczbę identycznych aminokwasów,
   - liczbę przerw,
   - score,
   - procent identyczności.

6. Spróbuj odpowiedzieć:
   - który alignment lepiej opisuje biologiczne podobieństwo badanych białek?

---

## Wyniki

- użyte sekwencje FASTA,
- parametry alignmentu,
- oba alignmenty,
- tabela porównawcza wyników.

---

## Wnioski

- czym różni się alignment globalny od lokalnego?
- kiedy lepiej stosować każdy z nich?
- dlaczego dwa alignmenty dla tych samych sekwencji mogą wyglądać zupełnie inaczej?

---

# Zadanie 4.2 – Wpływ kar za przerwy (gap penalties)

## Cel

Zrozumienie wpływu insercji i delecji na wynik alignmentu.

---

## Wprowadzenie

W czasie ewolucji sekwencje ulegają:
- mutacjom punktowym,
- insercjom,
- delecjom.

Aby poprawnie dopasować sekwencje, programy alignmentowe wprowadzają:
- przerwy (gaps).

Jednak każda przerwa obniża score alignmentu.

Programy stosują dwa typy kar:
- gap opening penalty,
- gap extension penalty.

Zmiana tych parametrów może radykalnie zmienić alignment.

---

## Wykonaj

1. Wykorzystaj te same sekwencje co w Zadaniu 4.1.

2. Wykonaj kilka alignmentów:
   - z bardzo wysokimi karami za gaps,
   - z bardzo niskimi karami za gaps.

3. Porównaj:
   - liczbę przerw,
   - długość alignmentu,
   - score,
   - procent identyczności.

4. Spróbuj znaleźć:
   - alignment biologicznie najbardziej sensowny.

---

## Wyniki

- zestaw parametrów,
- alignmenty,
- tabela porównawcza.

---

## Wnioski

- jak kary za gaps wpływają na alignment?
- dlaczego zbyt duża liczba przerw może być biologicznie nienaturalna?
- dlaczego czasem wiele krótkich przerw jest mniej prawdopodobne niż jedna długa?

---

# Zadanie 4.3 – Wpływ macierzy substytucji

## Cel

Poznanie znaczenia macierzy substytucji w analizie sekwencji białkowych.

---

## Wprowadzenie

Nie wszystkie mutacje aminokwasowe są równie prawdopodobne.

Przykładowo:
- leucyna i izoleucyna często zastępują się wzajemnie,
- tryptofan zmienia się znacznie rzadziej.

Macierze substytucji opisują:
- biologiczne prawdopodobieństwo zmian aminokwasów.

Najczęściej używane:
- PAM,
- BLOSUM.

---

## Wykonaj

1. Wykonaj alignment tych samych sekwencji:
   - używając BLOSUM62,
   - używając PAM30,
   - używając PAM250.

2. Porównaj:
   - score,
   - długość alignmentu,
   - procent identyczności,
   - rozmieszczenie mutacji.

3. Spróbuj ustalić:
   - która macierz najlepiej nadaje się do:
     - bardzo podobnych sekwencji,
     - odległych homologów.

---

## Wyniki

- alignmenty,
- tabela porównawcza,
- opis różnic.

---

## Wnioski

- czym różnią się macierze PAM i BLOSUM?
- dlaczego wynik alignmentu zależy od użytej macierzy?
- która macierz była najbardziej restrykcyjna?

---

# Zadanie 4.4 – Pairwise alignment za pomocą BLAST

## Cel

Pokazanie, że narzędzie BLAST może być używane również do porównywania dwóch konkretnych sekwencji.

---

## Wprowadzenie

BLAST kojarzony jest głównie z:
- wyszukiwaniem homologów w ogromnych bazach danych.

Jednak można go również wykorzystać do:
- bezpośredniego porównania dwóch sekwencji.

NCBI umożliwia:
- wykonanie pairwise BLAST,
- analizę regionów homologicznych,
- ocenę podobieństwa biologicznego.

---

## Wykonaj

1. Wejdź na:
   https://blast.ncbi.nlm.nih.gov/

2. Wybierz:
   - Protein BLAST (blastp)
   lub
   - Nucleotide BLAST (blastn).

3. Wprowadź:
   - jedną sekwencję jako Query,
   - drugą sekwencję jako Subject.

4. W ustawieniach:
   - ogranicz wyszukiwanie do jednej sekwencji Subject,
   - wyłącz standardowe przeszukiwanie całej bazy danych.

5. Porównaj:
   - score,
   - E-value,
   - identities,
   - positives,
   - gaps.

6. Zinterpretuj:
   - które regiony są najbardziej konserwatywne.

---

## Wyniki

- parametry BLAST,
- alignment,
- screenshot lub eksport wyników.

---

## Wnioski

- czym różni się BLAST od klasycznego alignmentu globalnego?
- dlaczego BLAST zwykle znajduje alignment lokalny?
- jakie są zalety i ograniczenia BLAST?

---

# Zadanie 4.5 – Biologiczna interpretacja alignmentu

## Cel

Nauczenie biologicznej interpretacji podobieństwa sekwencji.

---

## Wprowadzenie

Alignment nie jest jedynie matematycznym dopasowaniem znaków.

Każda mutacja może:
- zmieniać funkcję białka,
- wpływać na strukturę,
- wpływać na aktywność enzymatyczną,
- powodować choroby.

Regiony silnie konserwatywne często odpowiadają za:
- centrum aktywne,
- miejsca wiązania ligandów,
- domeny funkcjonalne.

---

## Wykonaj

1. Wybierz alignment z poprzednich zadań.

2. Zidentyfikuj:
   - regiony identyczne,
   - regiony konserwatywne,
   - insercje/delecje,
   - najbardziej zmienne fragmenty.

3. Sprawdź rekordy białek w:
   - UniProt,
   - NCBI Protein.

4. Spróbuj ustalić:
   - czy regiony konserwatywne odpowiadają znanym domenom.

5. Jeśli to możliwe:
   - znajdź mutacje związane z chorobami.

---

## Wyniki

- opis alignmentu,
- wskazane regiony konserwatywne,
- interpretacja biologiczna.

---

## Wnioski

- dlaczego niektóre regiony ewoluują bardzo wolno?
- czy podobieństwo sekwencji zawsze oznacza podobną funkcję?
- jakie ograniczenia ma analiza pairwise alignment?

---

# Zadanie dodatkowe 1 – Alignment sekwencji DNA vs białka

## Wykonaj

1. Wybierz:
   - gen kodujący białko,
   - odpowiadającą mu sekwencję aminokwasową.

2. Wykonaj:
   - alignment DNA,
   - alignment białek.

3. Porównaj:
   - liczbę mutacji,
   - długość alignmentów,
   - obecność gaps.

---

## Wnioski

- dlaczego alignment białek często jest bardziej informacyjny niż alignment DNA?
- czym są mutacje synonimiczne?

---

# Zadanie dodatkowe 2 – Czy podobieństwo oznacza wspólne pochodzenie?

## Pytanie otwarte

Czy wysokie podobieństwo sekwencji zawsze oznacza:
- wspólne pochodzenie ewolucyjne,
- identyczną funkcję biologiczną?

Uzasadnij odpowiedź przykładami biologicznymi.
