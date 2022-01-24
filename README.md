# ZUM_NLP_2
Analiza sentymentu na podstawie tweet'ów w języku polskim o COVID-19.

Celem projektu jest stworzenie analizatora sentymentu do analizy polaryzacji społeczeństwa w Polsce na podstawie tweetów na temat COVID-19.


# ETAP 1
1. Pozyskanie danych 
Zebrano około 500 tys. tweetów w języku polskim na temat COVID-19. Tweety zostały pobrane za pomocą tweepy API na podstawie ich identyfikatora. Identyfikatory Tweetów zostały pobrane ze strony https://zenodo.org/record/5090588#.YZDZdmDMKUn.

2. Czyszczenie danych
Z danych zostały usunięte znaki specjalne, interpunkcyjne, URL, email, powtórzenia. Wszystkie dane tesktowe zostały przekształcone na mała literę. Usunięcie stop words.

3. Word embeddings

4. Wykorzystano K-MEANS do stworzenia clustrów (k=2)

5. Dodanie etykiet klasy 
Dane zostały oznaczone jako pozytywne/negatywne (2 klasy).


# ETAP 2
Wybierano 3 modele ML:
* Logistic regression
* Linear Suppor Vector
* Naive Bayes

Na modelach trenowano dane. Wyniki zostały zaprezentowane wykorzystując confusion matrix i roc curve.
