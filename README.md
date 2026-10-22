Healthcare Data Exploratory Data Analysis (EDA)
Project Overview
This project performs exploratory data analysis (EDA) on a healthcare
patient dataset using Python. It explores patient demographics, medical
conditions, admission types, and billing amounts through summary
inspection and visualizations.
Objectives
- Inspect the dataset's structure, size, columns, and data types.
- Explore the distribution of patient ages.
- Compare age distributions by gender.
- Examine the number of patients by gender and medical condition.
- Compare medical conditions across genders.
- Analyze admission-type counts.
- Compare admission types across medical conditions.
- Explore the distribution of patient billing amounts.
Dataset
The notebook loads a CSV file named healthcare_preprocessed (1).csv.

The saved notebook output shows 54,966 rows and 18 columns. The
columns are:
- Name
- Age
- Gender
- Blood_Type
- Medical_Condition
- Admission_Date
- Doctor
- Hospital
- Insurance_Provider
- Billing_Amount
- Room Number
- Admission_Type
- Discharge_Date
- Medication
- Test_Results
- Length_of_Stay
- Age_Group
- Admission_Urgency
The notebook output reports no missing values in these 18 columns. The
notebook uses a preprocessed dataset; it does not show the preprocessing
steps.
Technologies Used
- Python --- programming language
- Pandas --- loading and inspecting data, counting categories, and
  cross-tabulation
- NumPy --- numerical computing library imported in the notebook
- Matplotlib --- plotting
- Seaborn --- statistical visualizations
- Jupyter Notebook / Google Colab --- notebook environment
Analysis and Visualizations
1. Dataset inspection: displays sample rows, dataset shape, column
   names, and data types.
2. Patient age distribution: histogram of Age with a kernel
   density estimate (KDE).
3. Age distribution by gender: histogram comparing Age across
   Gender.
4. Patient count by gender: bar chart using the counts in Gender.
5. Patients by medical condition: bar chart using the counts in
   Medical_Condition.
6. Gender across medical conditions: count plot comparing gender
   groups for each medical condition.
7. Admission type distribution: bar chart showing counts for
   Admission_Type.
8. Admission types by medical condition: cross-tabulation and
   stacked bar chart comparing Medical_Condition with
   Admission_Type.
9. Billing amount distribution: histogram of Billing_Amount with
   a KDE curve.
How to Run
1. Open EDA 6.ipynb in Jupyter Notebook or Google Colab.
2. Upload healthcare_preprocessed (1).csv to the environment.
3. If necessary, update the CSV path in the notebook. The current code
   uses:
   df = pd.read_csv("/content/healthcare_preprocessed (1).csv")
4. Run the notebook cells from top to bottom.
Key Libraries
Install the main libraries if they are not already available:
pip install pandas numpy matplotlib seaborn
Notes and Limitations
- The CSV dataset is required; it was not included with the uploaded
  notebook.
- The notebook explores patterns and distributions. It does not train
  a machine-learning model or make predictions.
- The notebook does not establish medical causation or provide
  clinical recommendations.
- Although the dataset is described through patient-related fields,
  the notebook does not document the data source or define every
  category.
- The notebook includes patient names and other potentially sensitive
  fields. Use appropriately authorized data and avoid sharing
  identifiable patient information publicly.
Conclusion
This notebook provides an introductory overview of a healthcare dataset
through descriptive inspection and visualizations. It summarizes patient
age and gender distributions, medical-condition counts, admission
patterns, and billing amounts.
