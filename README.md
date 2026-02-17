# Object-Detection-in-Adverse-Weather-Conditions-for-Autonomous-Vehicles
Submitted 
🌧️ YOLO-Weather: Robust Object Detection in Adverse Weather
# 📌 Overview

Object detection in adverse weather conditions remains a critical challenge for autonomous vehicles. Environmental factors such as snow, fog, rain, and sandstorms significantly degrade visual quality, weaken feature representation, and reduce the reliability of YOLO-based detectors.

This project introduces YOLO-Weather, a robust object detection framework designed to improve detection performance under challenging weather conditions while maintaining real-time capability.

# 🚗 Problem Statement

Adverse weather conditions:

Reduce image contrast and clarity

Introduce high-frequency noise (rain streaks, snow particles)

Cause geometric distortions

Create domain gaps between clean and degraded environments

Although models such as:

YOLOv8STE

D-YOLO

YOLOExtreme

have improved robustness using image enhancement, domain adaptation, or architectural modifications, they still struggle with:

High-frequency weather artifacts

Blurred object edges

Cross-domain inconsistency

# 🧠 Proposed Method: YOLO-Weather

YOLO-Weather builds upon YOLOv12 as the backbone and introduces several key improvements:

🔹 1. Deformable Convolution

Enhances geometric adaptability to handle weather-induced distortions.

🔹 2. Frequency-Domain Attention Block

Uses Fast Fourier Transform (FFT)

Suppresses high-frequency artifacts (rain, snow noise)

Preserves important structural information

Complements spatial attention mechanisms

🔹 3. Consistency Regularization Strategy

Encourages weather-invariant representation learning

Reduces domain switching issues

Eliminates the need for external image restoration networks

# 🏗️ Architecture Overview

YOLOv12 Backbone
⬇
Deformable Convolution
⬇
Frequency-Domain Attention (FFT-based)
⬇
Detection Head with Consistency Regularization

📊 Experimental Results

Evaluated on:

DAWN dataset

Additional weather-related benchmarks

# 🔹 Performance on DAWN
Metric	Score
Precision	89%
Recall	82%
F1-score	85%

The model demonstrates strong robustness under adverse weather conditions while maintaining real-time detection capability for autonomous driving systems.

# ⚙️ Key Contributions

Frequency-domain attention for weather noise suppression

Deformable convolution for geometric robustness

Consistency regularization for domain-invariant learning

Real-time performance without external enhancement pipelines

# 🚀 Applications

Autonomous vehicles

Intelligent transportation systems

Smart surveillance in harsh weather

Advanced driver assistance systems (ADAS)
