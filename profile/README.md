# HappySession

**HappySession** project attempts to provide surfing forecasts for spots in Brittany (and elsewhere).  

![bg9](https://github.com/user-attachments/assets/011d1a5a-71bd-41f4-b326-df7873223fdf)

The **HappySession** service is built around several components:  

| Service | Description | Status | Visibility | Languages |
|---------|:------------|--------|------------|-----------|
| **mongo** | An TLS/SSH secured Docker image of [MongoDB](https://www.mongodb.com). | staging | private | Dockerfile |
| **extractor** | As its name suggests, this component extracts raw data from [NOAA's WW3 model](https://polar.ncep.noaa.gov/waves/wavewatch/).  This component acts as CRON to extract data every 6 hours. | staging | private | Python, Dockerfile |
| **rules-engine** | An dedicated [Drools engine](https://www.drools.org) implementation.  This component acts as CRON to compute forecasts data every 6 hours.| staging | private | Java, Dockerfile |
| **rules** | A set of dedicated rules to spot wave forecasts. | staging | private | Java, Dockerfile |
