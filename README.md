# Filipino Sign Language Gesture Recognition System

**A Real-Time Computer Vision and Machine Learning Research Project**

Developed as part of the research:

*Bridging the Communication Gap: Developing a Real-Time System for Translating Basic Filipino Sign Language Gestures into Text-to-Speech*

A Raspberry Pi-based research prototype designed to recognize selected Filipino Sign Language hand gestures and translate them into readable text and prerecorded Tagalog speech.

**Research Recognition:** Best in Research Paper

## Project Overview

This project explores how computer vision and machine learning can support communication between Filipino Sign Language users and individuals unfamiliar with basic sign language gestures.

The system processes live camera input, detects hand landmarks, and identifies supported gestures through a trained classification model and motion-based recognition logic.

Recognized gestures are displayed on the application's interface, with corresponding prerecorded speech played when audio is enabled.

The project was developed as an academic research prototype and does not provide comprehensive Filipino Sign Language translation.

## My Contributions

**Role: Lead Software Developer**

My development responsibilities included:

- Developing and integrating the real-time gesture recognition application using Python.
- Implementing camera processing and hand landmark detection with OpenCV and MediaPipe.
- Integrating a trained machine learning classifier for recognizing selected alphabet gestures.
- Implementing movement-based detection for selected dynamic gestures.
- Developing the graphical interface using Tkinter.
- Implementing Alphabet Mode and Motion Mode switching.
- Integrating offline Tagalog speech playback using personally recorded audio.
- Configuring the application for use with Raspberry Pi 4 hardware.

The project was completed as part of a collaborative academic research effort.

## Technologies Used

| Technology | Application |
|---|---|
| Python | Application development |
| Raspberry Pi 4 | Hardware platform |
| OpenCV | Real-time camera processing |
| MediaPipe | Hand landmark detection |
| Scikit-learn | Random Forest gesture classification |
| NumPy | Landmark and motion calculations |
| Joblib | Trained classifier integration |
| Tkinter | Application interface |
| Pillow | Camera frame rendering |
| Pygame | Offline speech playback |

## How the System Works

**1. Camera Input**

A connected camera captures live video of the user's hand gestures.

**2. Hand Landmark Detection**

MediaPipe detects 21 hand landmarks, providing x, y, and z coordinates for each landmark.

**3. Gesture Recognition**

The application provides two recognition modes:

- **Alphabet Mode:** Uses landmark features and a trained Random Forest classifier to recognize supported static hand gestures.
- **Motion Mode:** Uses hand movement patterns and predefined rules to detect selected dynamic gestures.

**4. Text Output**

Recognized gestures are displayed through the graphical interface.

**5. Speech Output**

When speech is enabled, the application plays a matching prerecorded audio file when one is available.

### Selected Dynamic Gestures

| Gesture | Tagalog Output |
|---|---|
| HI | Kumusta |
| THANK YOU | Salamat |
| SORRY | Pasensiya |


## Training Dataset

The research team collected hand landmark data to support the development and training of the Filipino Sign Language gesture recognition model.

Using MediaPipe, each detected hand was represented by 21 landmarks, with X, Y, and Z coordinates recorded for each landmark.


### Python Dependencies

The `requirements.txt` file lists the main Python libraries used in the original gesture recognition application.

It is provided for technical reference. The complete application source code is not publicly included in this repository.

Package versions are not pinned, and compatibility with other operating systems or Python environments has not been independently verified.


### Dataset Overview

| Dataset Information | Details |
|---|---|
| Supported Alphabet Classes | 19 |
| Total CSV Files | 38 |
| Recorded Samples | 760 |
| Features per Sample | 63 |
| Hand Categories | Left and Right |
| File Format | CSV |

### Supported Alphabet Gestures

The dataset includes the following 19 alphabet classes:

**A, B, D, E, G, H, I, K, L, M, N, O, P, R, S, T, U, W, Y**

The dataset does not cover the complete A–Z alphabet.

### Dataset Organization

The `dataset/landmarks/` directory contains the recovered training data, organized into separate CSV files for left-hand and right-hand gestures.

The `dataset/samples/` directory contains a smaller example for easier inspection.

These landmark features were used to train a Random Forest classifier with Scikit-learn.

### Public Research Materials

This repository includes:

- The recovered alphabet hand landmark dataset.
- A trained gesture classification model (`gesture_model.pkl`).
- Original prerecorded Tagalog audio files (`voices/`).

The complete application source code remains private.

For additional technical information about the dataset, see the [Hand Landmark Dataset Documentation](dataset/README.md).



## Source Code Availability

This repository serves as a public showcase of the Filipino Sign Language Gesture Recognition System, developed as part of an academic research project.

The repository provides access to selected research and development materials, including:

- The recovered hand landmark training dataset.
- The trained gesture classification model.
- Original prerecorded Tagalog speech files.
- Documentation describing the system's development and recognition process.

The complete Python application source code and additional development scripts are not publicly distributed.

For academic, research, or professional inquiries, individuals interested in reviewing the full implementation may contact the project developer.

**Full implementation access may be provided upon request and approval**, subject to applicable research and contributor permissions.


## Project Limitations

- Recognizes only a limited set of supported gestures.
- Does not provide complete Filipino Sign Language interpretation.
- Dynamic gesture recognition relies on predefined motion rules.
- Recognition behavior can vary with camera conditions, hand positioning, and movement.
- The recovered application has not yet been independently revalidated in a new hardware environment.


## Contact

For project inquiries, research-related discussions, or requests to review the complete implementation, you may contact me through my developer portfolio.

**Developer Portfolio:** [Ram Kirsten Santos](https://ramkirstensantos.vercel.app)

Additional project materials may be provided upon request and approval.


*This repository documents an academic research prototype and selected development materials. It is not a complete application distribution.*