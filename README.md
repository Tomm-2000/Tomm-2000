# Hussain Yousef · Project Portfolio

I build tools that help people find evidence, interpret data, and make decisions. This page describes the problems I worked on, how the software approaches them, and what I tested. Source repositories for my own projects are maintained separately.

## AI Engineering · Retrieval and Language Models

**Customer Services RAG** helps a support agent answer questions from a knowledge base. It combines keyword search (BM25), semantic search, and knowledge-graph retrieval to find relevant material. Gemini drafts a reply with citations, and uncertain cases go to a human reviewer who can check the evidence.

**MedRAG · Graduation project** explores how to support stroke-related research questions with traceable answers. FAISS and BM25 retrieve candidate passages, Neo4j supplies graph context, and MedCPT reranks the biomedical evidence. A reviewer can trace an individual claim back to its source. The intended use is research and professional review.

**GrantPilot AI** helps a grant-reporting team bring supporting documents and financial records together. The prototype extracts evidence, reconciles records, and uses the resulting material to draft reports for review.

**Semantic FAQ Chatbot** matches a user's wording to an existing FAQ, even when the question uses different words. It compares BGE embeddings using cosine similarity and falls back when the best match is weak.

## Speech and Audio

**Speech Emotion Recognition** predicts one of eight vocal emotions from a recording. Two frozen speech encoders, wav2vec 2.0 and WavLM, each feed a small classifier. The system averages their class probabilities. Across five speaker-disjoint RAVDESS development folds, the ensemble reached a mean macro F1 of **0.757**, compared with **0.717** and **0.727** for the individual models. On a fixed external sample of 30 CREMA-D recordings it classified **7 of 30** correctly. This small external check illustrates how strongly performance can depend on the recording collection.

## Full-Stack Engineering

**Damascus Student Work & Training** is an Arabic-first React, TypeScript, and Express prototype for students and employers. A scheduling engine accounts for classes, travel time, existing shifts, and overlapping availability. For example, two students available from 10–12 and 11–13 together cover three hours of a 10–14 shift. The employer can see the uncovered hour before assigning the shift. The prototype uses synthetic data and has 42 passing tests in the verified release.

## Computer Vision

| Project | What it does |
| --- | --- |
| Multi-Object Detection & Tracking | Pairs YOLO11 detections with Deep SORT so a viewer can follow the same object across successive video frames using its track ID. |
| Building Damage Assessment | Explores building damage in xView2 satellite imagery, using computer vision to study damage visible after a disaster. |
| Plant Disease Classification | Compares a CNN and ResNet50 for assigning a disease label to a leaf photograph. |
| Traffic Sign Recognition | Uses pretrained vision transformers to classify traffic-sign images and explores transfer learning for visual recognition. |
| MediaPipe Curl Counter | Turns webcam pose landmarks into elbow angles and uses angle thresholds to count completed repetitions. |
| YOLOv8 Object Detection | Locates and labels objects in still images or live webcam input, returning a bounding box for each detection. |
| Haar Face & Eye Detection | Uses pretrained OpenCV cascades to locate faces and eyes in an image. |
| K-Means Image Segmentation | Groups pixels by color and reconstructs the image from those groups to show what color-based segmentation captures. |
| Digital Image Processing | Collects OpenCV coursework exploring how processing operations change an image before higher-level visual analysis. |
| CIFAR-10 Image Classification | Explores transfer learning for assigning small images to one of ten object categories. |

## Machine Learning and Statistics

- **Movie Recommendation System** uses collaborative filtering to suggest movies from patterns in users' preferences.
- **AI Music Generation** models sequences of MIDI events with a PyTorch LSTM and generates musical continuations.
- **Applied Probability & Statistics** uses Python to investigate probability distributions and interpret data through statistical exercises.

## Networking Labs

**Cisco Packet Tracer Labs** covers IPv6 routing, VLAN configuration, and connectivity checks. The exercises connect configuration choices to an observable outcome: which hosts can reach each other across the simulated network.
