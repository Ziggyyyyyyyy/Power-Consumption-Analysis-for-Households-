# ⚡ Power Consumption Analysis for Households

Use real-world data and machine learning to analyze and forecast household electricity consumption through an interactive web application built with Flask.

---

## 📁 Project Structure

```
CDCProject.zip
├── HouseholdElectricPower1.ipynb   # Data preprocessing, exploration & model training
├── app.py                         # Flask app backend for live predictions
├── model1.pkl                     # Pre-trained regression model
├── templates/
│   ├── index.html                 # Input form
│   └── result.html                # Result display
├── static/
│   └── meter.png                  # Visual asset
└── README.md                      # Project documentation
```

---

## ⚙️ How It Works

### 🔹 1. **Data Preparation**
- Clean and explore the dataset (`HouseholdElectricPower1.ipynb`)
- Extract features like:
  - `Global active/reactive power`
  - `Voltage`, `Global intensity`
  - `Sub-meter readings`
- Convert `Date` and `Time`, handle missing values

### 🔹 2. **Model Training**
- Trained a regression model (e.g., Linear Regression)
- Saved model as `model1.pkl` for deployment

### 🔹 3. **Web Application**
- `app.py` runs the Flask server
- HTML templates provide the user interface
- Input: Voltage, intensity, etc.
- Output: Predicted power usage

### 🔹 4. **Deployment**
- All files bundled in `CDCProject.zip` for sharing or deployment

---

## 📊 Dataset Features

- Minute-level household power measurements
- Features:
  - `Global_active_power`, `Voltage`, `Global_intensity`
  - `Sub_metering_1`, `Sub_metering_2`, `Sub_metering_3`
  - `Date & Time`

---

## ▶️ Steps to Run the Project

### 🔧 1. Clone or Extract the Project
```bash
git clone https://github.com/yourusername/household-power-analysis.git
cd household-power-analysis
```
Or unzip `CDCProject.zip`.

### 📦 2. Install Required Libraries
```bash
pip install -r requirements.txt
# OR manually:
pip install pandas numpy scikit-learn matplotlib seaborn flask
```

### 🧪 3. Run the Jupyter Notebook (Optional)
```bash
jupyter notebook HouseholdElectricPower1.ipynb
```

### 🌐 4. Run the Flask Web App
```bash
python app.py
```
Then go to: **http://127.0.0.1:5000/**

### 🖥️ 5. Use the Interface
- Enter Voltage, Intensity, Sub-meter readings
- Click **Submit** to get predicted power usage

---

## 🛠️ Tech Stack

- **Python**
- **Flask** – Backend web framework
- **Pandas**, **NumPy** – Data handling
- **Scikit-learn** – ML model
- **Matplotlib**, **Seaborn** – Visualization
- **HTML/CSS** – Frontend UI

---

## 🙌 Acknowledgments

- **Dataset**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `flask`
