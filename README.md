# 📊 Visual Analysis of Crimes in India (2001-2012)

This projects has the goal of exploring and visualizing data regarding crimes in India in the time between 2001 and 2012, seeking spacial, time and demographic patterns. This project was developed as part of the Data Visualization Subject in the Computer Science Course at UTFPR.

## 🎯 Goal
Turn a complex data set into interactive view that answer questions about public security, observing crimes commited against women and other violent crimes.

## 📂 The Data
We chose to use the file (`01_District_wise_crimes_committed_IPC_2001_2012`) which is part of the [Women's Crime in India](https://www.kaggle.com/datasets/thedevastator/uncovering-trends-in-women-s-crimes-in-india-200?select=01_District_wise_crimes_committed_IPC_2001_2012.csv) dataset.
It contains information and reports about activities that violate the Indian Penal Code (IPC) divided across multiples districts. The dataset contains 33 columns + index, the most relevant being **STATE/UT**, **DISTRICT**, **YEAR**, **MURDER**, **ATTEMPT TO MURDER**, **RAPE**, with approximately 9016 instances.

## 📈 Views Created

The project features 5 interactive views (available in [/plots](./plots) directory):

1. **National Tendencies ([E02_grafico_tendencias_crimes.html](./plots/E02_grafico_tendencias_crimes.html))**:
  - **_Question_: How have the different categories of crime evolved in over the years?**
  - **_Technique_: Interactive Line Chart. Focus on the temporal dimension comparing the volume of each category**
2. **District's Criminal Profile ([E02_bubble_chart_animado.html](./plots/E02_bubble_chart_animado.html))**:
  - **_Question_: Is there a correlation between violent crimes and crimes against property?**
  - **_Technique_: Bubble Chart (Scatter plot) animated over time. Maps multiple dimensions**
3. **Criminal Composition by State ([E03_grafico_barras_100.html](./plots/E03_grafico_barras_100.html))**:
  - **_Question_: What is the crime proportion (typology) in the 10 states with highest criminal rates?**
  - **_Technique_: 100% Stacked Bar Chart. Hides the "absolute volume" to revel the internal distribution**
4. **Inequality and distribution ([E03_boxplot_animado.html](./plots/E03_boxplot_animado.html))**:
  - **_Question_: Is the criminal rate homogeneous within the state or are there outliers districts?**
  - **_Technique_: Time-animated Box Plot. Focuses on the statistical view of medians and identifying outliers**
5. **Crime's Geography ([E03_mapa_interativo_dropdown.html](./plots/E03_mapa_interativo_dropdown.html))**:
  - **_Question_: Where are the biggest geographic hotspots for general criminality and violence against women?**
  - **_Technique_: Interactive Choropletic Map. Uses dropdowns menu to switch between different metrics.**

## 🛠️ Technologies
- **Python 3.11**
- **Pandas** (Data Cleaning, aggregation and data transformation)
- **Plotly** (Creation of Interactive views)

## 🚀 How to Run this Project Locally 
In case you want to check or toy with the `ipynb` file, you can clone this repository. Just make sure you have conda/miniconda installed.

1. Clone the repository:
```bash
git clone https://github.com/GalafassiNAT/data-visualization.git
cd data-visualization
```
2. Create the virtual environment using the configuration file:
```bash
conda env create -f environment.yml
```
3. Activate the environment:
```bash
conda activate data_viz
```
4. Open Jupyter Notebook:
```bash
jupyter notebook
```
