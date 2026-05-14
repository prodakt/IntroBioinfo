# Ćwiczenie 6 – Analiza funkcjonalna białek i adnotacja biologiczna

## Wprowadzenie

W poprzednich modułach kursu poznano:
- biologiczne bazy danych,
- sposoby wyszukiwania informacji,
- formaty zapisu sekwencji,
- narzędzia BLAST,
- pairwise alignment,
- multiple sequence alignment (MSA).

W praktyce bioinformatycznej samo znalezienie podobnej sekwencji jest jednak dopiero początkiem analizy biologicznej.

Najważniejsze pytania pojawiają się dopiero później:

- Jaką funkcję pełni dane białko?
- W jakich procesach biologicznych uczestniczy?
- Czy jest enzymem, receptorem, białkiem strukturalnym?
- Gdzie w komórce występuje?
- Czy posiada regiony konserwatywne lub domeny funkcjonalne?
- Czy istnieje jego struktura przestrzenna?
- Czy mutacje w tym białku mogą prowadzić do chorób?
- Czy można przewidzieć funkcję nieznanej sekwencji wyłącznie na podstawie podobieństwa do innych białek?

Współczesna bioinformatyka bardzo często polega właśnie na:
- integrowaniu informacji z wielu baz danych,
- analizie homologii,
- interpretacji biologicznej wyników komputerowych.

W tym module student przejdzie pełną drogę:
od „surowej sekwencji” do biologicznej interpretacji funkcji białka.

Będzie to pierwszy moduł, w którym analiza zaczyna przypominać rzeczywistą pracę badawczą:
- analizę nieznanego genu,
- interpretację wyników sekwencjonowania,
- przewidywanie funkcji nowego białka,
- analizę potencjalnych biomarkerów i mutacji chorobowych.

Umiejętności zdobywane w tym module są wykorzystywane m.in. w:
- biologii molekularnej,
- biotechnologii,
- diagnostyce molekularnej,
- medycynie personalizowanej,
- genomice,
- proteomice,
- biologii strukturalnej,
- projektowaniu leków,
- analizie danych NGS,
- bioinformatyce klinicznej.

---

# Wykorzystywane bazy danych i narzędzia

## UniProt
https://www.uniprot.org/

## NCBI Protein
https://www.ncbi.nlm.nih.gov/protein/

## Conserved Domains Database (CDD)
https://www.ncbi.nlm.nih.gov/Structure/cdd/cdd.shtml

## InterPro
https://www.ebi.ac.uk/interpro/

## Pfam
https://pfam.xfam.org/

## Protein Data Bank (PDB)
https://www.rcsb.org/

## AlphaFold Protein Structure Database
https://alphafold.ebi.ac.uk/

## ClinVar
https://www.ncbi.nlm.nih.gov/clinvar/

## OMIM
https://www.omim.org/

---

# Zadanie 6.1 – Analiza rekordu UniProt

## Cel

Poznanie struktury nowoczesnych rekordów białkowych oraz integracji informacji biologicznych z wielu źródeł.

---

## Wprowadzenie

UniProt jest jedną z najważniejszych baz danych białek na świecie.  
Łączy informacje:
- o sekwencji,
- funkcji,
- strukturze,
- lokalizacji komórkowej,
- mutacjach,
- chorobach,
- literaturze naukowej,
- domenach białkowych.

W praktyce bioinformatycznej rekord UniProt bardzo często stanowi „centrum wiedzy” o białku.

---

## Wykonaj

1. Wybierz jedno białko:
   - związane z Twoimi zainteresowaniami,
   - lub znalezione we wcześniejszych ćwiczeniach.

2. Znajdź odpowiadający rekord:
   - w UniProt.

3. Zidentyfikuj i opisz:
   - accession number,
   - nazwę białka,
   - organizm,
   - długość sekwencji,
   - funkcję biologiczną,
   - lokalizację komórkową,
   - domeny funkcjonalne,
   - informacje o strukturze,
   - odnośniki do innych baz danych.

