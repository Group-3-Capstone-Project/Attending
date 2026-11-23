# CNN-Based Student Attendance and Classroom Behaviour Analysis System

## 1. Project Overview

The **CNN-Based Student Attendance and Classroom Behaviour Analysis System** is a computer vision and deep learning project designed to automate student attendance monitoring and analyse classroom engagement using CCTV footage.

The system uses **Convolutional Neural Networks (CNNs)** and computer vision techniques to process classroom video footage, detect students, monitor their presence, and identify observable classroom behaviours.

Beyond traditional attendance tracking, the system aims to provide insights into student attentiveness and classroom participation by identifying behaviours such as:

- Attentive students.
- Sleeping or resting students.
- Students looking away or appearing distracted.
- Students raising their hands.
- Students displaying signs of disengagement.
- General classroom activity and participation.

The analysed information is transformed into statistical summaries and visual insights through an interactive dashboard, helping educators understand classroom engagement patterns and make more informed decisions.

## 2. Problem Statement

Traditional student attendance systems rely heavily on manual roll calls, which consume valuable instructional time and are susceptible to human error.

Furthermore, conventional attendance systems only establish whether a student is physically present. They do not provide information about classroom engagement, attentiveness, or observable behavioural patterns.

There is therefore a need for an intelligent monitoring system capable of combining automated attendance tracking with computer vision-based classroom behaviour analysis.

This project addresses that gap by leveraging CNN-based image analysis to extract meaningful information from CCTV footage and generate insights that can support classroom monitoring and educational decision-making.

## 3. Project Objectives

The primary objectives are:

1. **Automated Attendance Monitoring:** Detect students appearing in classroom CCTV footage and estimate attendance.
2. **Behavioural Classification:** Identify observable behaviours such as attentiveness, sleeping, distraction, and hand-raising.
3. **Classroom Engagement Analysis:** Estimate overall classroom engagement using detected behavioural patterns.
4. **Video Processing:** Extract and analyse selected frames from recorded CCTV footage.
5. **Insights Generation:** Generate statistical summaries highlighting attendance levels and classroom behavioural trends.
6. **Data Visualization:** Present analytical results through an interactive dashboard.

## 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| CNN | Image feature extraction and behavioural classification |
| TensorFlow / Keras or PyTorch | Deep learning model development |
| OpenCV | CCTV video processing and frame extraction |
| NumPy | Numerical computations |
| Pandas | Data processing and analysis |
| Matplotlib / Seaborn | Data visualization |
| Gradio | Interactive analysis interface |
| Google Colab | Model development and experimentation |

*The exact frameworks depend on the implementation used in the project.*

## 5. System Architecture

The system follows a computer vision-based processing pipeline.

```text
       CCTV VIDEO FOOTAGE
                |
                v
       VIDEO PREPROCESSING
                |
                v
        FRAME EXTRACTION
                |
                v
       STUDENT DETECTION
                |
                v
       CNN-BASED ANALYSIS
                |
         +------+------+
         |             |
         v             v
   ATTENDANCE      BEHAVIOUR
   MONITORING     CLASSIFICATION
         |             |
         v             v
   STUDENT          ATTENTIVE
   PRESENCE         SLEEPING
                    DISTRACTED
                    HAND RAISED
                    OTHER
         |             |
         +------+------+
                |
                v
        DATA AGGREGATION
                |
                v
        INSIGHTS GENERATION
                |
                v
        INTERACTIVE DASHBOARD
```

## 6. Key Features

### A. Automated Attendance Monitoring
- Processes classroom CCTV footage.
- Detects visible students across sampled video frames.
- Estimates the number of students present.
- Provides attendance-related statistical summaries.

### B. Student Behaviour Analysis

The system analyses visual patterns to identify different classroom behaviours.

| Behaviour | Description |
|---|---|
| Attentive | Student appears oriented towards the teaching area or learning activity |
| Sleeping | Student displays visual patterns associated with sleeping |
| Distracted | Student appears to be looking away from the learning activity |
| Hand Raised | Student raises a hand, potentially indicating participation |
| Disengaged | Student displays observable patterns associated with reduced engagement |

