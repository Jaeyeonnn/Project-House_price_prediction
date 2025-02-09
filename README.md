# Real Estate Price Prediction

## Project Objective
- The goal of this project is to develop a model that predicts real estate prices in Seoul using transaction data from the past 10 years (from January 2014 to April 2024). Additionally, a web page will be created to display the predictions.

## Project Environment
- Python 3.10.13
- Node.js 20(lts)

## Project Structure
```
.
├── seoul_real_estate
│   ├── 2014매매.csv
│   ├── ~
│   └── 2024임대.csv
├── frontend
│   ├── app
│   │   ├── module
│   │   │   └── openstreetmap.js
│   │   ├── layout.js
│   │   └── page.js
│   └── package.json
├── django
│   └── real_estate
│       ├── config
│       ├── model
│       │   └── model.h5
│       ├── api
│       └── manage.py
├── preprocessing.ipynb
├── README.md
└── requirements.txt
```

## Pre-requisite 
1. Install Python 3.10.13 and Node.js 20 (LTS)
2. Install required libraries using requirements.txt:
```bash
pip install -r requirements.txt
```
3. Install necessary libraries for the frontend:
```bash
cd frontend
npm install
```
4. Run the Django server:
```bash
cd django/real_estate
python manage.py runserver
```
5. Build and run the frontend server:
```bash
cd frontend
npm install
npm run build
npm run start
```

## Features
- The system predicts real estate transaction prices based on the address input by the user ("administrative district road name address").
- The system displays the input address on the map.
- The predicted transaction price is displayed in a chart.

![image](/public/Animation.gif)

## Datasets
- National Statistical Portal Local Indicators 국가통계포털 지방지표(2014~2023)
- Ministry of Land, Infrastructure, and Transport Real Transaction Price Disclosure System 국토교통부 실거래가 공개시스템(2014~2024)
- Spatial Convergence Big Data Platform Apartment Information 공간융합 빅데이터 플랫폼 아파트 기준정보(2024.02)
