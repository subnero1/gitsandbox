## SECTION 1 : PROJECT TITLE
## Intelligent Patient Responder System

<img src="SystemCode/clips/static/hdb-bto.png"
     style="float: left; margin-right: 0px;" />


## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT
(coming soon)


Using the techniques imparted to us in lectures, our group first set out to build a sizeable knowledge base via conducting an interview and administering a survey. While building the system, we utilized tools such as Java to scrape real time data from HDB website and transform it into a database, CLIPS to synthesize the rule based reasoning process, and Python to integrate it into an easy to use UI for the everyday user. To add icing on the cake, we even hosted the system on a website so that the everyday user can access it through the click of a link.


Our team had an amazing time working on this project, and hope to share our insights with everyone. Despite a focus on BTO flats, we would recommend it for everybody interested in understanding property market trends for residence or investment purposes. There truly are a wide array of factors behind the decision to invest in a property, and we only wish there was more time to work on the scope and scale of the project. 

---

## SECTION 3 : CREDITS / PROJECT CONTRIBUTION

| Official Full Name  | Student ID (MTech Applicable)  | Work Items (Who Did What) | Email (Optional) |
| :------------ |:---------------:| :-----| :-----|
| Yap Jing Yang | A0229976H | Nurse Dashboard front-end, Project Report Writing, Business Video | E0687384@u.nus.edu |
| Francis Tan Wee Meng | A1234567B | Python Coding, MongoDB Deployment, Project Report Writing, Technical Video| XXXXXXXX@u.nus.edu |
| Ramya | A1234567C | MyCroft User Input, Admin Dashboard front-end, Heroku Host Deployment, Project Report Writing, Technical Video   | XXXXXXXX@u.nus.edu |
| Wong DongChen | A0083129E| NLP processing, Project Report Writing, Business Video| XXXXXXXX@u.nus.edu |

---

## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO

[![Sudoku AI Solver](http://img.youtube.com/vi/-AiYLUjP6o8/0.jpg)](https://youtu.be/-AiYLUjP6o8 "Sudoku AI Solver")

Note: It is not mandatory for every project member to appear in video presentation; Presentation by one project member is acceptable. 
More reference video presentations [here](https://telescopeuser.wordpress.com/2018/03/31/master-of-technology-solution-know-how-video-index-2/ "video presentations")

---

## SECTION 5 : USER GUIDE

`Refer to appendix <Installation & User Guide> in project report at Github Folder: ProjectReport`

### [ 1 ] To run the system using iss-vm

> download pre-built virtual machine from http://bit.ly/iss-vm

> start iss-vm

> open terminal in iss-vm

> $ git clone https://github.com/telescopeuser/Workshop-Project-Submission-Template.git

> $ source activate iss-env-py2

> (iss-env-py2) $ cd Workshop-Project-Submission-Template/SystemCode/clips

> (iss-env-py2) $ python app.py

> **Go to URL using web browser** http://0.0.0.0:5000 or http://127.0.0.1:5000

### [ 2 ] To run the system in other/local machine:
### Install additional necessary libraries. This application works in python 2 only.

> $ sudo apt-get install python-clips clips build-essential libssl-dev libffi-dev python-dev python-pip

> $ pip install pyclips flask flask-socketio eventlet simplejson pandas

---
## SECTION 6 : PROJECT REPORT / PAPER

`Refer to project report at Github Folder: ProjectReport`

#### Sections for Project Report 

- Executive Summary
- Business Problem Background	
    - Problem Statement	
    - Market Research	
    - Product Solution	
      - Product Objectives
      - Project Scope and Deliverables
    - Project Team
- Product Design	
  - Main Features	
  - Process Flow	
  - System Highlights	
    - Voice Activation
    - Language Processing
    - Data collection and relearning	
- System Modeling
  - Technical Flow
- System Development & Implementation	
  - User Interface
    - MyCroft (User input)
    - Nurse Station Panel
    - Nurse Activity Manager(Admin Dashboard)	
  - Backend Processing
    - NLP Classification of request
    - Dynamic Rule-Based Sorting	
  - Data Management
    - Storage of data
    - Data Interaction	
  - System Limitations	
- System Performance & Evaluation
  - Performance
  - Challenges
  - Future Developments
    - Better Data Acquisition
    - Sentiment Sensing in Voice Identification	

---
## SECTION 7 : MISCELLANEOUS

`Refer to Github Folder: Miscellaneous`

### Files needed for NLP pre-processing
  - Symptom-severity_training_data.csv
  - patient_input.txt

