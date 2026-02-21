# 📊 Analiza procesu rekrutacyjnego -- Dashboard BI

## 📌 Opis projektu

Projekt przedstawia eksploracyjną analizę własnego procesu aplikowania
na stanowiska związane z Business Intelligence i analityką danych.

Celem było potraktowanie poszukiwania pracy jako mierzalnego procesu
oraz identyfikacja obserwowanych wzorców w zakresie:

-   czasu reakcji rekruterów,\
-   poziomu dopasowania kompetencyjnego,\
-   spójności poziomu stanowiska z zakresem wymagań,\
-   struktury końcowych statusów aplikacji.

Analiza obejmuje 18 aplikacji realizowanych w trybie zdalnym lub
hybrydowym oraz w oparciu o umowę o pracę.

Dane zostały zamrożone w dniu otrzymania oferty -- ewentualne późniejsze
aktualizacje statusów nie zostały uwzględnione.

------------------------------------------------------------------------

## 🧱 Zakres danych

Zebrane dane obejmowały m.in.:

-   datę wysłania aplikacji,\
-   datę pierwszej odpowiedzi,\
-   końcowy status procesu (na dzień zamrożenia danych),\
-   poziom stanowiska deklarowany w ogłoszeniu,\
-   poziom stanowiska wnioskowany na podstawie wymagań,\
-   wymagane technologie,\
-   procent spełnienia wymagań,\
-   czas reakcji rekrutera.

Dane zostały w pełni zanonimizowane.

------------------------------------------------------------------------

## 🛠 Narzędzia

-   **Excel** -- modelowanie danych i obliczenia\
-   **Power Query** -- transformacje i budowa tabel pomocniczych\
-   **Looker Studio** -- warstwa wizualna i dashboard eksploracyjny

------------------------------------------------------------------------

## ⚙ Proces analityczny

### 1️⃣ Modelowanie danych (Excel)

-   ujednolicenie nazw technologii i poziomów stanowisk\
-   wyliczenie procentowego dopasowania do wymagań\
-   obliczenie czasu reakcji rekrutera\
-   rozróżnienie poziomu stanowiska deklarowanego i wnioskowanego

Ze względu na niewielką próbę oraz obecność wartości skrajnych jako
główną miarę czasu reakcji przyjęto medianę.

------------------------------------------------------------------------

### 2️⃣ Transformacje (Power Query)

Zbudowano:

-   tabelę technologii (udział w ofertach vs odsetek reakcji)\
-   tabelę etapów procesu (wizualizacja przepływu między etapami)

Warstwa przetwarzania została oddzielona od warstwy wizualnej.

------------------------------------------------------------------------

### 3️⃣ Wizualizacja (Looker Studio)

Dashboard obejmuje:

-   KPI procesu (liczba aplikacji, % reakcji, % odrzuceń, mediana czasu
    reakcji)\
-   rozkład końcowych statusów aplikacji\
-   analizę czasu reakcji według statusu\
-   wizualizację przepływu między etapami\
-   analizę spójności poziomu stanowiska\
-   tabelę porównawczą technologii

Dashboard został zaprojektowany jako narzędzie eksploracyjne.

------------------------------------------------------------------------

## 🔍 Kluczowe obserwacje

-   Większość aplikacji nie przeszła do dalszego etapu procesu (na
    moment zamrożenia danych)\
-   Jedyna odpowiedź rekrutacyjna pojawiła się bardzo szybko\
-   Brak odpowiedzi lub odrzucenie następowały zwykle po kilku
    tygodniach\
-   Poziom dopasowania kompetencyjnego był wysoki niezależnie od wyniku
    procesu\
-   Odpowiedź rekrutacyjna dotyczyła oferty o spójnym poziomie
    stanowiska, natomiast oferty niespójne kończyły się odrzuceniem\
-   Reakcje dotyczyły głównie technologii najczęściej występujących w
    wymaganiach rynkowych (Excel, SQL, Power BI)

Ze względu na ograniczoną liczbę obserwacji wnioski mają charakter
eksploracyjny.

------------------------------------------------------------------------

## 🧠 Wartość projektu

Projekt pokazuje:

-   podejście procesowe do analizy danych\
-   modelowanie i transformację danych w Power Query\
-   projektowanie dashboardu eksploracyjnego\
-   świadome oddzielenie obserwacji od przyczynowości przy małej próbie

------------------------------------------------------------------------

## 📁 Struktura repozytorium

    ├── data/
    ├── model/
    ├── dashboard/
    └── README.md
