<div align="center">
<svg width="100%" viewBox="0 0 900 130" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- backgrounds -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#050810"/>
      <stop offset="40%" style="stop-color:#0f0a2e"/>
      <stop offset="70%" style="stop-color:#071a10"/>
      <stop offset="100%" style="stop-color:#050810"/>
    </linearGradient>
    <!-- neural pulse gradient -->
    <linearGradient id="pulseGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#4ade80;stop-opacity:0"/>
      <stop offset="25%" style="stop-color:#4ade80;stop-opacity:1"/>
      <stop offset="50%" style="stop-color:#a855f7;stop-opacity:1"/>
      <stop offset="75%" style="stop-color:#7c3aed;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#7c3aed;stop-opacity:0"/>
    </linearGradient>
    <linearGradient id="pulseGrad2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#7c3aed;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#7c3aed;stop-opacity:0.8"/>
      <stop offset="60%" style="stop-color:#4ade80;stop-opacity:0.8"/>
      <stop offset="100%" style="stop-color:#4ade80;stop-opacity:0"/>
    </linearGradient>
    <!-- shark slash fill -->
    <linearGradient id="slashFill" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#4ade80;stop-opacity:0.07"/>
      <stop offset="50%" style="stop-color:#7c3aed;stop-opacity:0.12"/>
      <stop offset="100%" style="stop-color:#4ade80;stop-opacity:0.07"/>
    </linearGradient>
    <!-- glow filters -->
    <filter id="glowG" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3.5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glowV" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glowSoft" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="8" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <clipPath id="sharkClip">
      <polygon points="0,0 900,0 900,95 820,130 0,130"/>
    </clipPath>
  </defs>
  <!-- base background -->
  <rect width="900" height="130" fill="url(#bgGrad)"/>
  <!-- shark-slice diagonal fill panel (Option 3 aesthetic) -->
  <polygon points="0,0 900,0 900,90 780,130 0,130" fill="url(#slashFill)"/>
  <!-- secondary reverse slash accent -->
  <polygon points="0,110 200,130 0,130" fill="#4ade80" opacity="0.05"/>
  <polygon points="900,80 900,130 650,130" fill="#7c3aed" opacity="0.06"/>
  <!-- sharp diagonal slice edge lines (shark cuts) -->
  <line x1="0" y1="108" x2="790" y2="108" stroke="#4ade80" stroke-width="0.5" opacity="0.2"/>
  <line x1="0" y1="112" x2="800" y2="112" stroke="#7c3aed" stroke-width="0.3" opacity="0.15"/>
  <!-- neural network nodes (Option 1) — background layer -->
  <g opacity="0.18">
    <circle cx="80"  cy="35" r="2" fill="#4ade80"/>
    <circle cx="200" cy="55" r="2" fill="#7c3aed"/>
    <circle cx="330" cy="28" r="2" fill="#4ade80"/>
    <circle cx="450" cy="65" r="2" fill="#a855f7"/>
    <circle cx="580" cy="30" r="2" fill="#7c3aed"/>
    <circle cx="700" cy="58" r="2" fill="#4ade80"/>
    <circle cx="820" cy="35" r="2" fill="#7c3aed"/>
    <circle cx="140" cy="90" r="1.5" fill="#7c3aed"/>
    <circle cx="270" cy="80" r="1.5" fill="#4ade80"/>
    <circle cx="400" cy="95" r="1.5" fill="#4ade80"/>
    <circle cx="520" cy="78" r="1.5" fill="#7c3aed"/>
    <circle cx="650" cy="88" r="1.5" fill="#a855f7"/>
    <circle cx="760" cy="72" r="1.5" fill="#4ade80"/>
  </g>
  <!-- neural synapse lines -->
  <g opacity="0.12" stroke-width="0.8">
    <line x1="80"  y1="35" x2="200" y2="55"  stroke="#4ade80"/>
    <line x1="200" y1="55" x2="330" y2="28"  stroke="#7c3aed"/>
    <line x1="330" y1="28" x2="450" y2="65"  stroke="#4ade80"/>
    <line x1="450" y1="65" x2="580" y2="30"  stroke="#a855f7"/>
    <line x1="580" y1="30" x2="700" y2="58"  stroke="#7c3aed"/>
    <line x1="700" y1="58" x2="820" y2="35"  stroke="#4ade80"/>
    <line x1="140" y1="90" x2="270" y2="80"  stroke="#7c3aed"/>
    <line x1="270" y1="80" x2="400" y2="95"  stroke="#4ade80"/>
    <line x1="400" y1="95" x2="520" y2="78"  stroke="#4ade80"/>
    <line x1="520" y1="78" x2="650" y2="88"  stroke="#7c3aed"/>
    <line x1="650" y1="88" x2="760" y2="72"  stroke="#a855f7"/>
    <!-- cross links -->
    <line x1="80"  y1="35" x2="140" y2="90"  stroke="#4ade80"/>
    <line x1="330" y1="28" x2="270" y2="80"  stroke="#7c3aed"/>
    <line x1="450" y1="65" x2="400" y2="95"  stroke="#a855f7"/>
    <line x1="580" y1="30" x2="520" y2="78"  stroke="#4ade80"/>
    <line x1="700" y1="58" x2="650" y2="88"  stroke="#7c3aed"/>
    <line x1="820" y1="35" x2="760" y2="72"  stroke="#4ade80"/>
  </g>
  <!-- ANIMATED pulse wave (Option 2 radar sweep aesthetic) -->
