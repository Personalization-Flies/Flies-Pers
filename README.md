# Nasze Eksperymenty

Witaj na stronie przedstawiającej nasze najnowsze eksperymenty w dziedzinie sztucznej inteligencji. Poniżej znajdziesz szczegółowy opis każdego z projektów, nad którymi pracowaliśmy.

## Zespół

Nasz zespół składa się z doświadczonych programistów i naukowców zajmujących się AI, którzy mają na celu rozwijanie nowatorskich rozwiązań w dziedzinie przetwarzania języka naturalnego i uczenia maszynowego.

- **Michał Madej** 
- **Dawid Jędrzejewski** 
- **Katarzyna Broczkowska**
- **Mikołaj Libura**
- **dr inż. Jan Kocoń** - Opiekun Pracy
- **prof. dr hab. inż. Przemysław Kazienko** - Opiekun Pracy

## Projekty

### Eksperyment 1: Generowanie rymów przez LLM'y 

**Cel:** 

**Opis:** 

**Wyniki:**

### Eksperyment 2: Personalizacja w zadaniu klasyfikacji

**Cel:** 

**Opis:** 
Baseline jest modelem służącym jedynie jako niepersonalizowane odniesienie, dzięki któremu możliwa jest wizualizacja przyrostu.

<img src="Photos/baseline.jpg" alt="Baseline" style="width: 400px; height: auto;">

OneHot — model ten jest niezwykle podobny do omawianego wcześniej podejścia z użyciem
User ID. W tym przypadku wartość User ID jest dodawana w postaci wektora kodowanego w sposób one-hot do wektora osadzeń pochodzącego z modelu językowego.

<img src="Photos/OneHot.jpg" alt="OneHot" style="width: 400px; height: auto;">

HuBi-Formula - architektura opierająca się na wyliczonej wcześniej wartości Human Bias.
Struktura tego modelu jest identyczna do modelu OneHot, różniąca się obecnością wspomnianej
miary HB zamiast wartości User ID. 

<img src="Photos/Formula.jpg" alt="Formula" style="width: 400px; height: auto;">

HuBi-Simple - jest już pełnym modelem predykcyjnym, bazowanym na idei zaczerpniętej
z dziedziny systemów rekomendacyjnych. Do uzyskania predykowanej etykiety model wykorzystuje trzy różne komponenty, są nimi wspomniane wcześniej zamrożone osadzenia z modelu
językowego, wyuczalna wartość HB oraz wartość Word-Bias. Zmianą w porównaniu do wcześniejszych modeli jest zdolność miary HB do nauki podczas etapu treningu. Nie jest ona już
prekalkulowana przed głównym treningiem modelu

<img src="Photos/Simple.jpg" alt="Simple" style="width: 400px; height: auto;">

HuBi-Medium to model również inspirowany metodami systemów rekomendacyjnych, a dokładnie metodą Neural Collaborative Filtering. W porównaniu do modelu HuBi-Simple
tworzy on wielowymiarowy wektor osadzeń zawierający informacje o użytkowniku. Dodatkowo
jego długość jest hiperparametrem, co pozwala na dostosowanie go do swoich potrzeb.

<img src="Photos/medium.jpg" alt="Medium" style="width: 400px; height: auto;">


**Wyniki:** 

<img src="Photos/Dawid.png" alt="Wykres_zysku emocji" style="width: 1200px; height: 550px;">

<img src="Photos/Michal.png" alt="Wykres_zysku humoru" style="width: 1200px; height: 550px;">

<img src="Photos/Kasia.png" alt="Wykres_zysku hejtu" style="width: 1200px; height: 550px;">

<img src="Photos/Miki.png" alt="Wykres_wydźwięku" style="width: 1200px; height: 550px;">
**Więcej informacji:**

## Kontakt

Jeśli masz pytania dotyczące naszych projektów, prosimy o kontakt:

- Email: [kontakt@naszazespół.com](mailto:kontakt@naszazespół.com)
