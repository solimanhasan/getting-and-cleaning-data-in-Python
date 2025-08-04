# CodeBook for the Human Activity Recognition Dataset – Tidy Version

## 📄 Dataset Source

The data was collected from the [UCI HAR Dataset](https://archive.ics.uci.edu/ml/datasets/human+activity+recognition+using+smartphones).

## ✨ Transformations Made

1. Merged the training and the test sets.
2. Labeled the dataset with descriptive variable names using `features.txt`.
3. Extracted measurements on the mean and standard deviation using regex.
4. Replaced activity numbers with activity names using `activity_labels.txt`.
5. Created a second, tidy dataset with the average of each variable for each activity and each subject.

## 🔢 Variables

The tidy dataset contains:
- `Subject`: ID of the person (1–30)
- `Activity`: Name of the activity performed (e.g., WALKING, SITTING)
- **561 feature columns** from accelerometer and gyroscope signals, focusing on:
  - Mean (`mean()`)
  - Standard Deviation (`std()`)

Each row represents the average of each variable for each activity and each subject.
