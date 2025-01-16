# HappySession

**HappySession** project attempts to provide surfing forecasts for spots in Brittany (and elsewhere).  

![bg9](https://github.com/user-attachments/assets/011d1a5a-71bd-41f4-b326-df7873223fdf)

The **HappySession** service is built around several components:  

| Service | Description | Status | Visibility | Languages |
|---------|:------------|--------|------------|-----------|
| **happy-mongo** | An TLS/SSH secured Docker image of [MongoDB](https://www.mongodb.com). | prod | private | Dockerfile |
| **happy-gateway** | A [Krakend CE](https://www.krakend.io) configuration to propose a gateway with some interresting features as JWT sign and validation on API verbs. | prod | private | Krankend yaml |
| **happy-api** | The main API verbs for the `happysession`system. | prod | private | Java, Dockerfile |
| **happy-extractor** | As its name suggests, this component extracts raw data from [NOAA's WW3 model](https://polar.ncep.noaa.gov/waves/wavewatch/). This component acts as CRON to extract data with periodic interval and manage some API verbs. | prod | private | Python, Dockerfile |
| **happy-rules-engine** | An dedicated [Drools engine](https://www.drools.org) implementation.  This component acts as CRON to compute forecasts data every 6 hours.| staging | private | Java, Dockerfile |
| **happy-rules** | A set of dedicated rules to spot wave forecasts. | staging | private | Java, Dockerfile |
