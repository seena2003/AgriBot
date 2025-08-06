# 🌿 AgriBot – ML/DL Powered Agriculture Assistant

A **Machine Learning** and **Deep Learning** based web application that helps in **crop recommendation**, **fertilizer suggestion**, and **plant disease detection** using AI-powered predictions.

> 🔍 _Featured on [Krish Naik's YouTube Channel](https://www.youtube.com/watch?v=zJcSod-L-Ps)_

---

## ⚠️ Disclaimer

This is a **Proof of Concept (POC)** project. The datasets used are limited and not verified for real-world agricultural use. Please **do not** rely on this application for actual farming decisions. It demonstrates the potential of AI in precision agriculture when implemented at scale with accurate and verified datasets.

---

## 💡 Motivation

Agriculture plays a crucial role in many countries, especially in India, where a large portion of the population depends on farming for livelihood. With modern technologies like **ML** and **DL**, we can support farmers in increasing their productivity and making data-driven decisions.

AgriBot provides:
- **Crop Recommendation** based on soil nutrients and weather.
- **Fertilizer Suggestion** to balance soil deficiencies or excesses.
- **Disease Prediction** from leaf images using deep learning models.

---

## 📊 Datasets Used

- [Crop Recommendation Dataset](https://www.kaggle.com/atharvaingle/crop-recommendation-dataset)
- [Fertilizer Suggestion Dataset](https://github.com/Gladiator07/AgriBot/blob/master/Data-processed/fertilizer.csv)
- [Plant Disease Detection Dataset](https://www.kaggle.com/vipoooool/new-plant-diseases-dataset)

---

## 📓 ML/DL Notebooks

- [Crop Recommendation (Kaggle)](https://www.kaggle.com/atharvaingle/what-crop-to-grow)
- [Plant Disease Detection (Kaggle)](https://www.kaggle.com/atharvaingle/plant-disease-classification-resnet-99-2)

---

## 🛠️ Tech Stack

**Frontend**:  
HTML, CSS, JavaScript, Bootstrap

**Backend**:  
Python, Flask, Git

**ML Libraries**:  
NumPy, Pandas, Matplotlib, Scikit-learn, PyTorch

**Deployment**:  
Heroku

---

## 🚀 Deployment

- **Live Site**: [AgriBot on Heroku](https://AgriBot.herokuapp.com/)  
  > _Note: May take a moment to load due to Heroku free-tier hibernation._

- **Deployment Branch**: [`deploy`](https://github.com/Gladiator07/AgriBot/tree/deploy)

---

## 💻 How to Use

### 🌾 Crop Recommendation
- Enter **N-P-K** values, **city**, and **state**.
- Temperature and humidity are auto-fetched from OpenWeatherMap API.
- Recommended crop is shown based on inputs.

> ✅ Tip: Use commonly known city names for best results.

### 💡 Fertilizer Suggestion
- Enter **N-P-K** values and the **crop name**.
- System detects nutrient deficiency or surplus.
- Recommendations are provided to balance soil.

### 🦠 Disease Detection
- Upload an image of the plant **leaf**.
- The system classifies it as **healthy or diseased**, shows crop type, disease name, and solutions.

<details>
<summary>Supported Crops</summary>

- Apple  
- Blueberry  
- Cherry  
- Corn  
- Grape  
- Orange  
- Peach  
- Pepper  
- Potato  
- Raspberry  
- Soybean  
- Squash  
- Strawberry  
- Tomato  

</details>

---

## 🧪 Run Locally

> Requirements: `git`, `conda` or `miniconda`

```bash
git clone -b deploy https://github.com/Gladiator07/AgriBot.git
cd AgriBot

# Create virtual environment
conda create -n AgriBot python=3.6.12
conda activate AgriBot

# Install dependencies
pip install -r requirements.txt

# Start server
python app.py