4. Sprawdź:
   - czy rekord jest:
     - reviewed (Swiss-Prot),
     - czy unreviewed (TrEMBL).

5. Znajdź:
   - publikacje powiązane z rekordem.

---

## Wyniki

- opis rekordu,
- numer akcesyjny,
- tabela najważniejszych informacji,
- screenshot wybranych elementów rekordu.

---

## Wnioski

- dlaczego rekordy reviewed są bardziej wiarygodne?
- jakie informacje są najważniejsze dla biologa?
- dlaczego współczesne bazy danych są silnie połączone między sobą?

---

# Zadanie 6.2 – Analiza domen białkowych

## Cel

Identyfikacja regionów funkcjonalnych białka oraz interpretacja ich znaczenia biologicznego.

---

## Wprowadzenie

Większość białek składa się z:
- domen,
czyli fragmentów odpowiedzialnych za określone funkcje biologiczne.

Przykładowo:
- domena kinazowa odpowiada za fosforylację,
- domeny transbłonowe umożliwiają zakotwiczenie w błonie,
- domeny wiążące DNA uczestniczą w regulacji ekspresji genów.

Analiza domen jest jedną z podstaw:
- przewidywania funkcji białek.

---

## Wykonaj

1. Wybierz białko z Zadania 6.1.

2. Przeanalizuj jego sekwencję:
   - w CDD,
   - InterPro,
   - lub Pfam.

3. Zidentyfikuj:
   - domeny funkcjonalne,
   - ich pozycje,
   - ewentualne motywy konserwatywne.

4. Sprawdź:
   - czy regiony konserwatywne pokrywają się z domenami zidentyfikowanymi wcześniej w MSA.

5. Spróbuj odpowiedzieć:
   - które fragmenty białka są prawdopodobnie najważniejsze funkcjonalnie.

---

## Wyniki

- lista domen,
- pozycje domen,
- screenshot analizy domenowej,
- opis funkcjonalny.

---

## Wnioski

- czym różni się domena od całego białka?
- dlaczego domeny są często konserwatywne ewolucyjnie?
- czy jedno białko może mieć wiele funkcji?

---

# Zadanie 6.3 – Struktura przestrzenna białka

## Cel

Poznanie podstaw analizy struktury przestrzennej białek.

---

## Wprowadzenie

Funkcja białka zależy nie tylko od sekwencji aminokwasowej, ale również od:
- struktury przestrzennej.

Nawet pojedyncza mutacja może:
- zmienić strukturę,
- zaburzyć funkcję,
- prowadzić do choroby.

Współczesna bioinformatyka bardzo intensywnie wykorzystuje:
- modelowanie struktur,
- przewidywanie struktur,
- analizę centrów aktywnych,
- analizę oddziaływań białek.

---

## Wykonaj

1. Znajdź strukturę wybranego białka:
   - w PDB,
   lub
   - w bazie AlphaFold.

2. Otwórz model 3D.

3. Zidentyfikuj:
   - helisy alfa,
   - beta-kartki,
   - regiony nieuporządkowane,
   - ligand,
   - centrum aktywne (jeśli występuje).

4. Sprawdź:
   - czy regiony konserwatywne z alignmentu odpowiadają ważnym elementom struktury.

5. Spróbuj odpowiedzieć:
   - dlaczego niektóre regiony są bardziej konserwatywne.

---

## Wyniki

- numer rekordu PDB/AlphaFold,
- screenshot struktury,
- opis struktury.

---

## Wnioski

- dlaczego struktura białka jest ważniejsza niż sama sekwencja?
- czy bardzo podobne sekwencje zawsze mają identyczną strukturę?
- jakie ograniczenia mają modele przewidywane komputerowo?

---

# Zadanie 6.4 – Mutacje i choroby

## Cel

Poznanie związku między mutacjami a funkcją białek.

---

## Wprowadzenie

