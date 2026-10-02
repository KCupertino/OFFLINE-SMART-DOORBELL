# An Intelligent but Offline Smart Doorbell ECE 635

## Motivation
Smart doorbells are useful for identifying people who come to the door but many smart doorbell systems depend on cloud services and an internet connection.In this project I want to build a simple smart doorbell that can process the
camera input locally on an edge device this will help me understand how machinelearning models can be deployed and run directly on devices like Raspberry Pi.

## Design Goals

The main goal of this project is to build an offline smart doorbell using a raspberry pi and the camera module.

The system should be able to:
 - Detect when a person appears in front of the camera and capture an image of the person.
 - Run a person detection model on the edge device.
 Identify whether the person is a known person or a unknown person and perform the inference locally without depending on cloud processing.

## Deliverables

The main deliverables for this project are:

- Learn how to deploy a machine learning model on an edge device and implement a lightweight face or person detection model.
- Capture an image when someone appears in front of the      camera.
- Run inference directly on the edge device and identify known and unknown people.
- Provide the code and a final demonstration of the system.


## System Blocks

The basic flow of the system will be:

Camera - Capture Image - Face / Person Detection - Generate Face Embedding -Compare with Stored Known Person Embeddings
-Known / Unknown Person -Display / Log Result

The camera will capture the image of a person at the door and the lightweight model will be used for face or person detection for recognizing known people the system will store embeddings of known people and compare them with the embedding of the detected person.

## Hardware Requirements

- Raspberry Pi or BeagleBone
- Camera module
- Required power supply and storage

## Software Requirements

- Python
- Linux / Raspberry Pi OS
- TensorFlow Lite or another lightweight face/person detection model
- Git and GitHub

## Team member responsibilities

- Team Member 1 : Athiniraj Karthigairaj

I will be responsible for setting up the hardware and software, implementing
the detection system, testing the model, researching suitable lightweight
models, documenting the project, and preparing the final demonstration.

## Lead Roles

- Setup
- Software
- Networking
- Writing
- Research
- Algorithm Design

## Project Timeline

# Phase1 - Research and setup
- Learn the basics of running ML models on edge devices
- Research lightweight face/person detection models
- Set up the Raspberry pi and camera

# Phase 2 - Face / person detection
- Capture images using the camera.
- Set up a lightweight detection model
- Test person or face detection.

# Phase 3 - Known person recognition
- Create store embeddings for known people.
- Compare detected persons embedding with stored embeddings
- Classify person as known or unknown

# Phase 4 - Edge deployment
- Run the complete system directly on the edge device.
- Test the system with different people.
- Make sure the model can run efficiently on the device.

# Phase 5 - Final demo 
- Test the complete smart doorbell system
- Prepare the code for submission
- Prepare the final demonstration

## References
Howard, A. G., et al., "MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications," 2017. https://arxiv.org/abs/1704.04861