### C. Classroom Engagement Insights

The system aggregates detected behaviours to generate insights such as:

- Estimated classroom engagement levels.
- Distribution of detected behavioural categories.
- Frequency of sleeping or distracted behaviour.
- Student participation indicators.
- Changes in observed classroom behaviour over time.

### D. Interactive Dashboard

The dashboard presents the analysis in an accessible format, including:

- Total sampled frames.
- Estimated student headcount.
- Peak visible student count.
- Behavioural detection statistics.
- Engagement category distribution.
- Graphical representations of classroom activity.

## 7. Analytical Outputs

The system generates an analysis summary containing metrics such as:

| Metric | Description |
|---|---|
| Sampled Frames | Number of video frames analysed |
| Video Duration | Total duration of the CCTV footage |
| Estimated Headcount | Estimated number of visible students |
| Peak Headcount | Highest number of students detected in a sampled frame |
| Raised-Hand Detections | Number of detected hand-raising instances |
| Behaviour Detections | Number of successful behavioural classifications |
| Engagement Share | Estimated proportion of detections classified into engagement-related categories |

These metrics provide a quantitative overview of classroom activity.

## 8. Machine Learning Approach

The project uses Convolutional Neural Networks (CNNs), a deep learning architecture particularly effective in image recognition and visual pattern extraction.

CNNs learn spatial features from images through convolutional layers, pooling operations, and fully connected layers.

The extracted visual features can then be used to classify different classroom behaviours.

The general CNN workflow includes:

1. Input image acquisition.
2. Image resizing and preprocessing.
3. Feature extraction through convolutional layers.
4. Dimensionality reduction through pooling.
5. Behaviour classification.
6. Prediction and confidence scoring.

The quality of the predictions depends on the training dataset, model architecture, image quality, and classification thresholds.

## 9. Expected Benefits

- Reduces the time required for manual attendance monitoring.
- Provides additional information beyond physical attendance.
- Helps educators identify potential classroom engagement challenges.
- Supports data-driven educational decision-making.
- Provides measurable classroom activity indicators.
- Demonstrates the practical application of deep learning and computer vision in education.

## 10. Limitations and Ethical Considerations

The system is intended to support classroom monitoring rather than replace human judgment.

Some important considerations include:

- A student looking away does not necessarily mean they are distracted.
- Head position alone cannot conclusively establish whether someone is sleeping.
- Occlusion, poor lighting, camera positioning, and video quality can affect detection accuracy.
- Headcount estimates across frames should not automatically be treated as unique student attendance records.
- Behavioural classifications are estimates and should not be interpreted as definitive assessments of student attention.
- CCTV footage must be processed in accordance with applicable privacy and data protection requirements.
- Appropriate consent, access controls, secure storage, and retention policies should be implemented.

## 11. Future Improvements

Potential improvements include:

1. **Face Recognition Integration:** Introduce privacy-compliant student identification for individual attendance tracking.
2. **Real-Time Monitoring:** Extend the system to analyse live CCTV streams.
3. **Object Detection:** Integrate YOLO or similar architectures to improve student detection.
4. **Temporal Behaviour Analysis:** Use LSTM or other temporal models to analyse behavioural changes across consecutive frames.
5. **Improved Classification:** Expand the behavioural dataset to improve classification accuracy.
6. **Historical Analytics:** Track classroom engagement trends across lessons and academic periods.
7. **Automated Reporting:** Generate downloadable classroom performance and attendance reports.

## 12. Project Conclusion

This project demonstrates how deep learning and computer vision can be applied to educational environments to automate attendance monitoring and provide insights into classroom behaviour.

By combining CNN-based visual analysis, video processing, behavioural classification, and interactive data visualization, the system provides an intelligent approach to understanding classroom activity.

Ultimately, the project aims to move beyond traditional attendance systems towards more informative, data-driven classroom monitoring solutions.

---

**Project Category:** Artificial Intelligence | Deep Learning | Computer Vision | Educational Technology

**Core Model:** Convolutional Neural Network (CNN)

**Application:** Automated Student Attendance and Classroom Behaviour Analysis
