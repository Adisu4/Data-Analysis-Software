Medical Device Failure Classification and Predictive Maintenance
Description
This project provides a machine learning-based solution for classifying medical device failures and optimizing predictive maintenance schedules. It processes repair data, predicts failure categories using a Naive Bayes classifier, and visualizes trends in device failures over time. The system is designed to help healthcare facilities reduce unplanned downtime and improve maintenance efficiency.

Key Features
Failure Classification: Predicts failure categories (e.g., BATT, ACC, USE) with 85% accuracy using a Naive Bayes model.

Data Analysis: Analyzes repair data from 4,000+ devices across 48 hospitals (2021-2024).

Dynamic Visualization: Generates interactive bar charts to visualize failure trends by year and category.

User-Friendly Interface: Built with Tkinter, the GUI allows users to upload data, analyze devices, and predict failure categories.

Maintenance Recommendations: Provides tailored maintenance strategies based on predicted failure categories.

Technologies Used
Programming Language: Python

Machine Learning: Scikit-learn, Naive Bayes, CountVectorizer

Data Processing: Pandas, NumPy

Visualization: Matplotlib, Seaborn

GUI Framework: Tkinter

Fuzzy Matching: FuzzyWuzzy (for device type matching)

Installation
Clone the repository:

bash
Copy
git clone https://github.com/Adisu4/Data-Analysis-Software.git
Install dependencies:

bash
Copy
pip install -r requirements.txt
Run the application:

bash
Copy
python main.py
Usage
Upload Data:

Click Select Excel File to upload your dataset (Excel file with sheets: Failure Management, Inventory, and Results of Repairs).

Process Data:

Click Process File to analyze the dataset and prepare it for predictions.

Analyze Device:

Enter a device type in the input field and click Analyze Device to view failure trends and statistics.

Predict Failure Category:

Enter a failure description and click Predict Failure Category to get the predicted failure type and recommended maintenance strategy.

Visualize Data:

Interactive bar charts are displayed for analyzed devices, showing failure trends by year and category.

Save Plot:

Click Save Plot to export the visualization as a PNG file.

File Structure
Copy
project/
├── main.py                  # Main application script
├── utils.py                 # Helper functions (data processing, analysis, etc.)
├── saved_models/            # Pre-trained models and encoders
│   ├── vectorizer.pkl       # CountVectorizer for text processing
│   ├── model.pkl            # Naive Bayes classifier
│   └── label_encoder.pkl    # LabelEncoder for category mapping
├── requirements.txt         # Python dependencies
├── README.md                # Project documentation
└── assets/                  # Images and resources
    ├── Zakynthos.png        # Background image
    └── INBIT.jpeg           # Logo
Example Dataset
The application expects an Excel file with the following sheets:

Failure Management: Contains columns Description, Machine ID, and Fault Code.

Inventory: Contains columns Device ID and General group English Name.

Results of Repairs: Contains columns Fault Code and Repair start date.

Results
Failure Classification: Achieves 85% accuracy in predicting failure categories.

Visualization: Interactive bar charts show failure trends by year and category.

Maintenance Optimization: Provides actionable recommendations to reduce downtime and improve resource allocation.

