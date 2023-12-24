# <p align="center"> Investigating the Impact of Emotionally Charged Stimuli on Visual Imagery in EEG-based BCI Systems

## <p align="center"> Master’s Thesis submitted to the Department of Psychology and Computing,  Goldsmiths, University of London 2022-2023 </p>

**Supervisors**: Maria Herrojo Ruiz<sup>1</sup>, David Landi<sup>2</sup>, Giuseppe Lai<sup>1,3</sup>
1. Goldsmiths, University of London – Department of Psychology – London (UK)
2. LiquidWeb s.r.l. – R&D Officer and Co-founder – Siena (IT)
3. LiquidWeb s.r.l. – Siena (IT)


## Table of Contents

1. [Introduction](#introduction)
2. [Literature Review](#literature-review)
3. [Methods and Materials](#methods-and-materials)
4. [Results](#results)
5. [Discussion](#discussion)

# 1. Introduction <a name="introduction"></a>

Individuals with severe movement disorders, such as paralysis, locked-in syndrome (LIS), or amyotrophic lateral sclerosis (ALS) require alternative methods for communication and control. LIS is a state where patients are unable to generate voluntary speech, limb, or facial movements, despite their mental awareness and alertness (Laureys et al., 2005). Existing augmentative communication methods necessitate some level of voluntary muscle function, making them unsuitable for those who are completely paralysed or have significant motor disabilities. These individuals need a communication channel that bypasses muscle-based pathways and allows them to communicate without relying on peripheral nerves and muscles.

Brain-Computer Interfaces (BCIs) have emerged as a groundbreaking technology facilitating direct communication between the human brain and computers, circumventing the need for conventional input methods. This innovation holds immense promise, particularly for individuals grappling with profound motor impairments like LIS, offering renewed avenues for mobility and communication. Among various BCI modalities, Motor Imagery-based BCIs (MI-BCIs), leveraging Electroencephalogram (EEG) signals for brainwave acquisition, have garnered significant attention due to the advantage of high temporal resolution without necessitating invasive procedures. This has translated into diverse applications, from steering wheelchairs to manipulating robotic limbs, profoundly enhancing user-environment interaction. Within this context, EEG signals used for BCI control are susceptible to a myriad of influences, including the user's emotional state and levels of fatigue. These dynamic variations in EEG dynamics consequently impinge upon the efficacy of feature extraction within the BCI framework.

<p align="center">
  <img src="https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/raw/main/Plots%20and%20Diagrams/BCI.png" alt="Figure 2.1. Overview of Non-invasive EEG-based BCI system">
</p>

Given these complexities, the investigation of emotional stimuli's impact on visual imagery within EEG-based BCI systems becomes a matter of significance. This research endeavour aligns seamlessly with the pursuit of further enhancing the performance, reliability, and adaptability of BCIs. Through meticulous examination, we aspire to unravel the intricate interplay between emotional stimuli and neural patterns to bolster the robustness of EEG-based BCI applications. 

### **1.1 Thesis Structure**

The thesis commences by providing an introductory overview of the BCI framework, with a specific focus on BCIs utilizing EEG signals. Within this context, the role of emotions in EEG-based BCIs is elucidated. Subsequently, the following chapters are meticulously structured: Chapter Two undertakes a comprehensive review of pertinent literature and Chapter Three expounds upon the materials and methods employed throughout the study. In continuation, Chapter Four undertakes a meticulous presentation of the results obtained. The final chapter, Chapter Five, provides a comprehensive and insightful discussion that delves into the interpretation of the findings in the context of existing literature. 

### **1.2 Summary**
This study delves into the realm of BCIs, specifically focusing on Visual Imagery-based BCIs (VI-BCIs) that utilise EEG signals. The volatile nature of EEG signals, influenced by emotional states and other factors, poses challenges for their effective utilisation in BCIs. This research aims to explore the impact of emotional stimuli on EEG patterns in the context of VI-BCIs, with the ultimate goal of enhancing the reliability and performance of these systems. By uncovering how emotions impact individuals' ability to perform tasks, this study aspires to contribute to the advancement of EEG-based BCI applications, thus empowering those with motor impairments to interact more effectively. 


# 2. Literature Review <a name="literature-review"></a>
### **2.1 BCI Framework**

- **Introduction to BCI Systems:**
    - Facilitate communication and control through brain electrical activity.
    - Bypass traditional pathways for individuals with motor impairments.
- **BCI Categories:**
    - Invasive BCIs with implanted electrodes for high resolution.
    - Non-invasive BCIs, like EEG, offer safer alternatives.
    - Challenges in signal quality for non-invasive BCIs.

### **2.2 EEG-based BCIs**

- **EEG Overview:**
    - Non-invasiveness, real-time capabilities, and affordability.
    - Application in cursor movement, hand grasp control, and robotic tasks.
- **Challenges:**
    - Noisy signals, limited spatial resolution, and data processing difficulties.

### **2.3 Neural Markers for Brain Activity**

- **Evoked and Spontaneous BCIs:**
    - Evoked BCIs use external stimuli-triggered responses.
    - Spontaneous BCIs tap into inherent brain activity patterns.
- **Sensorimotor Rhythm (SMR)-based BCIs:**
    - Utilize motor imagery (MI) and visual imagery (VI).
    - ERD and ERS patterns in the alpha and beta frequency bands.

### **2.4 Emotions and BCI**

### 2.4.1 Role of Emotions in Cognition

- **Fundamental Role:**
    - Influence on learning, memory, perception, attention, reasoning, and problem-solving.

### 2.4.2 Emotions and EEG

- **EEG and Emotional States:**
    - Links between emotional states and EEG patterns.
    - Insights into neural underpinnings of human emotions.

### 2.4.3 Emotion Recognition in EEG-Based BCI

- **Challenges:**
    - Variability in subjective experiences.
    - Taxonomy models: Discrete Model and Dimensional Model.

### **2.5 Rational and Objective**

- **Influence of Emotions:**
    - On cognitive functions: attention, perception, memory, and decision-making.
    - Impact on VI tasks in EEG-based BCI systems.

### **2.6 Hypothesis**

- **Primary Hypothesis:**
    - Emotional stimuli impact neural mechanisms in VI tasks.
- **Two-Tailed Hypothesis:**
    - Predicts different effects of emotional stimuli on VI performance.

# 3. Methods and Materials <a name="methods-and-materials"></a>
### 3.1 Participants

- **Study Participants:**
    - 12 healthy volunteers (8 females, 4 males).
    - Inclusion criteria: Age 18-40, right-handed.
    - Exclusions: Neurophysiological conditions affecting EEG, aversions to snakes/spiders, or prior similar task experience.

### 3.2 Materials and Stimuli

- **Visual Imagery Paradigm:**
    - Braincontrol's VI tasks: Relax and Push.
    - Relax: Imagine a stationary object.
    - Push: Imagine pushing the object into space, visualized with illustration.
- **GAPED Dataset:**
    - 730 emotionally charged stimuli images (positive, negative, neutral) from GAPED.
    - Specific focus on negative images of snakes and spiders.
- **EEG System:**
    - 64-channel Biosemi ActiveTwo system.
    - Electrode placement based on the 10-20 system, digitized at 512 Hz.
    - Mastoids as reference channels, impedance levels below 30 kΩ.

### 3.3 Experimental Design

- **VI Experimental Paradigm:**
    - 12-second trials: fixation (2s), emotionally charged stimuli presentation (4s), VI condition (4s), and final fixation.
    - Inter-trial interval: 250 milliseconds.
    - Counterbalanced block order, randomized relax/push tasks.
- **Within-Subjects Design:**
    - Six blocks, 33 trials/block, two blocks per emotional stimulus.

### 3.4 EEG Preprocessing

- **Signal Processing:**
    - Notch filter at 50 Hz, bandpass filter (1-40 Hz) for signal preservation.
    - Event-related epochs extracted for further analysis.
    - Bad channel handling, robust average referencing, and noise removal.
    - Independent Component Analysis (ICA) for artifact identification.

### 3.5 Data Analysis

- **Time-Frequency Analysis (CWT):**
    - Continuous Wavelet Transform for time-frequency analysis.
- **Cluster-Based Permutation Tests:**
    - Non-parametric method for event-related EEG data analysis.
    - Identifying significant differences between conditions across subjects.

### 3.6 Feature Extraction

- **PCA-Based Approach:**
    - Principal Component Analysis for feature extraction.
    - FD-PCA: Applied to complete datasets.
    - SD-PCA: Applied to channels and time points significant through CBPT.

### 3.7 ML Classifier

- **Classifiers Explored:**
    - Support Vector Machines (SVM), k-Nearest Neighbors (KNN), Random Forests.

### 3.8 Statistical Analysis and Decoding

- **Data Transformation:**
    - Resampling to 256 Hz, time-frequency decomposition using Morlet wavelet.
    - Baseline correction and averaging in alpha and beta frequency ranges.
- **Dimensionality Reduction:**
    - PCA for feature selection using FD-PCA and SD-PCA.
    - Criteria for component selection explained.
- **Hyperparameter Tuning:**
    - SVM, KNN, and Random Forest classifiers.
    - Grid search for optimal hyperparameters.
- **Performance Metrics:**
    - Accuracy, test accuracy, precision, recall, and F1-score.

# 4. Results <a name="results"></a>
### 4.1 Modulation of Neuronal Oscillations following Emotionally Charged Stimuli

- **Cluster-Based Permutation Analysis:**
    - Disparities in "relax" and "push" conditions post emotionally charged stimuli.
    - Positive stimuli: Significant alpha and beta oscillations (1.5 to 2.5 seconds, p = 0.004).
    - Negative stimuli: Significant oscillations (1.2 to 2 seconds, p = 0.03) and (1.2 to 3 seconds, p = 0.002).
    - No significant negative clusters for any emotional stimuli.
- **Visualization:**
    - Following Figures illustrates alpha and beta oscillation patterns, with significant time points.
 
<p align="center">
  <img src="https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/raw/main/Plots%20and%20Diagrams/Negative_plot.svg" alt="Push vs. Relax during Negative Emotional Stimuli" title="Push vs. Relax during Negative Emotional Stimuli">
</p>

<p align="center">
  <img src="https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/raw/main/Plots%20and%20Diagrams/Neutral_plot.svg" alt="Push vs. Relax during Neutral Emotional Stimuli" title="Push vs. Relax during Neutral Emotional Stimuli">
</p>

<p align="center">
  <img src="https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/raw/main/Plots%20and%20Diagrams/Positive_plot.svg" alt="Push vs. Relax during Positive Emotional Stimuli" title="Push vs. Relax during Positive Emotional Stimuli">
</p>

### 4.2 Classification Performance and Results

### **4.2.1 PCA**

- **Explained Variance:**
    - FD-PCA: First principal component substantial variance (0.8461 relax, 0.5321 push).
    - SD-PCA: Dominant first principal component (0.3592 relax, 0.2165 push).

<p align="center">
<img src = "https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/blob/main/Plots%20and%20Diagrams/PCA.png">
</p>

### **4.2.2 Grid Search and Cross-Validation**

- **Hyperparameter Tuning:**
    - Optimal parameters (C=1, k=3, n_estimators=50) for SVM, KNN, and Random Forest.
    - Overfitting observed in Random Forest learning curve (Figure 4.3).

<p align="center">
<img src = "https://github.com/osheenjain/Investigating-the-Impact-of-Emotionally-Charged-Stimuli-on-Visual-Imagery-in-EEG-based-BCI-Systems/blob/main/Plots%20and%20Diagrams/Learning%20Curve%20Graphs%20Depicting%20the%20Performance%20of%20SVM%2C%20KNN%2C%20and%20Random%20Forest%20Classifiers%20concerning%20Positively%20Charged%20Stimuli.jpeg">
</p>

- **Performance Metrics:**
    - Table 5 (SM1) displays precision, recall, and f1-score for relax and push across classifiers.
    - KNN stands out as the most robust performer.
- **Classification Results:**
    - KNN Accuracy:
        - "Relax" emotion: 94.56%, precision 93.09%, recall 92.96% (FD-PCA).
        - "Push" emotion: 94.56%, precision 96.12%, recall 92.96% (FD-PCA).
    - KNN consistently strong across emotional categories and PCA methods.
- **Emotional Stimuli Impact:**
    - KNN excels under positive emotional stimuli, slight decrease in accuracy, precision, and recall under negative and neutral stimuli for "relax" vs "push."
- **Model Interpretation:**
    - KNN model effectiveness suggests emotions influence the ability to perform "relax" vs "push" motion in EEG data.

### **Summary Points**

- Emotionally charged stimuli induce significant alpha and beta oscillation differences in "relax" vs "push."
- FD-PCA and SD-PCA capture essential data variability with different emphasis.
- KNN emerges as the most robust classifier, demonstrating high accuracy, precision, and recall.
- Model performance varies under different emotional stimuli, with positive stimuli yielding the best results.
- Emotions play a role in classifying "relax" vs "push" motions in EEG data.

# 5. Discussion <a name="discussion"></a>

- **Hypothesis Confirmation:**
    - Significant changes in alpha and beta bands during VI tasks post emotionally charged stimuli.
    - Alpha power suppression during "push" task across emotional states.
    - Distinct beta patterns for positive stimuli, questioning emotional valence's influence on neural synchronization timing.
- **Machine Learning Classification:**
    - SVM, KNN, and Random Forest used for classification.
    - KNN consistently outperforms, showing higher accuracy, precision, and recall.
    - Random Forest exhibits promising accuracy but raises overfitting concerns.
- **Emotional Impact on VI Tasks:**
    - Small performance increase under positive emotional stimuli for KNN.
    - Suggests emotions influence VI tasks, calls for further investigation with a larger participant pool.
    - Acknowledges cautious interpretation of observed impact size.
- **Implications for BCI Design:**
    - Understanding emotions' link to EEG signals could revolutionize BCI design.
    - Real-time adaptation to users' emotional states may enhance BCI effectiveness.
    - KNN's consistent performance suggests its potential for robust and reliable BCI systems.
- **Limitations and Future Directions:**
    - Constrained emotional stimuli dataset and absence of a broader emotional spectrum acknowledged.
    - Challenges related to spatial resolution in EEG analyses and static nature of stimuli addressed.
    - Future research should explore dynamic stimuli, real-life scenarios, and advanced ML methods.
- **Conclusion:**
    - Contributes to understanding emotional stimuli impact on EEG-based BCIs, particularly VI tasks.
    - Theoretical insights combined with empirical findings offer implications for BCI design.
    - KNN's consistent performance implies potential for enhanced user experiences.
    - Strategic opportunities for companies like LiquidWeb to capitalize on emotional dimensions in BCI interactions.



