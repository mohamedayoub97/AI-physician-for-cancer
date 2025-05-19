# 🧠💉 AI-Physician-for-Cancer – Your Virtual Oncology Assistant

Welcome to **AI-Physician-for-Cancer**!  
An AI-powered virtual physician that helps detect **malignant (cancerous)** and **benign** tumors with deep learning.  
This intelligent assistant brings the power of modern medicine and artificial intelligence together in a mission to save lives. ❤️

---

## 🧬 What Is It?

🔎 **AI-Physician-for-Cancer** is a deep learning project that classifies breast cancer tumors as either:

- `1` → **Malignant**
- `0` → **Benign**

It uses a dense neural network trained on medical data to assist doctors, researchers, and students in identifying cancer risk from diagnostic features extracted from biopsies.

---

## 📦 Tech Stack

| Tool/Library       | Purpose                         |
|--------------------|----------------------------------|
| 🐍 Python          | Main programming language        |
| 📊 Pandas          | Data handling and manipulation   |
| 🔢 NumPy           | Numerical operations             |
| 🤖 TensorFlow      | Deep learning & model training   |
| 🧪 scikit-learn    | Data preprocessing & evaluation  |

---

## 📁 Dataset Info

🔗 **Source**: [Breast Cancer Wisconsin (Diagnostic) Data Set](https://gist.github.com/KhanradCoder/35a6beea49e5b9ba62797e595a9626c0)  
📄 **File**: `cancer.csv`

Features:
- 30 numerical input features (e.g., radius, texture, smoothness)
- 1 binary label column: `diagnosis(1=m, 0=b)`

---

## 🧠 Model Architecture

```text
Input Layer (30 features)
        ↓
Dense Layer (256 neurons, ReLU)
        ↓
Dense Layer (256 neurons, ReLU)
        ↓
Output Layer (1 neuron, Sigmoid)
```

✅ **Loss Function**: `binary_crossentropy`  
⚙️ **Optimizer**: `adam`  
📈 **Metrics**: `accuracy` (can add precision/recall)

---

## 🚀 Getting Started

### 🔧 Setup Instructions

1. **Clone the repo**:
   ```bash
   git clone https://github.com/your-username/AI-Physician-for-Cancer.git
   cd AI-Physician-for-Cancer
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas tensorflow scikit-learn
   ```

3. **Add dataset**:
   - Download `cancer.csv` [here](https://gist.github.com/KhanradCoder/35a6beea49e5b9ba62797e595a9626c0)
   - Place it in the project root directory

4. **Train the model**:
   ```bash
   python ai_in_15.py
   ```

---

## 📊 Model Evaluation

After training, the model will:
- ✅ Output test accuracy
- 🔍 Provide insights on performance
- 🧠 Be ready for prediction and deployment

📌 Add this to improve evaluation:
```python
from sklearn.metrics import classification_report, confusion_matrix

# Predict
y_pred = (model.predict(x_test) > 0.5).astype("int32")

# Evaluate
print(confusion_matrix(y_test, y_pred))
print(classification_report(y_test, y_pred))
```

---

## 🎯 Features To Add (Next Steps)

✅ Normalize the dataset using `StandardScaler`  
✅ Use `ReLU` instead of `Sigmoid` for hidden layers  
🔄 Add `EarlyStopping` and `ModelCheckpoint` callbacks  
📈 Log metrics using TensorBoard  
🖥️ Build a GUI or Web App using Streamlit or Flask  
☁️ Deploy model as a REST API (e.g., FastAPI + Heroku)

---

## ⚠️ Disclaimer

> **⚠️ Not for clinical use!**  
> This tool is for **educational and research purposes only**.  
> It is not intended to replace medical diagnosis or professional advice. Always consult certified healthcare professionals.

---

## 👨‍⚕️ Author

👤 **Mohamed Ayoub Essalami**  
🎓 Physics & Engineering Enthusiast | Passionate about AI in Healthcare  
📬 Reach me on [LinkedIn](https://www.linkedin.com) or via GitHub

---

## 🧠 Inspiration

Inspired by the fusion of:
- 🧬 Medical science
- 🖥️ Artificial Intelligence
- 💡 The pursuit of saving lives through innovation

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## ⭐️ Show Your Support

If you found this project helpful or interesting:
- ⭐️ Star the repo
- 🍴 Fork it
- 📢 Share it

Let’s use AI for good. Together. ❤️