<path d="M0,65 Q100,30 200,65 Q300,100 400,65 Q500,30 600,65 Q700,100 800,65 Q850,45 900,65"
     stroke="url(#pulseGrad)" stroke-width="1.8" fill="none" filter="url(#glowG)" opacity="0.95">
<animate attributeName="d"
   values="
     M0,65 Q100,30 200,65 Q300,100 400,65 Q500,30 600,65 Q700,100 800,65 Q850,45 900,65;
     M0,65 Q100,100 200,65 Q300,30 400,65 Q500,100 600,65 Q700,30 800,65 Q850,85 900,65;
     M0,65 Q100,30 200,65 Q300,100 400,65 Q500,30 600,65 Q700,100 800,65 Q850,45 900,65"
   dur="5s" repeatCount="indefinite"/>
</path>
<path d="M0,65 Q100,100 200,65 Q300,30 400,65 Q500,100 600,65 Q700,30 800,65 Q850,85 900,65"
     stroke="url(#pulseGrad2)" stroke-width="1" fill="none" filter="url(#glowV)" opacity="0.7">
<animate attributeName="d"
   values="
     M0,65 Q100,100 200,65 Q300,30 400,65 Q500,100 600,65 Q700,30 800,65 Q850,85 900,65;
     M0,65 Q100,30 200,65 Q300,100 400,65 Q500,30 600,65 Q700,100 800,65 Q850,45 900,65;
     M0,65 Q100,100 200,65 Q300,30 400,65 Q500,100 600,65 Q700,30 800,65 Q850,85 900,65"
   dur="7s" repeatCount="indefinite"/>
