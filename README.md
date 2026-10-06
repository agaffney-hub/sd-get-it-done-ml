# San Diego Get It Done Machine Learning Analysis

The [City of San Diego’s Get It Done application](https://www.sandiego.gov/get-it-done) allows residents to report
non-emergency issues such as potholes, graffiti, abandoned vehicles, and other problems that
require city attention. This project applies supervised and unsupervised machine learning to approximately 375,000 closed 2025 service requests from the City of San Diego's Get It Done program.

**Can machine learning predict and classify how long a Get It Done service request will take to resolve based on factors such as request type, location, and submission timing?**

## Models

**Linear Regression**
Predicts the number of days a request takes to resolve.

**Logistic Regression**
Classifies whether a request is resolved within 30 days or takes longer than 30 days.

**K-Means Clustering**
Groups requests based on shared characteristics to identify patterns within the data.

## Data

The project uses the City of San Diego's Get It Done Reports dataset, focusing on cases closed during 2025.

**Source:** [City of San Diego Open Data Portal](https://data.sandiego.gov/datasets/get-it-done-reports/)

The original dataset contains 378,669 records and 23 variables. The raw dataset is not included in this repository because it exceeds GitHub's file-size limit.

## Tools

* Python
* Pandas
* NumPy
* scikit-learn
* Matplotlib
* SciPy
* Google Colab
* GitHub

## Repository

Each model has its own folder containing the relevant notebooks, visualizations, and analysis.

<ul>
  <li>
    <strong>EDA</strong> — exploratory analysis and initial findings
<details>
  <summary><strong>Click here to see EDA analysis images</strong></summary>
  <table>
    <tr>
      <td><img src="EDA/box_plot_case_age_days.png" width="400" alt="Box Plot of Case Age Days"></td>
      <td><img src="EDA/box_plot_case_type.png" width="400" alt="Box Plot of Case Type"></td>
    </tr>
  </table>
  <img src="EDA/heatmap.png" width="1100" alt="Heatmap">
</details>
  </li>

  <li>
    <strong>Linear Regression</strong> — continuous prediction of resolution time
<details>
  <summary><strong>Click here to see Linear Regression analysis images</strong></summary>
  <table>
    <tr>
      <td><img src="Linear_Regression/residuals_vs_predicted.png" width="400" alt="Residuals vs Predicted"></td>
      <td><img src="Linear_Regression/qq_plot_residuals.png" width="400" alt="Q-Q Plot of Residuals"></td>
    </tr>
  </table>
  <img src="Linear_Regression/linear_regression_model_comparison.png" width="1100" alt="Model Performance">
    <table>
    <tr>
      <td><img src="Linear_Regression/linear_regression_r2_comparison.png" width="400" alt="Residuals vs Predicted"></td>
      <td><img src="Linear_Regression/linear_regression_rmse_comparison.png" width="400" alt="Q-Q Plot of Residuals"></td>
    </tr>
  </table>
</details>
  </li>

  <li>
    <strong>Logistic Regression</strong> — classification of 30-day resolution
<details>
  <summary><strong>Click here to see Logistic Regression analysis images</strong></summary>
  <table>
    <tr>
      <td><img src="Logistic_Regression/f1_score_by_resolution_group.png" width="400" alt="F1 Score by Resolution Group"></td>
      <td><img src="Logistic_Regression/logistic_regression_confusion_matrix.png" width="400" alt="Confusion Matrix"></td>
    </tr>
  </table>
  <img src="Logistic_Regression/logistic_regression_model_comparison.png" width="1100" alt="Model Comparison">
  <img src="Logistic_Regression/logistic_regression_model_performance.png" width="1100" alt="Model Performance">
</details>
  </li>
  
  <li>
    <strong>K-Means</strong> — unsupervised clustering of service requests
<details>
  <summary><strong>Click here to see K-Means analysis images</strong></summary>
  <img src="K-Means_Clustering/choosing_k_figures.png" width="1100" alt="Choosing K Figures">
  <table>
    <tr>
      <td><img src="K-Means_Clustering/clusters_projected_to_2_components.png" width="400" alt="Clusters Projected to Two Components"></td>
      <td><img src="K-Means_Clustering/council_district_mix_by_cluster.png" width="400" alt="Council District Mix by Cluster"></td>
    </tr>
  </table>
  <img src="K-Means_Clustering/request_type_mix_by_cluster.png" width="1100" alt="Request Type Mix by Cluster">
  <img src="K-Means_Clustering/resolution_time_by_cluster.png" width="1100" alt="Resolution Time by Cluster">
</details>
  </li>
</ul>


## Team

Get It Done Crew
San Diego State University
