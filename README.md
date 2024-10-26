# Computer Vision for Facial Identification at ASU

## Table of Contents
- [Project Overview](#project-overview)
- [Problem Definition](#problem-definition)
- [Proposed Solution](#proposed-solution)
- [Impact and Scope](#impact-and-scope)
- [Implementation](#implementation)
- [Deployment Plan](#deployment-plan)
- [Model Architecture](#model-architecture)
- [Evaluation and Risks](#evaluation-and-risks)
- [Future Enhancements](#future-enhancements)
- [References](#references)

---

## Project Overview
This project introduces a facial recognition system for Arizona State University (ASU) to streamline campus access and automate attendance logging. This solution provides a secure, convenient alternative to physical IDs and integrates with ASU’s Learning Management System (LMS) for automated record-keeping.

## Problem Definition
The current ASU system relies on physical ID cards, which can be lost, stolen, or shared, compromising both security and efficiency. This project aims to replace traditional methods with biometric facial recognition to enhance security and user experience.

## Proposed Solution

### End-to-End Solution Process
1. **Consent Acquisition:** Students authorize the use of their facial images.
2. **Image Collection & Storage:** Capture and store images at campus entry points.
3. **LMS Integration:** Syncs facial recognition data with ASU’s LMS (Canvas) for automatic attendance.
4. **Deployment Strategy:** Phased rollout with ongoing feedback and optimization.

---

## Impact and Scope

- **Convenience:** Students access facilities without needing a physical ID.
- **Efficiency:** Speeds up attendance and entry processes.
- **Security:** Limits unauthorized access and attendance fraud.
- **Campus-wide Scope:** Covers lecture halls, study rooms, and event spaces.

### Stakeholders
- **Students and Faculty:** Benefit from secure, seamless access.
- **Campus Security:** Enhanced monitoring with reduced fraud risk.
- **ASU IT Department:** Manages technical aspects and updates.

---

## Implementation

### Resource Requirements
- **Personnel:** Project Managers, IT Security Experts, Developers, and a Maintenance Team.
- **Data:** Facial images for database updates and model training.
- **Technology:** Camera installation, servers for data processing, and regular maintenance.

### Estimated Costs
- **Hardware:** Camera and server setup.
- **Maintenance:** Periodic software and hardware updates, cybersecurity.
- **Training & Hiring:** Additional staff and faculty training.

---

## Deployment Plan

1. **Pilot Testing:** Initial testing in controlled areas to ensure system accuracy.
2. **Performance Metrics:** Measure accuracy, processing speed, and user satisfaction.
3. **Compliance & Security Audits:** Regular checks to ensure privacy and data integrity.

---

## Model Architecture

The project leverages **ResNet-50** with transfer learning, fine-tuned for ASU’s dataset. The architecture includes:
- **Preprocessing:** Images are processed for compatibility with the model.
- **Training:** 50 epochs with the Adam optimizer, learning rate adjustments, and fine-tuning.
- **Validation:** Accuracy and loss are tracked to monitor performance.

### Training Data
- Dataset of 17,822 images, including ASU student images and labeled face data from Pinterest.

---

## Evaluation and Risks

- **Metrics:** Categorical cross-entropy loss and accuracy score.
- **Risk Mitigation:** Addresses security, technical, and privacy risks to ensure reliability and user trust.

### Potential Risks
- **Privacy Concerns:** Strict data access protocols.
- **Technical Failures:** Backup systems for uninterrupted access.
- **Bias Mitigation:** Diverse data collection representing ASU’s demographics.

---

## Future Enhancements

- **Advanced Model Architectures:** Explore attention mechanisms and capsule networks for improved feature focus.
- **Model Compression:** Techniques like quantization to reduce model size and improve processing efficiency.
- **Data Augmentation:** Enhanced techniques for a more diverse and robust dataset.

---

## References
- [VGGFace Dataset](https://exposing.ai/vgg_face/)
- [ResNet-50](https://pytorch.org/hub/nvidia_deeplearningexamples_resnet50/)
- [Paper Reference - IJERT Volume 09 Issue 05, May 2020](https://www.ijert.org/volume-09-issue-05-may-2020)
- [GitHub - Face Recognition Code by aakashjhawar](https://github.com/aakashjhawar/face-recognition-using-deep-learning)
- [GitHub - Celebrity Face Recognition by Srikeshram](https://github.com/Srikeshram/Celebrity-Face-Recognition)