Wiele chorób genetycznych wynika z:
- mutacji zmieniających sekwencję białka.

Mutacje mogą:
- zmieniać strukturę,
- destabilizować białko,
- zaburzać wiązanie ligandów,
- prowadzić do utraty funkcji.

Bioinformatyka kliniczna wykorzystuje:
- analizę wariantów,
- przewidywanie skutków mutacji,
- analizę SNP,
- bazy mutacji chorobowych.

---

## Wykonaj

1. Dla wybranego białka sprawdź:
   - ClinVar,
   - OMIM,
   - UniProt.

2. Znajdź:
   - mutacje związane z chorobami.

3. Zanotuj:
   - typ mutacji,
   - pozycję aminokwasu,
   - chorobę,
   - wpływ biologiczny.

4. Spróbuj określić:
   - czy mutacje występują w regionach konserwatywnych.

---

## Wyniki

- tabela mutacji,
- opis chorób,
- interpretacja biologiczna.

---

## Wnioski

- dlaczego mutacje w regionach konserwatywnych są często groźniejsze?
- czy każda mutacja zmienia funkcję białka?
- jakie znaczenie ma bioinformatyka w diagnostyce medycznej?

---

# Zadanie 6.5 – Predykcja funkcji nieznanego białka

## Cel

Integracja wszystkich poznanych wcześniej metod bioinformatycznych.

---

## Wprowadzenie

W praktyce badawczej bardzo często pojawiają się:
- nowe sekwencje,
- nieopisane geny,
- hipotetyczne białka.

Bioinformatyk musi wtedy:
- przewidzieć funkcję,
- znaleźć homologów,
- przeanalizować domeny,
- zinterpretować wyniki biologicznie.

To zadanie przypomina rzeczywisty mini-projekt badawczy.

---

## Wykonaj

1. Otrzymaj od prowadzącego:
   - nieznaną sekwencję białkową,
   lub
   - wybierz hipotetyczne białko z NCBI.

2. Wykonaj:
   - BLAST,
   - analizę domen,
   - MSA,
   - analizę UniProt,
   - analizę struktury.

3. Spróbuj przewidzieć:
   - funkcję białka,
   - lokalizację komórkową,
   - możliwe znaczenie biologiczne.

4. Oceń:
   - jak pewna jest Twoja predykcja.

---

## Wyniki

- opis analizy,
- użyte narzędzia,
- homologiczne białka,
- domeny,
- przewidywana funkcja.

---

## Wnioski

- czy można przewidzieć funkcję wyłącznie na podstawie sekwencji?
- które metody były najbardziej pomocne?
- jakie są ograniczenia bioinformatycznej predykcji funkcji?

---

# Zadanie dodatkowe 1 – AlphaFold i przyszłość biologii strukturalnej

## Wykonaj

1. Przeczytaj:
   - czym jest AlphaFold.

2. Sprawdź:
   - czy wybrane białko posiada model AlphaFold.

3. Spróbuj odpowiedzieć:
   - jak sztuczna inteligencja zmienia współczesną biologię.

---

## Wnioski

- czy przewidywanie struktur może zastąpić eksperymenty laboratoryjne?
- jakie są ograniczenia modeli AI?

---

# Zadanie dodatkowe 2 – Analiza własnego białka zainteresowań

## Wykonaj

Wybierz białko:
- związane z:
  - chorobą,
  - biotechnologią,
  - mikrobiologią,
  - rolnictwem,
  - medycyną,
  - immunologią,
  - neurobiologią,
  - lub własnymi zainteresowaniami.

Przygotuj:
- krótką analizę bioinformatyczną,
- integrując:
  - UniProt,
  - BLAST,
  - domeny,
  - strukturę,
  - mutacje.

---

# Pytanie otwarte (do dyskusji)

Czy współczesna bioinformatyka pozwala już „zrozumieć” funkcję białka wyłącznie na podstawie sekwencji?

Uzasadnij odpowiedź.
