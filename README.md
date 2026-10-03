# 🚗 Vehicle Predictive Maintenance

Machine learning models built to predict the remaining kilometers of a vehicle based on sensor metrics and vehicle telemetry.

* **The Problem:** Unpredictable failures cause high maintenance costs, which, in turn, impact customer satisfaction.
* **The Solution:** Machine learning algorithms make use of available sensor data to predict when a problem will emerge, thereby reducing future maintenance costs.

## TOOLS

* **programming language and data analysis:** Python, Pandas, Seaborn, matplotlib
* **machine learn and validation:** Scikit-learn, LightGBM, Keras


---

## DATASET
* **link:** https://www.kaggle.com/datasets/lalit7881/car-sensor-dataset
* **target variable:** Remaining kilometers


## FEATURE ENGINEERING

* the model contains a lot of categorical data, some of them are ordinal (such Tire_Condition	Vibration_Level) and others nominal (like Vehicle_Type). they are treated in a diffent way
* it also have KM_Range_Before_Defect, a feature tha contains intervals, each interval was replaced by the mean of interval

  
## RESULTS AND IMPACTS
* **MAE (mean absolute erro):** 5690.80 km, which means that the model is, on the average, 5690.80 km away from the real prediction.
it is not too far if we notice that the mean of remaining kilometers is 54116.43, although the standard deviation is high.


### LIMITATION AND FUTURE WORK
---
* **Dataset Constraints:** The current dataset is synthetic/limited and may not fully reflect real-world vehicle telemetry behavior.
* **Next Steps:** With access to domain-specific vehicle sensor specs and real-time operational logs, further hyperparameter tuning and feature extraction can significantly reduce prediction error.
