
```markdown
# 📊 Predicting the Number of Reactions to a LinkedIn Post
A Comprehensive Machine Learning Approach  
**By Jayashree S, Livedha S, Kumaran Hariharan, R. Sanjana, T. Ragupathi**  
_Department of Data Science and Business Systems, SRM Institute of Science and Technology_

---

## 📌 Overview

This project presents a data-driven machine learning approach to predict the **number of reactions** a LinkedIn post will receive. By analyzing structured data from multiple companies, we aim to identify key factors influencing engagement and optimize post performance using advanced regression models.

📝 **Published Paper:**  
📄 *Predicting the Number of Reactions to a LinkedIn Post: A Comprehensive Machine Learning Approach*  
🔗 [IEEE Xplore Link](https://ieeexplore.ieee.org/document/10941423)

---

## 🧠 Problem Statement

LinkedIn serves as a powerful platform for professional networking and brand engagement. However, accurately forecasting engagement on posts remains a challenge. This project aims to:
- Predict the number of reactions using post and company features.
- Compare multiple regression models.
- Provide actionable insights for improving LinkedIn content strategy.

---

## 🔍 Features in the Dataset

### 🔢 Numerical Features:
- `Followers`: Number of company followers.
- `Connections`: Number of direct LinkedIn connections.
- `Comments`: Number of comments received.
- `Num Hashtags`: Hashtags used in the post.
- `Hashtag Followers`: Followers of used hashtags.
- `Views`: Number of post views.
- `Votes`: Votes received (for poll-type posts).

### 🔤 Categorical Features:
- `Name`, `Headline`, `Location`, `About`
- `Content`, `Content Links`, `Time Spent`
- `Media Type`: [`Video`, `Image`, `Article`, `Poll`]
- `Hashtags`, `Media URLs`

### 🎯 Target Variable:
- `Reactions`: Total reactions (like, celebrate, support, insightful, curious, etc.)

---

## ⚙️ Methodology

### ✅ Preprocessing
- Missing Value Handling: Median (numerical), Mode (categorical)
- Encoding: Label Encoding
- Scaling: StandardScaler
- Outlier Handling: IQR method
- Feature Selection: Recursive Feature Elimination (RFE)

### 🤖 Models Used
- Multiple Linear Regression
- Decision Tree Regression
- **Ensemble Models**: Stacking Regressor, Voting Regressor
- Support Vector Regression (RBF Kernel)
- Feed Forward Neural Network (FNN)

---

## 🧪 Model Evaluation

| Model                     | MSE (Test) | R² Score |
|--------------------------|------------|----------|
| Multiple Linear Regression | 57435.58   | 0.51     |
| Decision Tree             | 35578.68   | 0.70     |
| Ensemble (Stacking)       | 19568.58   | 0.66     |
| Support Vector Regression | 32132.18   | 0.72     |
| **Feed Forward Neural Net** | **31801.73** | **0.73**  |

- 🏆 **Best Model**: Feed Forward Neural Network (FNN)
- 🎯 **Top Predictive Features**: Followers, Media Type, Views, Comments, Connections

---

## 🧬 Neural Network Design

- 3 Hidden Layers: 256 → 128 → 64 neurons with ReLU activation
- Dropout: 0.3 (each layer)
- Optimizer: Adam (lr = 0.001)
- Loss Function: Mean Squared Error (MSE)
- Early Stopping: Used after 150 epochs

---

## 📎 Project Structure

```

├── data/
│   └── linkedin\_posts.csv
├── models/
│   ├── linear\_regression.py
│   ├── decision\_tree.py
│   ├── ensemble\_model.py
│   ├── svr\_model.py
│   └── neural\_network.py
├── notebooks/
│   └── Exploratory\_Analysis.ipynb
├── utils/
│   └── preprocessing.py
├── results/
│   └── model\_metrics.csv
├── README.md
└── requirements.txt

````

---

## 🧠 Insights & Applications

- Engagement on LinkedIn is influenced by **media type**, **company reach**, and **content relevance**.
- Advanced models outperform linear ones in capturing non-linear behavior in engagement data.
- Helpful for **marketing strategists**, **social media analysts**, and **brand consultants** to tailor impactful posts.

---

## 📬 Contact

- Jayashree S  
- Livedha S  
- T. Ragupathi (Assistant Professor)  
📧 Department of Data Science and Business Systems  
📍 SRM Institute of Science and Technology, Chennai, India

---

## 🔖 Citation

If you use this research in your work, please cite:

```bibtex
@inproceedings{livedha2024linkedin,
  title={Predicting the Number of Reactions to a LinkedIn Post: A Comprehensive Machine Learning Approach},
  author={Jayashree S and Livedha S and Kumaran Hariharan and R. Sanjana and T. Ragupathi},
  booktitle={2024 International Conference on Emerging Techniques in Computational Intelligence and Applications (ETCIA)},
  year={2024},
  organization={IEEE},
  doi={10.1109/ETCIA60778.2024.10941423},
  url={https://ieeexplore.ieee.org/document/10941423}
}
````

---

## 📜 License

This repository is for **academic and educational purposes only**. All rights reserved by the authors.

```

---

Let me know if you'd like this as a downloadable `.md` file or want a version in **LaTeX**, **presentation slides**, or **poster format** for conference use.
```
