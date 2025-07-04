⚡ Power Consumption Analysis for Households
Use real-world data and machine learning to analyze and forecast household electricity consumption within an interactive web application.

Project Structure
-CDCProject.zip – Full project package (code, data, docs)
- HouseholdElectricPower1.ipynb – Jupyter notebook for data exploration, cleaning, and modeling
- app.py – Flask web application for interactive predictions
- model1.pkl – Pre-trained machine learning model
- index.html & result.html – Web interface templates
- meter.png – Web app visual asset
- README.md – Project documentation
  
⚙️ Working
1. Data Preparation: The notebook preprocesses and explores household power consumption data, deriving features such as global reactive power, intensity, and sub-meter readings.
2. Model Training: A regression model is trained to forecast power usage. The trained model is stored in `model1.pkl`.
3. Web Application: The Flask application accepts input parameters from households. The application downloads the trained model, processes user input, and outputs estimated power consumption.
4. Project Bundle: The entire project code is bundled in `CDCProject.zip` for convenience while sharing across different environments or system deployment.
The project utilizes a household electric power consumption dataset that contains the following features:
- Global active/reactive power
- Voltage
- Global intensity
- Sub-metering (kitchen, laundry, etc.)
  
Acknowledgments
- Data: Home electrical power consumption data set
- Libraries: pandas, numpy, scikit-learn, Flask, seaborn, matplotlib
