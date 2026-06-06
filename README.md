# Istanbul Earthquake Assembly Area & Risk Analysis

This project aims to analyze seismic risk zones and evaluate the adequacy and accessibility of earthquake assembly areas in Istanbul. By leveraging spatial data and machine learning clustering algorithms, the project provides a data-driven approach to urban disaster preparedness.

## 📌 Project Overview
Istanbul is located in a highly active seismic zone. This project utilizes demographic data, building risk assessments, and the locations of critical facilities (fire stations, health centers, and designated assembly areas) to perform a comprehensive risk analysis. Machine learning algorithms, specifically **K-Means** and **DBSCAN**, are applied to cluster regions based on vulnerability and the availability of emergency resources.

## 🚀 Key Features
* **Geospatial Data Processing:** Integration of district (`ilce`) and neighborhood (`mahalle`) level GeoJSON data.
* **Risk Clustering:** Application of K-Means and DBSCAN algorithms to identify high-risk zones and evaluate assembly area distribution.
* **Interactive Visualization:** Folium-based interactive maps detailing earthquake assembly areas, fire stations, and health facilities against building risk data.
* **Data Integration:** Merging multiple datasets (health facilities, fire stations, building risk status) into a unified master dataset for robust analysis.

## 📂 Repository Structure
* `Istanbul_Earthquake_Analysis.ipynb`: The main Jupyter Notebook containing data preprocessing, EDA, machine learning models, and Folium map generation.
* `data/`: Directory containing the datasets used in this project.
    * `master_dataset.csv`
    * `ilce_geojson.json` / `mahalle_geojson.json`
    * `assembly_areas.csv` *(originally depremToplanmaAlani)*
    * `health_facilities.csv` *(originally saglik-tesisleri)*
    * `fire_stations.csv` *(originally itfaiye-istasyon-konumlar)*

## 🛠️ Technologies & Libraries Used
* **Python 3.x**
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (K-Means, DBSCAN, NearestNeighbors)
* **Geospatial & Visualization:** Folium, Matplotlib, Seaborn, SciPy

## ⚙️ How to Run the Project
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/istanbul-earthquake-analysis.git](https://github.com/yourusername/istanbul-earthquake-analysis.git)
Navigate to the project directory:

Bash
cd istanbul-earthquake-analysis
Ensure you have the necessary libraries installed. You can install them using pip:

Bash
pip install pandas numpy scikit-learn folium matplotlib seaborn scipy
Open the Jupyter Notebook:

Bash
jupyter notebook Istanbul_Earthquake_Analysis.ipynb
📊 Results & Insights
(Add a brief summary here of what you discovered. For example: "The DBSCAN clustering revealed that while central districts have numerous assembly areas, their capacity is insufficient for the high-density, pre-2000 building stock. K-Means clustering highlighted specific neighborhoods on the fault line lacking immediate access to health facilities.")

Note: The datasets used in this project are compiled from open data portals and local municipalities for educational and analytical purposes.
