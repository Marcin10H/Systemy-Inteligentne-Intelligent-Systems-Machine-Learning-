# Projekt 2: ANN - Linearly Inseparable Data 🧩

## Opis projektu

Projekt stanowi rozwinięcie koncepcji sieci neuronowych o zagadnienia klasyfikacji danych nieliniowo separowalnych. Tego typu problemy decyzyjne wymuszają porzucenie prostych modeli liniowych na rzecz rozbudowanych perceptronów wielowarstwowych (MLP) zdolnych do aproksymacji złożonych, nieliniowych granic decyzyjnych.

### 🛠️ Technologie i Środowisko
Modele sieci neuronowych oraz proces ich uczenia zostały zrealizowane w dedykowanym środowisku symulacyjnym (pliki `.acid`). 

### 🛠️ Architektura i Parametry

* **Przestrzeń danych:** Złożone, przenikające się zbiory danych dwuwymiarowych przypisane do 3 klas. Stosunek danych uczących do testowych wynosił 2:1.
* **Struktury sieci:**
  * Sieć dwuwarstwowa (2W-SIG): 1 warstwa ukryta z 50 neuronami.
  * Sieć trójwarstwowa (3W-SIG): 2 warstwy ukryte składające się kolejno z 30 i 10 neuronów.
* **Funkcja aktywacji:** Sigmoidalna z aktywnym wejściem progowym (BIAS).
* **Trening:** Zaawansowany algorytm wstecznej propagacji błędu.

### 🧪 Przebieg badań i Wyniki

Kluczowym elementem projektu była analiza topologii sieci w kontekście jej zdolności do generalizacji. Zbyt mała liczba neuronów uniemożliwiała rozwiązanie problemu, podczas gdy rozbudowana sieć 3W-SIG poprawnie "wyginała" płaszczyznę decyzyjną, otaczając poszczególne klastry danych. 
Dokonano dogłębnej wizualizacji map aktywności neuronów warstw ukrytych, co pozwoliło zaobserwować, jak sieć dekonstruuje nieliniowy problem na prostsze cechy. Ostateczny model bezbłędnie przyporządkował trudne przypadki weryfikacyjne do odpowiednich klas z precyzją bliską 100%.

---

## English Description

This project expands on neural network concepts by tackling the classification of non-linearly separable data. Such complex decision problems require the implementation of Multi-Layer Perceptrons (MLP) capable of approximating intricate, non-linear decision boundaries.

### 🛠️ Tools & Environment
The neural network models and their training process were implemented in a dedicated simulation environment (`.acid` files). 

### 🛠️ Architecture & Parameters

* **Dataset:** Complex, overlapping 2D datasets assigned to 3 classes (2:1 train-to-test ratio).
* **Topologies:** * Two-layer network (2W-SIG): 1 hidden layer with 50 neurons.
  * Three-layer network (3W-SIG): 2 hidden layers with 30 and 10 neurons, respectively.
* **Training:** Backpropagation algorithm with active BIAS inputs and sigmoid activation functions.

### 🧪 Results

The core focus was analyzing network topology concerning generalization capabilities. Deep mapping of hidden layer neuron activation revealed how the 3W-SIG network deconstructs a non-linear space by effectively "bending" decision boundaries around data clusters. The fully trained model successfully classified highly complex verification samples with near-perfect accuracy.
