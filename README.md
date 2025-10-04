# 🪷 SIH-Ayurvedic Prakriti Diagnosis System  
**AI-based Tridosha Prediction using XGBoost and FastAPI**

---

## 📖 Overview  
This project is an **AI-powered Ayurvedic Diagnosis System** that predicts the three doshas — **Vata**, **Pitta**, and **Kapha** — based on user responses to 15 fundamental Ayurvedic questions.  
It aims to digitally replicate the **initial Ayurvedic assessment** process and provide users with insights into their **body constitution (Prakriti)** and **dosha balance**.

The system predicts each dosha level as **Low**, **Medium**, or **High**, and generates a **detailed interpretative report** with lifestyle recommendations.

---

## ⚙️ Key Features  
✅ 15-question form inspired by Ayurvedic consultation practices  
✅ Predicts **Vata, Pitta, Kapha** levels (Low / Medium / High)  
✅ **97% model accuracy** on the synthetic dataset  
✅ **XGBoost Classifier** for robust and explainable results  
✅ **FastAPI backend** integrated with an **HTML/CSS frontend**  
✅ Automatic preprocessing using **scikit-learn pipelines**  
✅ Dynamically generated **Ayurvedic report** for each user  

---

## 🧠 How It Works  

1. **User Input (Form Interface):**  
   The user fills in 15 basic questions covering lifestyle, sleep, digestion, mood, and physical traits.  

2. **Data Preprocessing:**  
   - The system uses **scikit-learn** preprocessing pipelines.  
   - Encodes categorical responses (e.g., “Very Low”, “Moderate”, “High”).  
   - Normalizes numerical features for consistency.  

3. **Model Prediction:**  
   - The processed input is passed to the trained **XGBoost Classifier** (multi-output model).  
   - Predicts probabilities for **Vata**, **Pitta**, and **Kapha** doshas.  
   - Maps predictions to levels:  
     - **0–0.4 → Low**  
     - **0.4–0.7 → Medium**  
     - **0.7–1.0 → High**

4. **Report Generation:**  
   A custom report is displayed in the frontend (HTML/CSS) with:  
   - Dosha levels (Low/Medium/High)  
   - Dominant dosha type  
   - Personalized Ayurvedic recommendations  

---

## 📊 Example Output  

| Dosha | Level | Description |
|--------|--------|-------------|
| **Vata** | High | Energetic, creative, but may face restlessness or dryness. Maintain warmth and grounding habits. |
| **Pitta** | Medium | Balanced metabolism and focus. Avoid excess heat and spicy foods. |
| **Kapha** | Low | Less prone to heaviness, but maintain regular movement. |

🪔 **Overall Diagnosis:** *Pitta-Vata Dominant*  
💡 **Recommendation:** Follow a cooling diet, prioritize hydration, and manage stress with meditation.

---

  

