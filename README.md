# 🚀 Applied Data Science Capstone Project
### 🎯 Predicting First Stage Landing Success of SpaceX Falcon 9 Rockets

---

## 📄 Project Overview

SpaceX has revolutionized the space industry by drastically reducing launch costs, largely due to its ability to reuse the first stage of Falcon 9 rockets. A typical Falcon 9 launch costs approximately **$62 million**, compared to competitors who charge over **$165 million**. This cost-effectiveness hinges on the ability to recover and reuse the rocket's first stage.

This project aims to **predict whether the first stage of a Falcon 9 rocket will land successfully**, leveraging machine learning and data science tools. Accurate predictions will enable better cost estimations and strategic planning.

---

## ❓ Key Questions

- 📦 How do variables like payload mass, launch site, number of previous flights, and orbit affect the success of the first stage landing?
- 📈 Has the landing success rate improved over time?
- 🧠 Which classification algorithm gives the best performance for this problem?

---

## 🧪 Methodology

### 1. 🔍 **Data Collection**
- 🌐 **REST API:** Pulled launch data from the SpaceX public API.
- 🕸️ **Web Scraping:** Used BeautifulSoup to extract data from Wikipedia’s Falcon 9 launch history page.

### 2. 🧹 **Data Wrangling**
- ✅ Filtered only Falcon 9 launches.
- 🧮 Replaced missing values using mean imputation.
- 🧩 Applied One-Hot Encoding to categorical features: `Orbit`, `LaunchSite`, `LandingPad`, `Serial`.

### 3. 📊 **Exploratory Data Analysis (EDA)**
- 🖼️ Visualized launch frequencies, success rates, and outcomes using Matplotlib and Seaborn.
- 🧾 Used SQL for advanced aggregations and insights on launch sites, orbit types, and success distributions.

### 4. 🌍 **Interactive Visualization**
- 🗺️ **Folium:** Plotted launch sites and outcomes on a world map.
- 📊 **Plotly Dash:** Built a web application featuring:
  - 🔽 Dropdown menu for site selection
  - 🎚️ Range slider for payload mass
  - 🥧 Pie chart showing success rates
  - 📈 Scatter plot comparing payload vs. success

### 5. 🤖 **Machine Learning & Modeling**
- 🧪 Standardized the feature set
- ✂️ Split the data into training and testing sets
- 🔧 Trained and optimized:
  - 🔹 Logistic Regression
  - 🔸 Support Vector Machines (SVM)
  - 🌲 Decision Trees
  - 🌳 Random Forest
- 🛠️ Performed hyperparameter tuning with GridSearchCV
- 📏 Evaluated models using accuracy on test data

---

## 📈 Results

- 📌 Found that `Orbit`, `LaunchSite`, and `PayloadMass` are major predictors of success.
- 📅 Observed a significant upward trend in landing success over the years.
- 🏆 **Best performing model:** SVM with RBF kernel, followed by Random Forest.

---

## ⚙️ Tech Stack

- 🐍 **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- 🧰 **Tools**: Jupyter Notebook, Git & GitHub  
- 🌐 **Deployment**: Flask / Streamlit, Render (for live hosting)  

---

## 🚧 Future Improvements

- 🖥️ Add a Streamlit frontend for real-time interactive predictions
- 🔁 Automate model retraining using scheduled jobs
- 🔄 Implement a CI/CD pipeline using GitHub Actions

---

## 📬 Contact

For any queries or collaboration, reach out:  
📧 **sai.subbu.in@gmail.com**

---

## 📄 License

This project is open-source and available under the terms of the MIT License.
