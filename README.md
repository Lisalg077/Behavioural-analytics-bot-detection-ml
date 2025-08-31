# Behavioural-analytics-bot-detection-ml
ML-based analysis of web server logs for bot detection
## Overview
This project analyses server logs to detect non-human (bot) traffic impacting a music media startup. The analysis identifies suspicious patterns and recommends strategies to mitigate traffic overload.

## Dataset
- Server logs in `data/server_logs.txt`.
- Sample log file format: timestamps, IP addresses, request paths, user agents, etc.
- **Note:** This dataset is small enough to include, but sensitive logs should not be publicly shared.

## Skills & Tools
- Python, Pandas, NumPy
- Scikit-learn (Random Forest Classifier)
- Matplotlib, Seaborn (visualisations)
- Jupyter Notebook
- Optional: Docker (for containerised execution)

## Approach
1. Load and parse logs into a structured format.
2. Explore traffic patterns : requests per IP, requests per hour.
3. Feature engineering : number of requests, unique endpoints, unique user agents per IP.
4. Label potential bots based on traffic heuristics (top 5% by request count).
5. Train a machine learning model to classify bots vs humans.
6. Evaluate model performance and visualize results.
7. Optional: Save predictions for further analysis.

## Results
- Detected high-frequency IPs and unusual traffic patterns
- Built a classifier achieving [insert metrics, e.g., accuracy] on labelled data
- Trained a Random Forest model with high accuracy in distinguishing bot vs Human IPs.
- Visualised traffic trends and feature importnace to explain the model 

## Usage
1. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/Behavioural-Bot-Detection-ML.git
