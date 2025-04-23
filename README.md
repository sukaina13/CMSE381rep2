# CMSE381rep2


Sukaina and Sherry Projects

The data: The Freiwald Tsao Face View AM dataset

Can we classify the face identity seen by the subject using neuron activity?

Classification Task: Classification Goal: Predict which of the 25 face identities was seen based on neuron activity recorded during each trial. Data Representation: Each row in the dataset represents neural activity recorded during a trial. Features: Spiking activity (binary values of 0 or 1) over time. Label: Face identity (one of 25 individuals). Models to Try: Logistic Regression (baseline model) k-Nearest Neighbors (KNN) Support Vector Machines (SVM) Random Forests Multi-layer Perceptron (MLP) / Deep Learning (if enough data is available)


 Dataset Description

The Freiwald Tsao Face Views AM dataset contains neural recordings from the anterior medial (AM) face patch—a region of the macaque brain that becomes active when viewing faces.

 Data Overview
Neural Activity: Spike train data recorded at 1 ms resolution across 800 ms trials.
Stimuli: 25 unique face identities, each shown from 8 head orientations.
Purpose: Decode face identity and head orientation using neural activity.
🔖 Key Columns
site_info.monkey: Monkey subject ID (e.g., "lupo")
site_info.region: Brain region ("am" = anterior medial face patch)
labels.stimID: Stimulus identifier (face image ID)
labels.person: Person ID (face identity label)
labels.orientation: Head orientation (e.g., "front")
labels.orient_person_combo: Combined identity + orientation label
🔬 Neural Spike Data (802 columns)
time.1_2 to time.800_801: Binary indicators of neuron spike (1 = spike, 0 = no spike)
Each column represents a 1 ms time bin of activity for that trial.
 Prediction Task 2: Total Spike Count

Objective: Predict the total number of spikes across all neurons in a trial.
Input: Face identity + head orientation.
Goal: Understand how strongly each stimulus (person/orientation) activates the brain.
Insight: Some identities might consistently trigger stronger responses—could indicate recognition or salience.
