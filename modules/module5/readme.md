# Ćwiczenie 5 – Multiple Sequence Alignment (MSA) i analiza regionów konserwatywnych

## Wprowadzenie

W poprzednim ćwiczeniu analizowano podobieństwo dwóch sekwencji biologicznych za pomocą pairwise alignment. W praktyce bioinformatycznej bardzo często konieczne jest jednak jednoczesne porównanie większej liczby sekwencji.

Do tego celu wykorzystuje się:
- Multiple Sequence Alignment (MSA),
czyli wielokrotne dopasowanie sekwencji.

MSA umożliwia:
- identyfikację regionów konserwatywnych,
- analizę mutacji,
- wykrywanie domen funkcjonalnych,
- analizę ewolucji molekularnej,
- przygotowanie danych do budowy drzew filogenetycznych,
- analizę rodzin białek i genów.

W czasie ćwiczenia wykorzystasz narzędzia:
- Clustal Omega,
- COBALT,
- Jalview,
- serwisy NCBI i EMBL-EBI.

---

## Materiały i tutoriale

### Narzędzia MSA w EMBL-EBI
https://www.ebi.ac.uk/jdispatcher/msa

### Clustal Omega (EMBL-EBI)
https://www.ebi.ac.uk/jdispatcher/msa/clustalo

### COBALT (NCBI)
https://www.ncbi.nlm.nih.gov/tools/cobalt/

### Jalview
https://www.jalview.org/

### EMBL-EBI – Multiple sequence alignment
https://www.ebi.ac.uk/training/online/courses/guide-to-sequence-analysis-tools/multiple-sequence-alignment/

### Guide to sequence analysis tools
https://www.ebi.ac.uk/training/online/courses/guide-to-sequence-analysis-tools/

---

# Zadanie 5.1 – Tworzenie Multiple Sequence Alignment

## Cel

Poznanie zasad tworzenia MSA oraz interpretacji podstawowych parametrów alignmentu.

---

## Wprowadzenie

MSA umożliwia jednoczesne porównanie wielu sekwencji i znalezienie:
- wspólnych regionów,
- mutacji,
- konserwatywnych aminokwasów,
- różnic ewolucyjnych.

W przeciwieństwie do pairwise alignment:
- wynik zależy od wszystkich sekwencji jednocześnie,
- kolejność i dobór sekwencji mają bardzo duże znaczenie.

---

## Wykonaj

1. Wybierz rodzinę białek:
   - cytochromy,
   - heksokinazy,
   - hemoglobiny,
   - kinazy,
   - białka błonowe,
   - lub inną rodzinę biologicznie uzasadnioną.

2. Pobierz:
   - minimum 5,
   - maksimum 15 sekwencji białkowych w formacie FASTA.

3. Upewnij się, że:
   - sekwencje są homologiczne,
   - pochodzą z różnych organizmów,
   - nie są fragmentami („partial”).

4. Wykonaj alignment:
   - w Clustal Omega,
   lub
   - w COBALT.

5. Zapisz wynik:
   - w formacie Clustal (.aln),
   - oraz FASTA alignment.

---

## Wyniki

- lista użytych rekordów,
- numery akcesyjne,
- plik alignmentu,
- screenshot alignmentu.

---

## Wnioski

- czy wszystkie sekwencje udało się dobrze dopasować?
- które fragmenty alignmentu są najbardziej podobne?
- czy długości sekwencji mają wpływ na jakość alignmentu?

---

# Zadanie 5.2 – Wpływ doboru sekwencji na alignment

## Cel

Zrozumienie wpływu podobieństwa sekwencji na jakość MSA.

---

## Wprowadzenie

Alignment wielu sekwencji staje się trudniejszy, gdy:
- sekwencje są bardzo odległe ewolucyjnie,
- różnią się długością,
- zawierają liczne insercje i delecje.

Dobór nieodpowiednich sekwencji może:
- pogorszyć alignment,
- zaburzyć regiony konserwatywne,
- prowadzić do błędnych interpretacji biologicznych.

---

## Wykonaj

1. Wykorzystaj alignment z Zadania 5.1.

2. Dodaj:
   - jedną bardzo odległą ewolucyjnie sekwencję,
   lub
   - jedną bardzo krótką sekwencję fragmentaryczną.

3. Ponownie wykonaj alignment.

4. Porównaj:
   - liczbę gaps,
   - długość alignmentu,
   - regiony konserwatywne,
   - ogólną czytelność alignmentu.

---

## Wyniki

- oba alignmenty,
- tabela porównawcza,
- opis zmian.

---

## Wnioski

- jak pojedyncza sekwencja może wpłynąć na cały alignment?
- dlaczego dobór danych wejściowych jest kluczowy?
- czy „więcej danych” zawsze oznacza „lepszy wynik”?

---

# Zadanie 5.3 – Regiony konserwatywne i motywy funkcjonalne

## Cel

Identyfikacja regionów konserwatywnych i ich interpretacja biologiczna.

---

## Wprowadzenie

