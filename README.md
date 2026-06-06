<div align="center">

<svg width="100%" viewBox="0 0 900 120" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0a0f1e"/>
      <stop offset="50%" style="stop-color:#0f1a35"/>
      <stop offset="100%" style="stop-color:#0a0f1e"/>
    </linearGradient>
    <linearGradient id="line1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#4ade80;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#4ade80;stop-opacity:1"/>
      <stop offset="70%" style="stop-color:#7c3aed;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#7c3aed;stop-opacity:0"/>
    </linearGradient>
    <linearGradient id="line2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c3aed;stop-opacity:0"/>
      <stop offset="40%" style="stop-color:#7c3aed;stop-opacity:0.6"/>
      <stop offset="60%" style="stop-color:#4ade80;stop-opacity:0.6"/>
      <stop offset="100%" style="stop-color:#4ade80;stop-opacity:0"/>
    </linearGradient>
    <filter id="glow-green">
      <feGaussianBlur stdDeviation="3" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow-violet">
      <feGaussianBlur stdDeviation="4" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- background -->
  <rect width="900" height="120" fill="url(#bg)"/>

  <!-- grid dots -->
  <g opacity="0.15">
    <circle cx="60" cy="30" r="1.2" fill="#4ade80"/><circle cx="120" cy="30" r="1.2" fill="#4ade80"/>
    <circle cx="180" cy="30" r="1.2" fill="#7c3aed"/><circle cx="240" cy="30" r="1.2" fill="#7c3aed"/>
    <circle cx="300" cy="30" r="1.2" fill="#4ade80"/><circle cx="360" cy="30" r="1.2" fill="#4ade80"/>
    <circle cx="420" cy="30" r="1.2" fill="#7c3aed"/><circle cx="480" cy="30" r="1.2" fill="#7c3aed"/>
    <circle cx="540" cy="30" r="1.2" fill="#4ade80"/><circle cx="600" cy="30" r="1.2" fill="#4ade80"/>
    <circle cx="660" cy="30" r="1.2" fill="#7c3aed"/><circle cx="720" cy="30" r="1.2" fill="#7c3aed"/>
    <circle cx="780" cy="30" r="1.2" fill="#4ade80"/><circle cx="840" cy="30" r="1.2" fill="#4ade80"/>
    <circle cx="60" cy="90" r="1.2" fill="#7c3aed"/><circle cx="120" cy="90" r="1.2" fill="#4ade80"/>
    <circle cx="180" cy="90" r="1.2" fill="#4ade80"/><circle cx="240" cy="90" r="1.2" fill="#7c3aed"/>
    <circle cx="300" cy="90" r="1.2" fill="#7c3aed"/><circle cx="360" cy="90" r="1.2" fill="#4ade80"/>
    <circle cx="420" cy="90" r="1.2" fill="#4ade80"/><circle cx="480" cy="90" r="1.2" fill="#7c3aed"/>
    <circle cx="540" cy="90" r="1.2" fill="#7c3aed"/><circle cx="600" cy="90" r="1.2" fill="#4ade80"/>
    <circle cx="660" cy="90" r="1.2" fill="#4ade80"/><circle cx="720" cy="90" r="1.2" fill="#7c3aed"/>
    <circle cx="780" cy="90" r="1.2" fill="#7c3aed"/><circle cx="840" cy="90" r="1.2" fill="#4ade80"/>
  </g>

  <!-- animated circuit lines -->
  <path d="M0,60 Q150,20 300,60 Q450,100 600,60 Q750,20 900,60" stroke="url(#line1)" stroke-width="1.5" fill="none" filter="url(#glow-green)" opacity="0.9">
    <animate attributeName="stroke-dashoffset" from="1800" to="0" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="d" values="M0,60 Q150,20 300,60 Q450,100 600,60 Q750,20 900,60;M0,60 Q150,100 300,60 Q450,20 600,60 Q750,100 900,60;M0,60 Q150,20 300,60 Q450,100 600,60 Q750,20 900,60" dur="6s" repeatCount="indefinite"/>
  </path>
  <path d="M0,60 Q150,100 300,60 Q450,20 600,60 Q750,100 900,60" stroke="url(#line2)" stroke-width="1" fill="none" filter="url(#glow-violet)" opacity="0.7">
    <animate attributeName="stroke-dashoffset" from="0" to="1800" dur="5s" repeatCount="indefinite"/>
  </path>

  <!-- glowing orbs -->
  <circle cx="180" cy="60" r="3" fill="#4ade80" filter="url(#glow-green)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;0.3;0.9" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="60;45;60" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="60" r="4" fill="#7c3aed" filter="url(#glow-violet)" opacity="0.9">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="2.5s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="60;75;60" dur="6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="720" cy="60" r="3" fill="#4ade80" filter="url(#glow-green)" opacity="0.9">
    <animate attributeName="opacity" values="0.9;0.3;0.9" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="cy" values="60;45;60" dur="6s" repeatCount="indefinite"/>
  </circle>

  <!-- top border line -->
  <line x1="0" y1="2" x2="900" y2="2" stroke="url(#line1)" stroke-width="1.5" opacity="0.6"/>
  <!-- bottom border line -->
  <line x1="0" y1="118" x2="900" y2="118" stroke="url(#line2)" stroke-width="1.5" opacity="0.6"/>

  <!-- corner accents -->
  <polyline points="0,0 0,20" stroke="#4ade80" stroke-width="2" opacity="0.8" filter="url(#glow-green)"/>
  <polyline points="0,0 25,0" stroke="#4ade80" stroke-width="2" opacity="0.8" filter="url(#glow-green)"/>
  <polyline points="900,0 900,20" stroke="#7c3aed" stroke-width="2" opacity="0.8" filter="url(#glow-violet)"/>
  <polyline points="875,0 900,0" stroke="#7c3aed" stroke-width="2" opacity="0.8" filter="url(#glow-violet)"/>
  <polyline points="0,120 0,100" stroke="#7c3aed" stroke-width="2" opacity="0.8" filter="url(#glow-violet)"/>
  <polyline points="0,120 25,120" stroke="#7c3aed" stroke-width="2" opacity="0.8" filter="url(#glow-violet)"/>
  <polyline points="900,120 900,100" stroke="#4ade80" stroke-width="2" opacity="0.8" filter="url(#glow-green)"/>
  <polyline points="875,120 900,120" stroke="#4ade80" stroke-width="2" opacity="0.8" filter="url(#glow-green)"/>
