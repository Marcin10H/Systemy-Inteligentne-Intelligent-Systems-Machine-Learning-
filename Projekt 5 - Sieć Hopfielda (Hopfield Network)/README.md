# Projekt 5: Hopfield Network - Autoassociative Memory 🌌

## Opis projektu

Zaawansowany projekt implementujący Sieć Neuronową Hopfielda – rekurencyjną architekturę (RNN) pełniącą funkcję pamięci autoasocjacyjnej. System ten nie służy do klasyfikacji, lecz do odtwarzania i rekonstrukcji oryginalnych ("idealnych") wzorców na podstawie obrazów silnie zniekształconych, zaszumionych lub częściowo zasłoniętych.

### 🛠️ Technologie i Środowisko
Modele sieci neuronowych oraz proces ich uczenia zostały zrealizowane w dedykowanym środowisku symulacyjnym (pliki `.acid`). 

### 🛠️ Metody Uczenia i Odczytu

* **Rozdzielczość danych:** Testy przeprowadzono na matrycach znaków w rozdzielczościach 8x10 oraz 16x20 pikseli.
* **Algorytmy Zapisu (Trening):** Przeanalizowano różne warianty uczenia wag synaptycznych, badając ich wpływ na pojemność pamięci sieci:
  * Reguła Hebba (RH)
  * Reguła Pseudoinwersji (RP)
  * Reguła Rzutowania Delta (RRD)
  * Zmodyfikowana Reguła Perceptronu (ZRP)
* **Algorytmy Odczytu:** Sprawdzono zbieżność sieci używając metody synchronicznej (MS) oraz asynchronicznej (losowa MAL i cykliczna MAC).

### 🧪 Przebieg eksperymentów i Wyniki

Sieć poddano ekstremalnym testom typu "stress-test", wprowadzając do obrazów wejściowych szum o natężeniu osiągającym nawet 70%, a także ucinając bądź zasłaniając fragmenty znaków. 
Wyniki jednoznacznie dowiodły, że zaawansowane reguły zapisu (takie jak Reguła Rzutowania Delta czy Zmodyfikowana Reguła Perceptronu) pozwalają na bezbłędne (100% poprawności) zrekonstruowanie oryginalnego znaku z szumu, który dla ludzkiego oka jest całkowicie nieczytelny. Projekt udowodnił potężne możliwości sieci rekurencyjnych w dziedzinie odszumiania sygnałów i rekonstrukcji danych.

---

## English Description

An advanced project implementing the Hopfield Neural Network—a Recurrent Neural Network (RNN) architecture acting as autoassociative memory. Rather than classifying data, this system reconstructs and retrieves original ("ideal") image patterns from inputs that are heavily distorted, noisy, or partially occluded.

### 🛠️ Tools & Environment
The neural network models and their training process were implemented in a dedicated simulation environment (`.acid` files). 

### 🛠️ Learning & Retrieval Methods

* **Data Resolution:** Experiments were conducted on character matrices sized 8x10 and 16x20 pixels.
* **Memory Storage Algorithms (Training):** Evaluated multiple synaptic weight learning rules to test memory capacity:
  * Hebbian Rule (RH)
  * Pseudo-inverse Rule (RP)
  * Delta Projection Rule (RRD)
  * Modified Perceptron Rule (ZRP)
* **Retrieval Algorithms:** Tested network convergence using Synchronous (MS) and Asynchronous (Random MAL and Cyclic MAC) updating methods.

### 🧪 Results

The network was subjected to severe stress tests, including noise levels reaching up to 70% and structural occlusions. The results conclusively proved that advanced training rules (like the Delta Projection Rule) enable the network to flawlessly reconstruct original characters from noise that is completely illegible to the human eye. This effectively demonstrates the immense power of RNNs in signal denoising and data recovery.
