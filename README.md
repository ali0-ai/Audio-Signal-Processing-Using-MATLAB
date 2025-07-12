# 🎧 Audio Signal Processing Using MATLAB

This project demonstrates a basic example of **noise removal from an audio signal** using **MATLAB**. It focuses on detecting and removing unwanted frequency components from a voice recording using digital filters.

---

## 📌 Project Objectives

1. Detect and calculate interference signal frequencies (**f₁** and **f₂**)
2. Compute Signal-to-Interference Ratio (**SIR or S/J**) in decibels
3. Apply filtering to suppress interference
4. Display time-domain and frequency-domain plots
5. Play and save the processed audio

---

## 📊 Step-by-Step Overview

### 1. 📥 Load and Analyze the Original Signal

```matlab
[f, Fs] = audioread('handel_J.wav');
T = 1 / Fs;
L = length(f);
t = (0:L-1) * T;
