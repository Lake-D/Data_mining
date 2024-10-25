Analyze the Relationship Between Amplitude and Coke Discharge Volume, and Design and Train a Model to Predict Amplitude

1.Data Selection and Cleaning:
Select appropriate data, check for outliers or noise, and perform suitable cleaning.

2.Exploring the Relationship Between Amplitude and Coke Discharge Volume:
Analyze the relationship between amplitude GXJ_ZDGLQ_GD and coke discharge volumes GXJ_A045 (Belt 1) and GXJ_A046 (Belt 2).

3.Model Selection:
Choose an appropriate model to predict amplitude GXJ_ZDGLQ_GD.

5.Model Training:
Based on the belt status (BMC102_A006 and BMC102_A007), select the corresponding belt's coke discharge volume (GXJ_A045 or GXJ_A046) as the feature, with GXJ_ZDGLQ_GD as the target variable, and train separate models for each belt.

Use the data from "Attachment 1.csv" as the training data.

Model Prediction:
In the test dataset "Attachment 2.csv", there are five segments where the amplitude values are zero (details in Note 3). Predict the amplitude for these segments and update the file accordingly.

Submit Code, Documentation, and Updated "Attachment 2.csv":
Ensure that the training and prediction code can be rerun reliably.

Field Descriptions:

Variable Name	Variable Description
timestamp	Timestamp
GXJ_A045	Coke discharge volume for Belt 1
GXJ_A046	Coke discharge volume for Belt 2
BMC102_A006	0/1 variable; 0 indicates Belt 1 is unused, 1 indicates Belt 1 is in use
BMC102_A007	0/1 variable; 0 indicates Belt 2 is unused, 1 indicates Belt 2 is in use
GXJ_ZDGLQ_GD	Amplitude

Notes:

Attachment 1 contains data for 40 days, and Attachment 2 contains data for 20 days. The time periods of the two datasets are consecutive.

Belts 1 and 2 are used at different times and are never in use simultaneously.

The coke discharge volume should be between 110 and 200.

The timestamps in Attachment 2 where amplitude predictions are required (i.e., where amplitude = 0) are as follows:

2024-08-23 15:00:00 – 2024-08-23 18:00:00
2024-08-27 18:00:00 – 2024-08-27 21:00:00
2024-09-02 09:00:00 – 2024-09-02 12:00:00
2024-09-07 09:00:00 – 2024-09-07 12:00:00
2024-09-12 00:00:00 – 2024-09-12 03:00:00
