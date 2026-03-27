<p align="center">
  <img src="docs/hero.jpg" width="100%" alt="HappySession Surf Forecast">
</p>

<p align="center">
  <img src="docs/logo_round.png" width="80" alt="HappySession logo">
</p>

<h1 align="center">HappySession</h1>

<p align="center">
Surf forecasting powered by ocean models, rules engines and machine learning.
</p>

<p align="center">
<a href="https://happysession.org">🌍 happysession.org</a>
</p>

<p align="center">
<img src="https://img.shields.io/badge/backend-java-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/data-python-yellow?style=for-the-badge">
<img src="https://img.shields.io/badge/mobile-swiftui-orange?style=for-the-badge">
<img src="https://img.shields.io/badge/web-nuxt3-00DC82?style=for-the-badge">
<img src="https://img.shields.io/badge/database-mongodb-green?style=for-the-badge">
</p>

<p align="center">
<img src="https://img.shields.io/badge/rules-drools-red?style=for-the-badge">
<img src="https://img.shields.io/badge/gateway-krakend-purple?style=for-the-badge">
<img src="https://img.shields.io/badge/infrastructure-docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img src="https://img.shields.io/badge/AWS-Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white">
<img src="https://img.shields.io/badge/AWS-Cognito-DD344C?style=for-the-badge&logo=amazonaws&logoColor=white">
</p>

---

# Turning ocean data into surf sessions

HappySession is a platform that transforms **raw oceanographic models into real surf forecasts**.

The project explores how **wave models translate into surf conditions at specific spots**, combining:

- 🌊 NOAA WaveWatch III ocean models  
- 🧠 rule-based surf forecasting  
- 🤖 machine learning spot classifiers  
- ⚙️ microservice backend architecture  
- 📱 native mobile applications  
- 🌐 modern web interface  

---

# 📱 iOS Application

Native SwiftUI application designed to help surfers quickly identify the **best spots and best time to paddle out**.

<p align="center">

<img src="docs/best_EN.jpg" width="200">
<img src="docs/understand_EN.jpg" width="200">
<img src="docs/map_EN.jpg" width="200">
<img src="docs/top_sessions_EN_2.jpg" width="200">
</p>

Features:

- **Stop analyzing.** Start surfing.
- **We tell you when to surf.** One hour. The right one.
- **Everything that matters.** At a glance.
- **Explore and compare.** Stop searching. Choose.


---

# 🌐 Web Application

HappySession is also available on the web.

Explore forecasts and surf spots directly in your browser.

🌍 https://happysession.org

<img src="docs/web.png" width="800">

Built with:

- **Nuxt 3**
- Vue
- map visualization
- REST APIs

---

# 🧠 Forecast Engine

The core of HappySession is a **hybrid forecasting engine** combining:

### Rule based forecasting

A **Drools rules engine** interprets wave models and surf spot characteristics.

Rules consider:

- swell direction
- swell period
- tide phase
- wind direction
- wind strength
- spot orientation

### Machine learning models

Some spots use **trained classifiers** to detect good surf conditions.

Example model: happy-model-trestraou

Predicts surf quality at **Trestraou surf spot**.

---

# 🏗 Platform Architecture

HappySession is built as a **modular microservice architecture**.

NOAA WaveWatch III
│
▼
Data extraction
│
▼
Forecast computation
│
▼
API
│
▼
Mobile & Web apps


---

# 🧩 Platform Components

| Service | Description | Tech |
|-------|-------------|------|
| **happy-extractor** | Extracts wave model data from NOAA | Python |
| **happy-api** | Core backend API | Java |
| **happy-rules-engine** | Forecast computation engine | Drools |
| **happy-rules** | Surf forecasting rule set | Drools |
| **happy-mongo** | Forecast data storage | MongoDB |
| **happy-gateway** | API gateway with JWT security | KrakenD |
| **happy-iOS** | Native mobile application | SwiftUI |
| **happy-web** | Web client | Nuxt 3 |
| **happy-model-trestraou** | ML classifier for surf prediction | Python |

---

# 📊 Data Pipeline

The forecasting pipeline runs continuously.

1️⃣ Extract wave model data from NOAA  
2️⃣ Store data in MongoDB  
3️⃣ Compute forecasts every 6 hours  
4️⃣ Expose predictions via REST API  
5️⃣ Deliver forecasts through web and mobile apps

---

# 🎯 Project Goal

HappySession explores new approaches to surf forecasting:

- translating ocean model data into surfable conditions
- combining **rule-based and machine learning prediction**
- building a full **data → backend → mobile platform**

The project aims to better understand how **ocean dynamics translate into real surf sessions**.

---

# 👨‍💻 Author

Created by **Sébastien Durand**

Software engineer and surfer building tools to better understand waves.


🧪 **HappySession is a private platform currently under active development.**