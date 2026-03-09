# Projekt 1: Multilayer Perceptron (MLP) - Linearly Separable Data 🧠

## Opis projektu

Projekt koncentruje się na budowie, treningu i ewaluacji Sztucznych Sieci Neuronowych (ANN) przeznaczonych do klasyfikacji danych dwuwymiarowych, które są liniowo separowalne. Głównym celem było zbadanie wpływu różnych architektur sieci, funkcji aktywacji oraz hiperparametrów procesu uczenia na szybkość zbieżności i zdolność modelu do poprawnej klasyfikacji.

### 🛠️ Technologie i Środowisko
Modele sieci neuronowych oraz proces ich uczenia zostały zrealizowane w dedykowanym środowisku symulacyjnym (pliki `.acid`). 

### 🛠️ Architektura i Parametry

* **Przestrzeń danych:** Dane dwuwymiarowe (x1, x2), podzielone na 3 odrębne klasy. Zbiór danych składał się ze 120 próbek uczących, 60 próbek testowych oraz dedykowanego zbioru weryfikującego.
* **Kodowanie:** Wykorzystano kodowanie klas w formacie `1-of-N` (One-Hot Encoding).
* **Testowane topologie sieci:** * Jednowarstwowa z funkcją skokową (1W-SKOK).
  * Dwuwarstwowa z funkcją skokową (2W-SKOK).
  * Jednowarstwowa z ciągłą funkcją sigmoidalną (1W-SIG).
  * Dwuwarstwowa z ciągłą funkcją sigmoidalną (2W-SIG).
* **Algorytmy uczące:** Klasyczna reguła perceptronowa (dla funkcji skokowych) oraz algorytm wstecznej propagacji błędu - Backpropagation (dla funkcji ciągłych).

### 🧪 Przebieg badań i Wyniki

W trakcie eksperymentów manipulowano współczynnikiem uczenia (learning rate) oraz współczynnikiem momentum. Zbadano wizualnie płaszczyzny decyzyjne oraz poziomy aktywności poszczególnych neuronów dla danych testowych. 
Najlepsze rezultaty osiągnięto dla sieci wykorzystujących ciągłe funkcje aktywacji trenowanych metodą wstecznej propagacji z odpowiednio dobranym momentum. Model osiągnął **100% dokładności klasyfikacji (Accuracy = 1.0)** zarówno na zbiorze treningowym, jak i testowym, generując bezbłędne podziały liniowe przestrzeni wejściowej.

---

## English Description

This project focuses on the construction, training, and evaluation of Artificial Neural Networks (ANN) designed to classify 2D linearly separable data. The primary objective was to investigate the impact of various network architectures, activation functions, and training hyperparameters on convergence speed and classification capability.

### 🛠️ Tools & Environment
The neural network models and their training process were implemented in a dedicated simulation environment (`.acid` files). 

### 🛠️ Architecture & Parameters

* **Dataset:** 2D spatial data distributed across 3 classes. The dataset comprises 120 training samples, 60 test samples, and an independent verification set.
* **Encoding:** `1-of-N` (One-Hot Encoding) for class labels.
* **Topologies tested:** Single-layer and Two-layer perceptrons utilizing both hard-limit (step) and continuous (sigmoid) activation functions.
* **Learning Algorithms:** Perceptron learning rule and the Backpropagation algorithm.

### 🧪 Results

By tuning the learning rate and momentum, the network's decision boundaries and neuron activation levels were thoroughly mapped. The optimal configurations utilizing sigmoid activation functions and Backpropagation achieved **100% classification accuracy** across all datasets, successfully establishing perfect linear decision boundaries.

