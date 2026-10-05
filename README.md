# Prédicteur de Branchement Global (C++)

Ce projet est un simulateur de **prédicteur de branchement à historique global** (*Two-Level Global Branch Predictor*) développé en C++. Il permet d'évaluer le taux de précision des prédictions de branchement sur une trace d'exécution donnée.

##  Fonctionnalités

- **Historique Global configurable :** Longueur du registre d'historique paramétrable de 1 à 64 bits.
- **Deux types de prédicteurs supportés :**
  - `0` : **Prédicteur Bimodal 1 bit** (prédit la dernière direction observée pour un historique donné).
  - `1` : **Prédicteur Saturant 2 bits** (automate à 4 états : *Strongly/Weakly Not Taken*, *Weakly/Strongly Taken*).
- Calcule et affiche le **taux de précision (%)** final sur l'ensemble des branches testées.

##  Compilation

Utilisez n'importe quel compilateur C++ standard (C++11 ou ultérieur) :

```bash
g++ -O2 -std=c++11 main.cpp -o predicteur
