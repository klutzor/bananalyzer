# 🍌 Bananalyzer – AI-modell för kundkonvertering

Detta projekt utvecklades som en del av en skoluppgift på ITHS med syftet att hjälpa e-handelsföretaget **KokoBananas** att identifiera vilka kundsessioner som sannolikt leder till ett köp. Genom maskininlärning förutspår modellen i realtid köpbeteende baserat på historiska sessionsegenskaper.

---

## 🎯 Syfte

Att med hjälp av dataidentifierade mönster kunna förutsäga om en kund kommer att genomföra ett köp – vilket i sin tur möjliggör riktade åtgärder i realtid (t.ex. rabatter eller personliga meddelanden).

---

## 📊 Dataset

- 12 183 kundsessioner
- 18 features (t.ex. antal sidvisningar, sessionstid, exit rates)
- Target: om kunden gjorde ett köp (klassificering)
- 15,4 % av sessionerna ledde till köp

---

## 🛠 Använda tekniker

- Python (Jupyter Notebook)
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (Decision Tree, Random Forest, GridSearchCV)
- Git & GitHub

---

## 🔍 Metod

1. **Dataförberedelse**
   - Rensning, konvertering, hantering av obalanserad data
2. **Feature Engineering**
   - Kombination av bounce rate, tid på produktsidor etc.
3. **Modellträning**
   - Baseline-modell (Decision Tree)
   - Optimerad modell (Random Forest + GridSearch)
4. **Utvärdering**
   - Threshold-tuning (0.5 → 0.3)
   - Precision, recall, confusion matrix, ROC AUC
5. **Affärspresentation**
   - Visuell rapport för icke-teknisk ledning

---

## 🤖 Resultat

- **Recall (threshold 0.3):** 88 %
- **Precision:** 25 %
- **ROC AUC:** 0.77  
- Identifierade nyckelfaktorer:
  - Sessionstid
  - Produktsidebesök
  - Exit/bounce-mönster

---

## 🧠 Lärdomar

- Betydelsen av tröskeljustering i obalanserade datamängder
- Hur man förklarar AI-resultat för icke-teknisk publik
- Modellvalets påverkan på affärsstrategier

---

## 📂 Filstruktur

```plaintext
├── Joel_Soderberg_ml_projekt.ipynb  # Notebook med hela flödet
├── requirements.txt                 # Miljökrav
├── .gitignore                       # Ignorerade filer (ex: .ipynb_checkpoints)
└── README.md                        # (den här filen)