Regiony konserwatywne:
- ewoluują bardzo wolno,
- są często związane z funkcją biologiczną,
- mogą odpowiadać za:
  - centrum aktywne enzymu,
  - wiązanie substratu,
  - stabilizację struktury,
  - wiązanie kofaktorów.

MSA pozwala wykrywać takie regiony.

---

## Wykonaj

1. Otwórz alignment:
   - w Jalview,
   lub
   - w viewerze Clustal/COBALT.

2. Włącz:
   - kolorowanie według konserwacji,
   - conservation score.

3. Zidentyfikuj:
   - regiony identyczne,
   - regiony silnie konserwatywne,
   - regiony zmienne.

4. Spróbuj określić:
   - które fragmenty mogą odpowiadać za funkcję białka.

5. Sprawdź jedną z sekwencji:
   - w UniProt,
   - lub Conserved Domains Database (CDD).

6. Porównaj:
   - regiony konserwatywne alignmentu,
   - opisane domeny funkcjonalne.

---

## Wyniki

- alignment z zaznaczonymi regionami,
- opis regionów konserwatywnych,
- odniesienie do domen funkcjonalnych.

---

## Wnioski

- dlaczego niektóre regiony są bardziej konserwatywne?
- czy wszystkie mutacje są równie ważne?
- czy region konserwatywny zawsze oznacza region funkcjonalny?

---

# Zadanie 5.4 – Alignment sekwencji DNA i białek

## Cel

Porównanie MSA dla sekwencji nukleotydowych i aminokwasowych.

---

## Wprowadzenie

Sekwencje DNA:
- zawierają tylko 4 typy nukleotydów,
- szybciej akumulują mutacje,
- zawierają mutacje synonimiczne.

Sekwencje białkowe:
- lepiej odzwierciedlają funkcję biologiczną,
- są bardziej konserwatywne ewolucyjnie.

Dlatego alignment DNA i alignment białek mogą wyglądać bardzo różnie.

---

## Wykonaj

1. Wybierz:
   - kilka homologicznych genów,
   - oraz odpowiadające im białka.

2. Wykonaj:
   - MSA dla DNA,
   - MSA dla białek.

3. Porównaj:
   - długość alignmentów,
   - liczbę gaps,
   - stopień konserwacji,
   - czytelność alignmentu.

4. Spróbuj wyjaśnić:
   - dlaczego alignmenty różnią się między sobą.

---

## Wyniki

- oba alignmenty,
- tabela porównawcza,
- opis różnic.

---

## Wnioski

- dlaczego alignment białek często jest bardziej użyteczny?
- czym są mutacje synonimiczne?
- które dane lepiej nadają się do analizy ewolucyjnej?

---

# Zadanie 5.5 – Drzewo filogenetyczne na podstawie alignmentu

## Cel

Wprowadzenie do analizy pokrewieństwa ewolucyjnego.

---

## Wprowadzenie

MSA jest podstawą:
- budowy drzew filogenetycznych,
- analizy ewolucji molekularnej,
- badania pokrewieństwa organizmów.

Drzewo filogenetyczne:
- przedstawia podobieństwo sekwencji,
- nie zawsze odpowiada dokładnie klasyfikacji biologicznej,
- zależy od jakości alignmentu.

---

## Wykonaj

1. Wykorzystaj alignment z Zadania 5.1.

2. Wygeneruj:
   - drzewo filogenetyczne,
   - za pomocą Clustal Omega lub COBALT.

3. Sprawdź:
   - które sekwencje grupują się razem,
   - które organizmy są najbardziej podobne.

4. Porównaj:
   - wynik drzewa,
   - znane pokrewieństwo biologiczne organizmów.

---

## Wyniki

- drzewo filogenetyczne,
- opis grupowania sekwencji.

---

## Wnioski

- czy podobieństwo sekwencji odpowiada pokrewieństwu organizmów?
- jakie błędy mogą pojawić się w analizie filogenetycznej?
- jak jakość alignmentu wpływa na drzewo?

---

# Zadanie dodatkowe 1 – Analiza cytochromu B

## Wykonaj

1. Pobierz:
   - sekwencje białkowe cytochromu B,
   - od minimum 10 organizmów.

2. Wykonaj:
   - MSA,
   - analizę regionów konserwatywnych,
   - drzewo filogenetyczne.

3. Spróbuj odpowiedzieć:
   - czy cytochrom B jest silnie konserwatywny?
   - które organizmy są najbardziej podobne?

---

## Wnioski

- dlaczego cytochrom B jest często używany w analizach filogenetycznych?

---

# Zadanie dodatkowe 2 – Consensus sequence

## Wykonaj

1. Na podstawie alignmentu:
   - wyznacz consensus sequence.

2. Spróbuj określić:
   - które pozycje są najbardziej stabilne ewolucyjnie.

---

## Wnioski

- czy consensus sequence może reprezentować „idealne” białko rodziny?
- jakie są ograniczenia takiego podejścia?

---

# Pytanie otwarte (do dyskusji)

Czy bardzo podobne sekwencje zawsze oznaczają:
- identyczną funkcję,
- wspólne pochodzenie,
- podobną strukturę przestrzenną?

Uzasadnij odpowiedź przykładami biologicznymi.
