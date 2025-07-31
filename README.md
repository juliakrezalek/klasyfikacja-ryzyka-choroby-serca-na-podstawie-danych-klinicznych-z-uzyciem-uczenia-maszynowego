# **Klasyfikacja ryzyka choroby serca na podstawie danych klinicznych**

### **Cel projektu:**  
Celem projektu było zbudowanie modelu klasyfikacyjnego, który przewiduje ryzyko choroby serca (0 lub 1) na podstawie danych klinicznych, takich jak: 
- Dane demograficzne - wiek i płeć pacjenta
- Objawy kliniczne - typ bólu w klatce piersiowej, obecność dławicy wysiłkowej
- Parametry fizjologiczne - ciśnienie tętnicze w spoczynku, poziom cholesterolu, maksymalne tętno
- Wyniki badań EKG - obniżenie i nachylenie odcinka ST
- Inne wyniki badań - wynik badania talowego i liczba naczyń wieńcowych widocznych we fluoroskopii

### **Projekt pozwala na oszacowanie prawdopodobieństwa ryzyka choroby serca u nowego pacjenta na podstawie wybranych cech.**

### **Źródło danych:**  
Dane pochodzą z  platformy [Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)  
Zbiór zawiera 105 rekordów i 14 cech (13 zmiennych niezależnych + 1 zmienna zależna - ryzyko choroby serca)

### **Wykorzystane narzędzia:**
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn (regresja liniowa, drzewo decyzyjne, Random Forest)
- Google Colab

### **Etapy projektu:**  
**1.	Eksploracyjna analiza danych (EDA):**
-	Sprawdzenie struktury danych, typów zmiennych i brakujących wartości
-	Analiza rozkładów zmiennych, wykrycie odstających wartości
-	Wizualizacje z wykorzystaniem wykresów (histogramy, wykresy pudełkowe)
-	Ocena korelacji między zmiennymi

**2.	Przygotowanie danych:**
- Podział danych na zbiór treningowy (80%) i testowy (20%)
- Wydzielenie zbioru walidacyjnego do oceny modeli i ograniczenia ryzyka przeuczenia
- Standaryzacja zmiennych numerycznych
- Kodowanie zmiennych kategorycznych

**3.	Budowa i porównanie modeli klasyfikacyjnych:**
- Przetestowano regresję logistyczną, drzewo decyzyjne i Random Forest
- Ocena za pomocą miar: accuracy, precision, recall, F1 score
- Analiza macierzy pomyłek dla każdego modelu
- Zastosowano ograniczenie głębokości i liczby drzew w Random Forest, aby zredukować overfitting
- Finalny wybór modelu oparty na wynikach F1 i analizie błędów

### **Wyniki:**
- Najlepszy wynik uzyskano dla modelu ograniczonego **Random Forest**, który osiągnął najwyższy wynik F1 przy zachowaniu akceptowalnego poziomu generalizacji
- Model wykazuje się dobrą równowagą między precyzją a czułością, co czyni go użytecznym w kontekście diagnostyki medycznej

Projekt stworzony przez **Julię Krężałek** w ramach nauki i budowy portfolio data science.
