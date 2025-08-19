# Software Projects

---

## Audit Data Automation

As the volume and complexity of audit data at ARPANSA (Australian Radiation Protection and Nuclear Safety Agency) increased, traditional Excel-based workflows became inefficient and unsustainable. The audit files were often unstructured, with inconsistent formats, complex columns, and data that was difficult to interpret or analyse effectively.

This application server addresses these challenges by:
* Directly transforming the traditional Excel worksheets into a normalised MySQL database schema using simple RESTful API calls
* Automatically generating IMRT and 3DRT auditing graphs to visualise data distributions for further analysis

#### Data Normalisation
<img src="images/full.png?raw=true"/>

#### Data Visualisation
<img src="images/fig-12.png?raw=true"/>
<!-- <div style="height: 30px;"></div> -->
<img src="images/fig-34.png?raw=true"/>


[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Django-white?logo=django)](#) [![](https://img.shields.io/badge/MySQL-white?logo=mysql)](#) [![](https://img.shields.io/badge/Docker-white?logo=docker)](#) [![](https://img.shields.io/badge/Bash-white?logo=gnubash)](#) [![](https://img.shields.io/badge/Matplotlib-white?logo=matplotlib)](#)
[![](https://img.shields.io/badge/NumPy-white?logo=numpy)](#) [![](https://img.shields.io/badge/pandas-white?logo=pandas)](#)


[View code on GitHub](https://github.com/MEICHENLIN/arpansa-audit-automation)

---

## Tweet Sentiment Pipeline

During the COVID-19 pandemic, Australian residents were ordered into lockdown, and a large proportion of public concern focused on the economic impact the pandemic would have. In response, the government introduced several economic initiatives, such as JobSeeker and JobKeeper payments, to provide financial support for residents.

The project investigates the following topics:
* Observing whether tweets mentioning #jobseeker and #jobkeeper show an overall positive or negative inclination using a sentiment analysis tool, [VADER-Sentiment](https://github.com/cjhutto/vaderSentiment), which is specialised for social media
* Inferring which industries most benefited from these economic schemes by aggregating sentiment data for each major city and comparing it with a labour market dataset
* Analysing how public attitudes towards the initiatives changed over time by aggregating historical sentiment across different time periods


#### Data Flows
1. Collect live and recent tweets using Twitter Search/Stream APIs in Python
2. Enrich the tweets using a Python-based sentiment analysis library
3. Store processed tweets in distributed CouchDB nodes
4. Visualise the tweets on a dashboard implemented with Node.js, Express and Bootstrap


<img src="images/data-flow.png?raw=true"/>

#### Automated Cloud Deployment
* Using Ansible playbook to run Docker containers

<img src="images/deployment.png?raw=true"/>

#### Dashboard Visualisation
* Time-based vs. location-based sentiment analysis

<img src="images/sentiment.png?raw=true"/>


[![](https://img.shields.io/badge/Python-white?logo=Python)](#) [![](https://img.shields.io/badge/Node.js-white?logo=nodedotjs)](#) [![](https://img.shields.io/badge/Express-white?logo=express)](#
) [![](https://img.shields.io/badge/Bootstrap-white?logo=bootstrap)](#) [![](https://img.shields.io/badge/CouchDB-white?logo=apachecouchdb)](#) [![](https://img.shields.io/badge/Ansible-white?logo=ansible)](#) [![](https://img.shields.io/badge/Docker-white?logo=docker)](#) [![](https://img.shields.io/badge/Bash-white?logo=gnubash)](#) [![](https://img.shields.io/badge/NumPy-white?logo=numpy)](#) [![](https://img.shields.io/badge/pandas-white?logo=pandas)](#)

[View code on GitHub](https://github.com/MEICHENLIN/tweet-sentiment-pipeline)

---
