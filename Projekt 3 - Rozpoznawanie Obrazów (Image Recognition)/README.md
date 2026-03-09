# Projekt 3: Image Recognition & Classification Metrics 👁️

## Opis projektu

Kompleksowy system rozpoznawania obrazów oparty na głębokich sieciach neuronowych. Projekt obejmuje klasyfikację danych wielowymiarowych – monochromatycznych obrazów znaków graficznych (liter i cyfr) oraz głęboką ewaluację modelu z wykorzystaniem standardowych w analityce danych metryk statystycznych.

### 🛠️ Technologie i Środowisko
Modele sieci neuronowych oraz proces ich uczenia zostały zrealizowane w dedykowanym środowisku symulacyjnym (pliki `.acid`). 

### 🛠️ Zbiory danych i Metodologia

* **Rozpoznawanie wzorców:** Zbiór danych stanowiły rastrowe obrazy 5 znaków (litery: M, A, R, C oraz cyfra 3) w rozdzielczościach 5x7 oraz 10x14 pikseli.
* **Wprowadzanie zakłóceń:** W celu nauki generalizacji oraz zapobiegania przeuczeniu (overfitting), do zbiorów testowych wprowadzono sztuczny szum (losową negację pikseli) na poziomach od 5% do 50%.
* **Analiza medyczna:** Klasyfikacja wielowymiarowych, rzeczywistych danych medycznych (np. detekcja nowotworów - Breast Cancer z repozytorium UCI) z zastosowaniem walidacji krzyżowej (k-fold cross-validation).

### 📊 Ewaluacja modelu (Metryki)

Wyniki eksperymentów zostały poddane rygorystycznej analizie statystycznej przy użyciu:
* **Macierzy pomyłek (Confusion Matrix)**
* **Accuracy (ACC)** - Ogólna dokładność modelu.
* **Sensitivity (TPR - True Positive Rate)** - Czułość klasyfikatora.
* **Specificity (TNR - True Negative Rate)** - Swoistość klasyfikatora.

### 🧪 Wyniki

Model uczony na matrycach 10x14 bez nałożonego szumu osiągnął wybitne wyniki (ACC = 1.0, TPR = 1.0, TNR = 1.0). Udowodniono, że odpowiednio zoptymalizowana sieć potrafi skutecznie rozpoznawać wzorce nawet przy znacznym zaszumieniu (do 30% uszkodzeń pikseli), zachowując wysoką zdolność predykcyjną.

---

## English Description

A comprehensive image recognition system based on Deep Neural Networks. The project involves multi-dimensional classification of monochrome images (characters and digits) and rigorous model evaluation using standard Data Science statistical metrics.

### 🛠️ Tools & Environment
The neural network models and their training process were implemented in a dedicated simulation environment (`.acid` files). 

### 🛠️ Datasets & Methodology

* **Pattern Recognition:** Raster images of 5 characters (M, A, R, C, 3) at 5x7 and 10x14 pixel resolutions.
* **Noise Injection:** To promote generalization and prevent overfitting, artificial noise (random pixel negation ranging from 5% to 50%) was injected into the test sets.
* **Medical Analysis:** Classification of real-world multi-dimensional medical data (e.g., Breast Cancer dataset from UCI) utilizing k-fold cross-validation.

### 📊 Model Evaluation

Performance was quantified using standard analytical tools:
* **Confusion Matrix**
* **Accuracy (ACC)**
* **Sensitivity (True Positive Rate - TPR)**
* **Specificity (True Negative Rate - TNR)**

### 🧪 Results

The model trained on 10x14 matrices without noise achieved perfect scores (ACC = 1.0, TPR = 1.0, TNR = 1.0). The study demonstrated that an optimized network can maintain robust predictive capabilities and recognize patterns effectively even when inputs suffer from significant noise degradation (up to 30% corrupted pixels).

