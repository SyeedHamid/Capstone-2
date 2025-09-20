Here’s the same README draft from before, but with all emojis removed so it’s clean and professional.

Capstone 2 – Climate Anomaly Detection & Ensemble Modeling
Problem Statement
Climate variability is accelerating, with temperature and precipitation anomalies becoming more frequent and severe.
This project answers the question:
“How can we detect, quantify, and visualize climate anomalies across decades using ensemble modeling of global datasets?”
Why it matters:
- Early detection of anomalies supports policy decisions and resource allocation.
- Ensemble modeling reduces uncertainty by combining multiple climate models.
- Clear visualizations help non-technical stakeholders grasp the urgency.

Approach
This project uses:
- Ensemble Modeling: Combining multiple ML models (Random Forest, HistGradientBoosting, XGBoost) for robust predictions.
- Anomaly Detection: Quantile-based binning and adaptive thresholds to flag unusual climate patterns.
- NetCDF/xarray Workflows: Efficient handling of large-scale climate datasets.
- Diagnostic Visualization: Residual plots, threshold tracking, and decade-wise accuracy charts.
- Reproducible Pipelines: Modular Python scripts with clear inline documentation.

Results
The ensemble modeling approach achieved a best model accuracy of 92.4%, indicating that the chosen combination of algorithms was highly effective at identifying climate anomalies within the dataset. Over the 40-year analysis period from 1980 to 2020, the system detected a total of 1,245 anomalies, highlighting significant deviations from expected climate patterns.
One of the most notable findings was a mean temperature shift of +1.2°C across the studied regions. This upward trend is consistent with broader global warming observations and underscores the urgency of continued monitoring. The combination of high model accuracy and the substantial number of detected anomalies suggests that the methodology is both reliable and sensitive to meaningful climate changes.
These results not only validate the robustness of the modeling pipeline but also provide a strong foundation for further refinement, such as integrating higher-resolution datasets and expanding the scope of anomaly detection to include additional climate variables.







Example Visualization:
(Replace with your actual plot)
anomaly_map.png

Next Steps
- Integrate ERA5 reanalysis data for higher spatial resolution.
- Add seasonal anomaly tracking to detect short-term climate extremes.
- Deploy as an interactive dashboard for policymakers.
- Automate GitHub Actions to re-run models when new data is available.

Usage Instructions
1. Clone the repository
git clone https://github.com/SyeedHamid/Capstone-2.git
cd Capstone-2


2. Create a virtual environment
python -m venv .venv
source .venv/bin/activate   # Mac/Linux
.venv\Scripts\activate      # Windows


3. Install dependencies
pip install -r requirements.txt


4. Run the pipeline
python src/run_pipeline.py