</path>
  <!-- animated neural node pulses (glowing active nodes) -->
  <circle cx="200" cy="55" r="4" fill="#4ade80" filter="url(#glowG)">
    <animate attributeName="opacity" values="1;0.2;1" dur="2.2s" repeatCount="indefinite"/>
    <animate attributeName="r" values="4;6;4" dur="2.2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="65" r="5" fill="#a855f7" filter="url(#glowV)">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="r" values="5;3;5" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="58" r="4" fill="#4ade80" filter="url(#glowG)">
    <animate attributeName="opacity" values="1;0.2;1" dur="2.8s" repeatCount="indefinite"/>
    <animate attributeName="r" values="4;6;4" dur="2.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="330" cy="28" r="3" fill="#7c3aed" filter="url(#glowV)">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="1.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="580" cy="30" r="3" fill="#4ade80" filter="url(#glowG)">
    <animate attributeName="opacity" values="1;0.3;1" dur="2.4s" repeatCount="indefinite"/>
  </circle>
  <!-- shark-edge: sharp diagonal cut bottom border -->
  <polyline points="0,126 860,126 900,115" stroke="#4ade80" stroke-width="1.2" fill="none" opacity="0.5" filter="url(#glowG)"/>
  <polyline points="0,129 840,129 900,118" stroke="#7c3aed" stroke-width="0.7" fill="none" opacity="0.35" filter="url(#glowV)"/>
  <!-- top scan line (radar sweep) -->
  <line x1="0" y1="1.5" x2="900" y2="1.5" stroke="url(#pulseGrad)" stroke-width="1.5" opacity="0.7"/>
  <!-- corner HUD brackets -->
  <g filter="url(#glowG)" stroke="#4ade80" stroke-width="1.8" fill="none" opacity="0.9">
    <polyline points="0,18 0,0 22,0"/>
    <polyline points="878,0 900,0 900,18"/>
  </g>
  <g filter="url(#glowV)" stroke="#7c3aed" stroke-width="1.8" fill="none" opacity="0.9">
    <polyline points="0,112 0,130 22,130"/>
  </g>
  <g filter="url(#glowG)" stroke="#4ade80" stroke-width="1.8" fill="none" opacity="0.9">
    <polyline points="878,115 900,105"/>
  </g>
</svg>

# Sona Rajarajan

<img src="https://readme-typing-svg.demolab.com?font=DM+Mono&weight=500&size=17&pause=1200&color=38BDF8&center=true&vCenter=true&width=800&lines=Integrated+M.Tech+%E2%80%A2+CSE+with+Business+Analytics+%40+VIT+Chennai;ML+Engineer+%7C+Data+Engineer+%7C+Cloud+Systems;Building+production-Ready+AI+%2B+Analytics+Infrastructure;Ingest+%E2%86%92+Process+%E2%86%92+Predict+%E2%86%92+Automate+%E2%86%92+Scale" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sona-rajarajan-186445278/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SonaRajarajan)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sonavrajarajan@gmail.com)

<br/>

<img src="https://komarev.com/ghpvc/?username=SonaRajarajan&color=a855f7&style=flat-square&label=Profile+Views"/>

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
Name        : Sona Rajarajan
Degree      : Integrated M.Tech — CSE with Business Analytics
University  : VIT Chennai   |   reg: 22MIA1161   |   graduating: 2027

Domains     : [ ML Systems · Data Engineering · Cloud Analytics · LLMOps · IoT/Edge AI ]
Currently   : [ LLMs · MLOps · Distributed Systems · Streaming Architectures ]
Open_To     : [ ML · Data Engineering · AI Infrastructure · Business Analytics Internships ]
```

I Build end-to-end intelligent systems — from streaming pipelines and ML models to cloud-integrated analytics platforms and LLM-powered applications.

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

<img src="https://github-readme-stats.vercel.app/api?username=SonaRajarajan&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0f1e&title_color=4ade80&icon_color=4ade80&text_color=4ade80&ring_color=7c3aed"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=SonaRajarajan&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0f1e&title_color=4ade80&text_color=4ade80"/>

<br/>

<img src="https://streak-stats.demolab.com?user=SonaRajarajan&hide_border=true&background=0A0F1E&ring=7c3aed&fire=7c3aed&currStreakLabel=4ade80&sideLabels=4ade80&dates=4ade80&currStreakNum=4ade80&sideNums=4ade80&stroke=0a0f1e&border=0a0f1e&starting_year=2023"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=SonaRajarajan&bg_color=0a0f1e&hide_border=true&line=7c3aed&point=4ade80&color=4ade80&area=true&area_color=2e1065"/>

</div>

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
