# 📈 BigsCoin  
Hello! Welcome to the 14th Tobig's Conference.  

Our project title is **Bigscoin**.

**Bigscoin** provides users with personalized Bitcoin pattern notifications and interpretable prediction services.

To add explainability and reliability to the prediction of deep learning models which are considered black boxes,

we developed a visualizing system that allows you to see **Bitcoin charts patterns and price predictions** at a glance using XAI techniques.

[![googledrive](https://img.shields.io/badge/report-Link-blue)](https://github.com/ToBigs1617-TS/Bigscoin/files/9138835/Bigscoin.pdf)
<br>  

**14th Tobig's TimeSeries and Explainable AI Conference**  

<p align="center"><img src="https://user-images.githubusercontent.com/72960666/179309070-5bd34ff4-0d45-4dca-89d3-207c59c07161.png"></p>


## Classification
Coin investors often set up investment strategies by referring to the candlestick chart patterns.  

Among the chart patterns, five most observed patterns in coin charts are as follows.  
<p align="center"><img src="https://user-images.githubusercontent.com/72960666/179292406-5e47a37c-cb4c-41a5-894f-b15d8ddb5e5d.png"></p>

But the problem is that **monitoring chart patterns all day long is time consuming and labor intensive**.  
In addition, traditional chart pattern recognition services are not clear and trustworthy  
because the decision making process is impenetrable.  

To address this inconvenience, we used **Conv2d-based model combined with Grad-Cam** in our real-time chart pattern alert service.  

### Data   
- Crawling high, low, market and closing price in 5 minute candlestick chart using "pyupbit" package [August 2017 ~ May 2022]  
- Transforming price data into candlestick chart images as model input   
- Labeling image data into 5 different chart patterns    

### Model  
We utilized **Grad-Cam** to visually interpret the **Conv2d-based model** output.  
You can see the **why the model chose to make the prediction** by looking at the Grad-Cam results.  
Users can easily figure out whether the pattern classified by the model is trustworthy.  

### Web 
<p align="center"><img src="https://user-images.githubusercontent.com/72960666/179319379-4b9be555-b059-49f2-9a0d-884b5e462401.png"></p>
<p align="center"><img src="https://user-images.githubusercontent.com/72960666/179319381-31e7d716-de2b-43ad-ba0b-85f7dceb89d5.png"></p>

## Regression
Users who receive pattern notifications start to think about their investment strategies,   
especially when they get **triangle patterns** where ups and downs are unpredictable.  
**N-BEATS**, an explainable time series model, can help users establish their strategies in a reliable way.  

### Data   
- Crawling high, low, market and closing price in 5 minute candlestick chart using "pyupbit" package   

### Model  
We use **N-BEATS model**, a deep learning architecture that decomposes its forecast into two distinct components, **trend and seasonality**, to provide explanation in the model.  
**Drop-out** is added to the model to visualize confidence interval for population mean of the predictions.  

### Web  
<p align="center"><img src = "https://user-images.githubusercontent.com/72960666/179319371-873b11e9-87bf-4cd2-88eb-654994356918.png"></p>


## Contributors 🧑‍🤝‍🧑

- Members of [ToBig's (Big Data Analysis & Artificial Intelligence Organization)](http://www.datamarket.kr/xe/) participated in this project.

|Year|Name|Team|Contribution|
|:-----:|:-----:|:-----:|:-----:|
|16th year|[Gwonho Kim](https://github.com/kkhv)|Web Serving|Project Leader, Backend|
|16th year|[Hanna Park](https://github.com/hanna56)|Web Serving|Frontend & Backend|
|16th year|[Yoone Kim](https://github.com/yoonene)|Web Serving|Frontend & Backend|
|16th year|[Jooho Kim](https://github.com/Jooho-Git)|Regression|N-BEATS Visualization & Model Tuning, Data Augmentation|
|17th year|[Hyuntai Kim](https://github.com/hyuntai97)|Regression|DeepAR, N-BEATS, Informer Modeling & Experiments|
|17th year|[Sanyoon Kim](https://github.com/tkddbs0411)|Regression|ARIMA Modeling & DeepAR Tuning|
|16th year|[Yerim Lee](https://github.com/YerimLee00)|Classification|Classification Modeling & Grad-CAM Visualization, Presentation|
|17th year|[Seyeon Rha](https://github.com/seyeonrha)|Classification|Experiments|
|17th year|[Heonwoo Yoo](https://github.com/yhw4343)|Classification|Domain Knowledge & Data Inspection|

