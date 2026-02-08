# Smart Farm Monitoring

Full-stack system for detecting abnormal cattle behaviour using video-based analysis and visualising insights through a web-based dashboard.

This repository serves as an **overview and entry point** for the Smart Farm Monitoring system and links to each component that makes up the complete application.

---

## 🚀 Project Overview

The Smart Farm Monitoring system is designed to assist farmers by detecting abnormal livestock behaviour (e.g. prolonged inactivity or heat stress indicators) through video analysis and notifying users via a web-based monitoring interface.

While the system was originally designed to integrate with external CCTV streams, the current implementation uses **recorded video footage** as a simulation of live input due to infrastructure and hardware constraints.  
The overall architecture, however, is structured to support real-time video sources with minimal changes.

---

## 🧩 System Architecture

The system consists of three independently developed components:

| Component | Responsibility | Repository |
|---------|----------------|------------|
| **Frontend** | Dashboard UI for monitoring system status and visualised data | https://github.com/JinLee0811/smart-farm-frontend |
| **Backend** | API service for data ingestion, processing, and alert logic | https://github.com/JinLee0811/smart-farm-backend |
| **ML Service** | Video-based behaviour detection and analytics | https://github.com/JinLee0811/smart-farm-ml-service |

Each component can be developed and tested independently, reflecting a modular, service-oriented design.

---

## 🔄 Data Flow (High-level)

Video Input → ML Service (Detection)
↓
Backend API (Processing & Alerts)
↓
Frontend Dashboard (Visualisation)

- Video input is processed as a continuous stream to **simulate real-time behaviour detection**
- Detected events are sent to the backend for processing and state management
- The frontend visualises system status, alerts, and monitoring results

---

## 🛠 Technology Stack

- **Frontend:** React, Next.js, TypeScript  
- **Backend:** Node.js (REST API)  
- **ML / Analytics:** Python, YOLOv8, OpenCV  
- **Database:** Relational database (e.g. PostgreSQL)  
- **Communication:** REST-based inter-service communication

---

## 📊 Presentation & Detailed Explanation

For a detailed explanation of the problem definition, system design, data flow, limitations, and results, refer to the project presentation below:

👉 **Project Presentation (Canva)**  
https://www.canva.com/design/DAHAtsAZpic/q2x8lIIOW1ayPc_cwyxqwA/edit

The slides provide:
- Problem definition and motivation
- Comparison with existing approaches
- System architecture and data flow
- Implementation details and limitations
- Project outcomes and future directions

---

## ⚠️ Notes on Implementation

- The current system uses recorded video files instead of live CCTV streams due to real-world infrastructure constraints.
- This decision allowed the team to focus on **end-to-end system design, data flow, and integration** rather than hardware dependencies.
- The architecture supports future extension to real-time video sources and multimodal inputs (e.g. video + audio).

---

## 🎯 Why This Project Matters

This project demonstrates:
- Clear problem definition and realistic constraint handling
- Modular full-stack system design
- Integration of ML inference with backend services and frontend visualisation
- Practical trade-offs between accuracy, scalability, and cost

---

## 📫 Contact

For questions or further discussion:  
**jinlee.engineer@gmail.com**
