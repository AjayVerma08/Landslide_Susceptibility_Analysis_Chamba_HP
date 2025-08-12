<h1>Geospatial Approach to Landslide Susceptibility Analysis of Chamba district of Himachal Pradesh using statistical (AHP) and machine learning (XGBoost) models.</h1>

<h3>Overview</h3>
<p>This research project evaluates landslide susceptibility in Chamba district, Himachal Pradesh, using two distinct methodologies:
    <ul>
        <li>Analytic Hierarchy Process (AHP) : A multi-criteria decision-making approach based on expert-weighted factors.</li>
        <li>XGBoost Machine Learning Model : A data-driven predictive model trained on historical landslide data and geospatial variables.</li>
    </ul>
    The study integrates 16 causative factors, including slope, precipitation, lithology, land use, and proximity to roads and rivers, to generate high-resolution susceptibility maps. The results provide insights into high-risk zones, supporting disaster risk management and land-use planning in the Himalayan region.
</p>

<h3>Key Features</h3>
<ul>
    <li>Comparative Analysis : Evaluates the performance of AHP (expert-driven) vs. XGBoost (data-driven) models.</li>
    <li>High Predictive Accuracy : XGBoost achieved 85.36% accuracy and an AUC of 0.91, outperforming AHP.</li>
    <li>Geospatial Data Integration : Uses DEM, satellite imagery, geological surveys, and landslide inventories.</li>
    <li>Reproducible Methodology : Includes Python scripts (XGBoost training) and GIS workflows (AHP-weighted overlay).</li>
</ul>

<h3>Methodology</h3>
<img width="1063" height="712" alt="Image" src="https://github.com/user-attachments/assets/1b84fd64-5c07-48c7-95d6-bce69a76c0a8" />

<h3>Results</h3>
<ol>
    <li>XGBoost outperformed AHP, with higher accuracy (85.36% vs. ~75-80%) and better spatial precision.</li>
    <li>Primary risk factors: Proximity to roads, slope steepness, and precipitation.</li>
    <li>High-risk zones: Central and southwestern Chamba, correlating with dense road networks and unstable lithology.</li>
</ol>

<h3>Usage</h3>
-> For AHP: Run weighted overlay in ArcGIS Pro by generating criteria weights similar to the uploaded CSV.
-> For XGBoost: Execute model_training.py with input CSV (training data).
-> Visualization: Compare susceptibility maps using QGIS/ArcGIS.

<h3>Requirements</h3>
-> Python 3.8+ (XGBoost, pandas, scikit-learn, rasterio)
-> ArcGIS Pro / QGIS (AHP analysis)
-> ALOS PALSAR DEM & Sentinel-2 data
-> Other Spatial Data according to region of interest
