# CMSE381rep2

Sukaina and Sherry Projects

The data: The Freiwald Tsao Face View AM dataset
 
### Can we classify the face identity seen by the subject using neuron activity?
Classification 
Task: Classification
Goal: Predict which of the 25 face identities was seen based on neuron activity recorded during each trial.
Data Representation:
Each row in the dataset represents neural activity recorded during a trial.
Features: Spiking activity (binary values of 0 or 1) over time.
Label: Face identity (one of 25 individuals).
Models to Try:
Logistic Regression (baseline model)
k-Nearest Neighbors (KNN)
Support Vector Machines (SVM)
Random Forests
Multi-layer Perceptron (MLP) / Deep Learning (if enough data is available)

### Can we determine the head orientation based on neural responses?
Classification

### How accurately can different machine learning models decode facial perception?
Comparison and evaluation 

Dataset Description
The Freiwald Tsao Face Views AM dataset consists of neural recordings from the anterior medial (AM) face patch, a brain region activated when a macaque sees a face. The dataset includes:
Neural activity (spike train data) recorded at 1ms resolution during image presentation.
Face stimuli: 25 individuals presented from 8 different head orientations.
Labels:
Face Identity (labels.person)
Head Orientation (labels.orientation)
site_info.monkey: The monkey subject (e.g., "lupo").
site_info.region: The brain region (e.g., "am" = anterior medial face patch).
labels.stimID: The stimulus identifier (a face image ID).
labels.person: The person ID (who is in the image).
labels.orientation: Head orientation (e.g., "front").
labels.orient_person_combo: Combined label of person and orientation.
Spike Data Columns (802):
time.1_2 to time.800_801: Neuron spike activity over 800 ms (binary values: 1 = spike, 0 = no spike).
Each column represents a 1 ms time bin of recorded neural activity.