</svg>

# Sona Rajarajan

<img src="https://readme-typing-svg.demolab.com?font=DM+Mono&weight=500&size=17&pause=1200&color=38BDF8&center=true&vCenter=true&width=800&lines=Integrated+M.Tech+%E2%80%A2+CSE+with+Business+Analytics+%40+VIT+Chennai;ML+Engineer+%7C+Data+Engineer+%7C+Cloud+Systems;Building+production-ready+AI+%2B+analytics+infrastructure;ingest+%E2%86%92+process+%E2%86%92+predict+%E2%86%92+automate+%E2%86%92+scale" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sona-rajarajan-186445278/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SonaRajarajan)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sonavrajarajan@gmail.com)

<br/>

<img src="https://komarev.com/ghpvc/?username=SonaRajarajan&color=a855f7&style=flat-square&label=profile+views"/>

<br/>

![](https://img.shields.io/badge/Integrated_M.Tech_·_Business_Analytics-0f172a?style=flat-square&labelColor=1e3a5f&color=38bdf8)
![](https://img.shields.io/badge/Infosys_×_AWS_Trained-0f172a?style=flat-square&labelColor=1e3a5f&color=4ade80)
![](https://img.shields.io/badge/5×_Hackathon_Winner-0f172a?style=flat-square&labelColor=1e3a5f&color=facc15)
![](https://img.shields.io/badge/Patent_Under_Review-0f172a?style=flat-square&labelColor=1e3a5f&color=f472b6)
![](https://img.shields.io/badge/Graduating_2027-0f172a?style=flat-square&labelColor=1e3a5f&color=a78bfa)

</div>

---

## 〔 About 〕

```yaml
name        : Sona Rajarajan
degree      : Integrated M.Tech — CSE with Business Analytics
university  : VIT Chennai   |   reg: 22MIA1161   |   graduating: 2027

domains     : [ ML Systems · Data Engineering · Cloud Analytics · LLMOps · IoT/Edge AI ]
currently   : [ LLMs · MLOps · Distributed Systems · Streaming Architectures ]
open_to     : [ ML · Data Engineering · AI Infrastructure · Business Analytics Internships ]
```

I build end-to-end intelligent systems — from streaming pipelines and ML models to cloud-integrated analytics platforms and LLM-powered applications.

The focus is never just the model. It's the entire lifecycle:

```
 RAW DATA  ──►  INGEST  ──►  PROCESS  ──►  PREDICT  ──►  AUTOMATE  ──►  SCALE  ──►  IMPACT
```

---

## 〔 Snapshot 〕

<div align="center">

| Projects | Internships | Research Works | Patent |
|:---:|:---:|:---:|:---:|
| **12+** | **4** | **3** | **1** |

</div>

---

## 〔 Project Portfolio 〕

> Complete breakdown of all projects — domain, objective, and tech stack.

<br/>

### 🤖 AI & Machine Learning

| # | Project | Domain | Objective | Tech Stack |
|---|---------|--------|-----------|------------|
| 01 | **[AI-Integrated Restaurant Wait Time Prediction](https://github.com/SonaRajarajan/AI-Integrated-Restaurant-Wait-Time-Prediction-System)** | Operational Analytics / Hospitality AI | Predict customer wait times using occupancy intelligence, arrival patterns, and table dynamics to optimize restaurant operations | `Python` `scikit-learn` `XGBoost` `Pandas` `ML` |
| 02 | **[AI-Based Home Decor Recommendation System](https://github.com/SonaRajarajan/AI-Based-Home-Decor-Recommendation-System)** | Computer Vision / Recommendation Systems | Solve the online shopping frustration of finding spatially-compatible décor using AI-powered visual matching and personalization | `Python` `Computer Vision` `Recommendation Engine` `AI` |
| 03 | **[AI Human Fall Detection & Monitoring for Elders](https://github.com/SonaRajarajan/AI-Based-Human-Fall-Detection-and-Monitoring-System-for-Elders)** | Healthcare AI / IoT Safety Systems | Analyze movement data in real-time to detect fall incidents and trigger automated alerts for elder care and safety monitoring | `Python` `TensorFlow` `OpenCV` `IoT` `CNN` |
| 04 | **[AI Wellness Monitoring & Health Analytics](https://github.com/SonaRajarajan/AI-Integrated-Wellness-Monitoring-and-Health-Analytics-System)** | Preventive Healthcare / Behavioral Analytics | Apply AI to wellness data to generate actionable health insights supporting preventive care and lifestyle optimization | `JavaScript` `AI` `Analytics` `Health APIs` |
| 05 | **Shape Contour Analyzer** | Computer Vision / Image Processing | Detect, classify, and analyze geometric shapes using contour detection for accurate visual pattern recognition | `Python` `OpenCV` `Image Processing` `Contour Detection` |
| 06 | **Pixel Dash — Gamified Employee Wellness Platform** | Enterprise AI / HR Analytics | AI-driven gamified corporate wellness system with behavioral analytics and engagement scoring *(Patent Under Review)* | `LangChain` `Gemini` `Power BI` `Python` |

<br/>

### 📊 Data Engineering & Analytics

| # | Project | Domain | Objective | Tech Stack |
|---|---------|--------|-----------|------------|
| 07 | **[Real-Time Streaming Data Pipeline](https://github.com/SonaRajarajan)** | Data Engineering / Stream Processing | Build a Kafka-powered streaming infrastructure integrating anomaly detection and Lambda Architecture for real-time analytics | `Apache Kafka` `InfluxDB` `Grafana` `Docker` `Lambda Architecture` |
| 08 | **[Data Analytics Version Control System](https://github.com/SonaRajarajan/Data-Analytics-Version-Control)** | MLOps / Experiment Tracking | Manage versions of datasets, analytics code, and experiment outputs enabling reproducible ML workflows and result comparison | `HTML` `Python` `Git` `ETL` `Experiment Tracking` |
| 09 | **Metropolitan Bus Network Optimizer** | Smart Mobility / Transit Analytics | Forecast transit demand and optimize bus allocation for smart city mobility planning using predictive analytics | `Python` `ML` `SQL` `Optimization` `ARIMA` |
| 10 | **Smart Carpooling Analytics Platform** | Predictive Mobility / Route Optimization | Intelligent ride allocation and route optimization using ML-based demand prediction and spatial analytics | `ML` `Optimization` `SQL` `Geospatial` |

<br/>

### 🏥 Healthcare & Clinical AI

| # | Project | Domain | Objective | Tech Stack |
|---|---------|--------|-----------|------------|
| 11 | **DR.CHAT — Multilingual Health Triage Chatbot** | NLP / Clinical AI | Multilingual NLP-powered health triage system integrating WHO/CDC/ICMR APIs for real-time symptom-based guidance | `Python` `BERT` `NLP` `WHO API` `ICMR` `FastAPI` |
| 12 | **Melanoma Detection System** | Medical Imaging / Computer Vision | CNN-based skin lesion classifier achieving high accuracy for early-stage melanoma detection from dermoscopic images | `Python` `TensorFlow` `CNN` `Medical Imaging` |
| 13 | **Alzheimer's Disease Detection** | Medical Imaging / Clinical ML | MRI-based cognitive decline detection using ensemble ML to support early clinical diagnosis | `Python` `XGBoost` `MRI Analysis` `scikit-learn` |
| 14 | **Wearable Sensor HAR Safety Pipeline** | Edge AI / Healthcare IoT | Human Activity Recognition system on wearable sensors using CNN-LSTM for worker safety monitoring in industrial environments | `Python` `CNN-LSTM` `TensorFlow` `IoT` `Edge AI` |

<br/>

### ☁️ Cloud, Systems & Infrastructure

| # | Project | Domain | Objective | Tech Stack |
|---|---------|--------|-----------|------------|
| 15 | **Allo Inventory — Full-Stack Reservation System** | Backend Engineering / Distributed Systems | Next.js inventory reservation platform with Redis distributed locks ensuring zero race conditions at concurrent write load | `Next.js` `Redis` `PostgreSQL` `Distributed Locks` `TypeScript` |
| 16 | **IoT Smart Home Energy Analytics** | Edge Computing / Sustainability Analytics | Real-time predictive energy analytics for smart homes enabling operational efficiency and consumption forecasting | `Python` `IoT` `Time-Series ML` `Visualization` |
| 17 | **NLP Customer Care Routing System** | NLP Automation / Enterprise AI | Intelligent NLP-powered request prioritization and routing automation for enterprise customer support workflows | `Python` `NLP` `Transformers` `Automation` |
| 18 | **Telehealth Physiotherapy Platform** | Healthcare + Computer Vision | Real-time pose estimation and physiotherapy guidance platform using body landmark tracking for remote rehabilitation | `FastAPI` `OpenCV` `MediaPipe` `Computer Vision` |

---

## 〔 Experience 〕

| Organization | Role | Highlights |
|---|---|---|
| ☁️ **Infosys × AWS** | Cloud Engineer Trainee | End-to-end cloud ML deployment on AWS infrastructure |
| 📊 **Infosys Springboard** | Data Science / Analytics Intern | **Top 5 Achiever** out of 500+ participants |
| 📡 **GAO Tek Inc.** | Data Engineering / IoT Intern | IoT data systems and backend engineering |
| 📦 **MIB Industries** | Supply Chain Analytics Intern | Supply chain optimization and analytics |

---

## 〔 Tech Stack 〕

<div align="center">

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

**AI / ML**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21F?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square&logo=xgboost&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)

**Data Engineering**

![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apache-kafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat-square&logo=influxdb&logoColor=white)

**Cloud & Visualization**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

</div>

---

## 〔 Achievements & Research 〕

```diff
+ 5× Hackathon Winner  (National Level)
+ Patent Under Review  (AI-Driven Gamified Employee Wellness Platform — Pixel Dash)
+ Top 5 Achiever @ Infosys Springboard  (out of 500+ participants)
+ 3 Research Works in progress
```

**Research Areas**
- Human Activity Recognition & Motion Safety Monitoring (CNN-LSTM, Wearable Sensors)
- Gamified Corporate Wellness Analytics (LLM-powered, Patent Pending)
- Gen Z CRM Intelligence & Consumer Behavior Analytics

---

## 〔 GitHub Analytics 〕

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=SonaRajarajan&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0f1e&title_color=c084fc&icon_color=22d3ee&text_color=e2e8f0&ring_color=a855f7"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SonaRajarajan&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0f1e&title_color=c084fc&text_color=22d3ee"/>

<br/>

<img src="https://streak-stats.demolab.com?user=SonaRajarajan&hide_border=true&background=0A0F1E&ring=c084fc&fire=a855f7&currStreakLabel=c084fc&sideLabels=22d3ee&dates=94a3b8&currStreakNum=22d3ee&sideNums=22d3ee&stroke=0a0f1e&border=0a0f1e&starting_year=2023"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=SonaRajarajan&bg_color=0a0f1e&hide_border=true&line=a855f7&point=22d3ee&color=c084fc&area=true&area_color=581c87"/>

</div>

---

<div align="center">

## let's build something meaningful ⚡

Open to internship opportunities in:

`Machine Learning` · `Data Engineering` · `AI Infrastructure` · `Business Analytics` · `Cloud/DevOps`

<br/>

[![LinkedIn](https://img.shields.io/badge/connect_on_linkedin-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sona-rajarajan-186445278/)
[![GitHub](https://img.shields.io/badge/explore_projects-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SonaRajarajan)
[![Email](https://img.shields.io/badge/send_a_mail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sonavrajarajan@gmail.com)

<br/><br/>

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  © 2025 Sona Rajarajan  ·  VIT Chennai  ·  Building the future, one commit at a time
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

</div>
