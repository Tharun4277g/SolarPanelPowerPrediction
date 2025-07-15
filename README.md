# ☀️ Solar Panel Power Prediction and Cost Prediction Using Machine Learning

## 📌 Overview

This project uses **Machine Learning (ML)**—primarily **Linear Regression and Artificial Neural Networks (ANNs)**—to predict solar panel power output based on environmental conditions and estimate **electricity cost savings** from solar energy. The system supports real-time user input and generates daily/monthly predictions, cost comparisons, and visual alerts using interactive UI elements.

---

## 🎯 Key Features

* ✅ Predict **DC power output** from AC power and efficiency.
* ✅ Forecast daily solar power generation based on weather and seasonal data.
* ✅ Calculate **monthly AC power savings** and compare them against predicted solar (DC) power.
* ✅ Predict **electricity cost** using slab rates and actual AC consumption.
* ✅ Visualize daily solar power output and savings.
* ✅ Interactive inputs using **ipywidgets** and colorful console feedback via **colorama**.
* ✅ Loads a pretrained ML model (`linear_regression_model.pkl`) for power forecasting.

---

## 🧰 Tech Stack

* **Language**: Python 3.8+
* **Machine Learning**: Linear Regression / ANN (trained with historical solar energy data)
* **Deployment**: Jupyter Notebook (for interactivity)
* **Visualization**: `matplotlib`, console color outputs
* **UI & Widgets**: `ipywidgets`, `colorama`
* **Model Storage**: `pickle`

---

## ⚙️ Required Libraries

Install dependencies via:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn ipywidgets colorama
```

---

## 🔁 How It Works

### 1. **Power Conversion**

* Convert AC power (user input) to DC power using solar panel efficiency.

### 2. **Model Prediction**

* Load a pretrained ML model.
* Take environmental inputs: AC Power, Temperature, Irradiance, Day of Year.
* Predict daily **DC (solar) power output** using a regression model.

### 3. **Daily Energy Usage Insights**

* Summarize daily energy generation.
* Identify days with **highest and lowest** usage.

### 4. **Electricity Bill Estimation**

* Input AC units consumed.
* Calculate electricity cost using standard **slab rates**.
* Display a **color-coded bill** and total cost.

### 5. **Monthly Prediction Module**

* Take total AC power consumed in a month, temperature, and irradiance.
* Predict solar output for **each day of the month**.
* Compute daily and total **AC power saved**.
* Visualize results with clear console formatting.

---

## 🖥️ How to Run

1. Clone or download the project files.
2. Ensure your `linear_regression_model.pkl` is in the same folder.
3. Open the notebook in Jupyter Lab or Jupyter Notebook.
4. Run all cells to:

   * Enter values interactively.
   * See predictions and bill estimations.
5. For cost prediction only:

   ```bash
   python electricity_bill.py  # (if exported as script)
   ```

---

## 📈 Sample Outputs

* 📊 Predicted solar power for each day of the month.
* 💡 Electricity bill with cost per slab and total cost.
* 🔋 Daily energy saved using solar panels.
* 🌡️ Comparison between AC and predicted DC output.

---


