# EE200: Signals, Systems and Networks – Practical Project

This repository contains my solution to the EE200 (Signals, Systems and Networks) practical assignment under the guidance of **Dr. Tushar Sandhan** at **IIT Kanpur**.

The project explores frequency-domain signal processing techniques on both images and audio signals using Python, Fourier analysis, spectral filtering, and system design concepts.

## Project Structure

```text
EE200-Frequency-Domain-Signal-Processing/
│
├── README.md                    ← Main repo overview
│
├── ProblemStatement/
│   ├── README.md                ← Assignment description
│   ├── Basic_image_audio_tut.ipynb
│   ├── cat_gray.jpg
│   ├── dog_gray.jpg
│   └── song_with_2piccolo.wav
│
└── Solution/
    ├── README.md                ← Your approach & results
    ├── EE200_Practical_Report_240500.pdf
    ├── Q1_Frequency_Mixer.ipynb
    ├── Q2_Frequency_Demixer.ipynb
    └── sound file.wav
```

## Part 1: Frequency Mixer – Beauty and the Blur

This section investigates image processing in the frequency domain using the 2D Fourier Transform.

### Objectives

* Compute and visualize 2D FFT spectra of grayscale images.
* Analyze magnitude and logarithmic (dB) spectra.
* Verify Fourier rotation properties by rotating images and comparing spectra.
* Design low-pass and high-pass frequency masks.
* Create a hybrid image by combining:

  * Low-frequency structure from one image.
  * High-frequency details from another image.

### Concepts Used

* 2D Discrete Fourier Transform (DFT)
* FFT Shift
* Magnitude and Phase Spectra
* Spatial-Frequency Analysis
* Frequency-Domain Image Fusion
* Gaussian Low-Pass and High-Pass Filters

### Results

The final hybrid image combines the global appearance of one image with the fine details of another, demonstrating how different spatial frequencies contribute to visual perception.

---

## Part 2: Frequency De-Mixer – Unwanted Solo

This section focuses on removing an unwanted musical instrument from a mixed audio recording using frequency-domain analysis and filtering.

### Objectives

* Load and preprocess audio signals.
* Analyze frequency content using FFT.
* Estimate Power Spectral Density (PSD) using Welch's Method.
* Detect dominant interference frequencies.
* Design a Butterworth Band-Stop (Notch) Filter.
* Validate filter performance using:

  * Bode Plots
  * Pole-Zero Analysis
* Remove the unwanted frequency components while preserving the original music.

### Concepts Used

* Fast Fourier Transform (FFT)
* Power Spectral Density (PSD)
* Peak Detection
* Butterworth Filters
* Band-Stop Filtering
* Pole-Zero Plots
* Bode Analysis
* Zero-Phase Filtering (filtfilt)

### Results

The corrupted audio signal was analyzed, unwanted spectral components were identified, and a frequency-selective filter was designed to suppress them. The cleaned audio was then exported while preserving the original musical content.

---

## Tools and Libraries

* Python
* NumPy
* SciPy
* Matplotlib
* PIL (Pillow)
* Librosa
* SoundFile

## Key Learning Outcomes

* Fourier Transform based signal analysis
* Frequency-domain image manipulation
* Hybrid image generation
* Spectral analysis of audio signals
* PSD estimation and peak detection
* Digital filter design and validation
* Practical applications of signals and systems concepts

```
```
