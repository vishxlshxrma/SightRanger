# **SightRanger 🛰️🔒**

### **AI-Powered Smart Surveillance System**

SightRanger is an intelligent, real-time surveillance and intrusion-detection platform built using **FastAPI**, **YOLOv8**, and **Next.js**.
It continuously monitors video streams from webcams or mobile devices, detects human presence using deep-learning, and instantly sends email alerts with captured evidence.

---

## 🚀 **Features**

### **🔍 Real-Time Intrusion Detection**

Continuously captures video and uses a **YOLOv8 model** to detect human intrusions with high accuracy.

### **📨 Email Alert System**

Automatically sends email notifications with **attached video clips** whenever a human is detected.

### **🖥️ Web Dashboard (Next.js)**

Manage surveillance settings, view clips, monitor alerts, and customize configurations from an intuitive dashboard.

### **📦 Bulk Video Processing**

Efficient batch-processing pipeline reduces model load and improves performance for continuous monitoring.

### **⚙️ Modular Architecture**

Independent **backend + frontend** services designed for scalability, containerized via Docker.

---

## 🛠️ **Tech Stack**

| Component        | Technology Used             |
| ---------------- | --------------------------- |
| Backend          | FastAPI, Python 3.11        |
| ML Model         | YOLOv8                      |
| Frontend         | Next.js 14, React, Tailwind |
| Notifications    | Email/SMTP                  |
| Containerization | Docker & Docker Compose     |

---

# 🧰 Getting Started

## **1️⃣ Clone the Repository**

```bash
git clone https://github.com/vishxlshxrma/SightRanger.git
cd SightRanger
```

---

## **2️⃣ Configure Environment Variables**

Copy the example environment files:

```bash
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env
```

Now update your credentials inside both `.env` files:

* Email SMTP credentials
* Model configuration
* Frontend API URLs
* Any custom settings

---

## **3️⃣ Build & Run the Application**

### Using Docker Compose:

```bash
docker compose up --build
```

Or using Make:

```bash
make run
```

Once running, access the dashboard at:

👉 **[http://localhost:3000](http://localhost:3000)**

---

## **4️⃣ Stop & Clean Containers**

```bash
docker compose down --remove-orphans
```

Or using Make:

```bash
make clean
```

---

# 📬 Acknowledgments

SightRanger is powered by **YOLOv8** — an industry-leading real-time object detection model.
Special thanks to the open-source community for enabling powerful, accessible AI tools.