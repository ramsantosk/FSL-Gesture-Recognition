# Filipino Sign Language Hand Landmark Dataset

## Overview

This directory contains sample hand landmark data collected during the development of the **Filipino Sign Language Gesture Recognition System**, an academic research project focused on recognizing selected Filipino Sign Language gestures through computer vision and machine learning.

The dataset was collected by the research team using MediaPipe Hand Landmarker functionality and was used to support the development of a gesture classification model.

## Data Collection

Hand gesture samples were collected using a camera and MediaPipe hand tracking.

For each detected hand, the system extracted 21 hand landmarks, with three coordinate values per landmark:

- **X:** Horizontal position
- **Y:** Vertical position
- **Z:** Relative depth coordinate

Each recorded sample contains 63 numerical features (21 landmarks × 3 coordinates).


## Dataset Format

The `landmarks/` directory contains 38 CSV files representing 19 selected Filipino Sign Language alphabet gesture classes.

Each gesture class includes separate landmark recordings for the left and right hands.

### Dataset Organization

- **19 alphabet gesture classes**
- **38 CSV files** (19 left-hand and 19 right-hand files)
- **760 recorded hand landmark samples**
- **63 numerical features per sample**

The supported alphabet classes are:

A, B, D, E, G, H, I, K, L, M, N, O, P, R, S, T, U, W, Y.

The dataset does not cover the complete A–Z alphabet.

### Naming Convention

| Example File | Description |
|---|---|
| `A_L.csv` | Left-hand gesture samples for letter A |
| `A_R.csv` | Right-hand gesture samples for letter A |
| `B_L.csv` | Left-hand gesture samples for letter B |
| `B_R.csv` | Right-hand gesture samples for letter B |

### Hand Landmark Features

Each recorded sample contains 63 numerical values representing 21 detected hand landmarks.

Each landmark contains three coordinates:

- X — Horizontal position
- Y — Vertical position
- Z — Relative depth

The coordinates are stored in a flattened numerical format.

### Public Dataset Contents

The `landmarks/` directory contains the recovered alphabet gesture dataset.

The `samples/` directory provides a smaller example containing five records from `A_L.csv`.

These files demonstrate the hand landmark data representation used during the development and training of the gesture classification system.


## Machine Learning Application

The original dataset supported the development of a gesture classification system using a Random Forest classifier implemented with Scikit-learn.

The trained classifier was integrated into a Python application that uses OpenCV and MediaPipe for real-time hand detection and gesture recognition.


## Data Availability

The recovered alphabet hand landmark dataset is included in this repository for academic reference and technical documentation.

The dataset contains:

- 38 CSV files representing 19 selected Filipino Sign Language alphabet gesture classes.
- Separate left-hand and right-hand recordings for each supported letter.
- 760 recorded hand landmark samples.
- 63 numerical features per sample, representing 21 hand landmarks.

The `landmarks/` directory contains the recovered alphabet training dataset, while the `samples/` directory provides a smaller example for easier inspection.

The repository also includes the trained gesture classification model (`gesture_model.pkl`) and the developer's original prerecorded audio files in the `voices/` directory.

The complete application source code and other development scripts are not publicly distributed.

For academic, research, or professional inquiries, access to the full implementation may be requested from the project developer, subject to approval.

The provided materials document the original research and development process and do not represent comprehensive Filipino Sign Language recognition.


## Research Context

This dataset was collected as part of the research project:

**Bridging the Communication Gap: Developing a Real-Time System for Translating Basic Filipino Sign Language Gestures into Text-to-Speech**

The project was developed for academic research and is not intended to represent comprehensive Filipino Sign Language recognition.