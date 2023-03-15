``` 
SENTIMENT ANALYSIS FOR AMHARIC LANGUAGE 
```
<i>(Fundamentals of Machine Learning class project. <img src="./logo.jpg" alt="logo of Debre Birhan University" style="width: 8vh; height: 3vh; border-radius: 2vh;"> )</i>
<hr/> 

## 1. Introduction

### 1.1. General Description

Sentiment analysis is used to analyze raw text to drive objective quantitative results using natural language processing, machine learning, and other data analytics techniques. It is used to detect positive or negative sentiment in text, and often businesses use it to gauge branded reputation among their customers.

Natural language processing (NLP) refers to the branch of computer science—and more specifically, the branch of artificial intelligence or AI—concerned with giving computers the ability to understand text and spoken words in much the same way human beings can.

NLP combines computational linguistics—rule-based modeling of human language—with statistical, machine learning, and deep learning models. Together, these technologies enable computers to process human language in the form of text or voice data and to ‘understand’ its full meaning, complete with the speaker or writer’s intent and sentiment.

NLP drives computer programs that translate text from one language to another, respond to spoken commands, and summarize large volumes of text rapidly—even in real time. NLP also plays a growing role in enterprise solutions that help streamline business operations, increase employee productivity, and simplify mission-critical business processes.

Several NLP tasks break down human text and voice data in ways that help the computer make sense of what it's ingesting. One of these is the ability of the machine to understand natural languages or Natural Language Understanding (NLU).

In this project we will try to build a machine learning model that will perform a sentiment analysis on Amharic language.

### 1.2. Project Justification / Motivation

We are under development of Amharic Book store website. In this website all users will give comments or sentiments on their fillings about the uploaded books. The problem is that authors and administrators of the system needs summarized information about the given sentiments under each book, whether the given comments are positive, negative, neutral and mixed. So, we are motivated to solve this problem.

### 1.3. Technology Used

<ul>
<li><b>TensorFlow: </b>An end-to-end machine learning platform</li>
<li><b>Scikit-learn: </b> A python library that has a collection of machine learning algorithms and datasets</li>
<li><b>Pandas: </b> A python library for reading data from different file format (SV, JSON, etc.).</li>
</ul> 

## 2. Statement Of Problem

### 2.1. Problem Statement

There are a lot of ecommerce websites being launched in Ethiopia. For example, <i>asbeza.net</i> and <i>addismercato.com</i> are the two ecommerce websites. These websites are built to connect shoppers to products or services for trading online. On the most basic level, they provide everything we need for online shopping.

On these sites the buyers/customers leave their review and the services providers/sellers would like to know the popularity of their product or the perception of customers about the products and services.

With hundreds and thousands of reviews posted for every product, doing the analysis is out of question and there is very little done on Natural Language Processing (NLP) on Amharic language or any other Ethiopian language.

## 2.2. Why we choose to do this project

We decided to do this project for two reasons

1. As we have mentioned above e-commerce website that are currently operating and other start ups that want to enter into this market face a serious problem trying to analyze user reviews.

2. We also want to enter into this marker by creating an online book store and we want to develop a model that will make our lives easier. 2. We also want to contribute our share towards natural language processing for Amharic and other Ethiopian languages.

## 3. Objectives

### 3.1. General Objective

The main objective of this project is to build different machine learning models for Amharic sentiment analysis. These models will be used to classify a piece of text written in Amharic language and classify it as positive negative or neutral.

### 3.2. Specific Objective

Our specific objective in doing this project is to accurately identify and categorize the given Amharic sentiments as either positive, negative, or neutral.

## 4. Methodology

### 4.1. Project Development Method

We preferred agile software development model. With Agile Methodologies, designs, code and tests are iteratively implemented and feedback from users is taken into account throughout the process. This makes it easier for us to accommodate changes in requirements that may come up during the project's course of implementation. It facilitates communication between customers/stakeholders and developers and help manage complex tasks that go into sentiment analysis projects.

### 4.2. Data Source

The dataset is based on Twitter data source collected in the months of December 2019 and January 2020, targeting only tweets written in the 'Fidel' script. The dataset is used from another project by group of individuals attempting to build annotation tools and classification models.<i> Yimam, S. M., Alemayehu, H. M., Ayele, A., & Biemann, C. (2020). Exploring Amharic Sentiment Analysis from Social Media Texts: Building Annotation Tools and Classification Models. https://doi.org/10.18653/v1/2020.coling-main.91</i>

The dataset is divided into train and test sets containing 7510 and 930 records respectively. Both sets contain tweet ID, sentiment label and the tweet itself as a column.

### 4.3. Data Preprocessing Technique

The data preprocessing involves the following steps: -

<ul>
<li>Data cleaning</li>
<ul>
<li>Remove null values from dataset</li>
<li>Drop repeated rows (drop rows with similar tweet id)</li>
<li>Remove URL, mentions, emoji and symbols from tweets</li>
<li>Method to normalize character level mismatch such as - In Amharic language there are several characters that sound the same but have different symbol for example ‘ጸሀይ’ and 'ፀሐይ’, ‘አዳም’ and ‘ዓዳም’, therefore, we wrote a function to make them consistent.</li>
</ul>
<li>Tokenization – a way of extracting tokens from the dataset</li>
<li>Sequencing – represent the tweet/string as a number or a sequence of numbers.</li>
</ul> 
After all this steps the data is fed into the machine learning models.

## 5. Implementation

### 5.1. Model Development

We developed three models specifically Artificial Neural Network model, Naïve Bayes model and Support Vector Machines model with the following results: -

<table>
<thead>
<th></th>
<th>Accuracy</th>
<th>Recall</th>
<th>Precision</th>
<th>F1</th> 
</thead>
<tbody>
<tr>
<td>ANN</td>
<td>0.26</td>
<td>-</td>
<td>-</td>
<td>-</td>
</tr>
<tr>
<td>Naïve Bayes</td>
<td>0.23</td>
<td>0.04</td>
<td>0.88</td>
<td>0.07</td>
</tr>
<tr>
<td>SVM</td>
<td>0.51</td>
<td>0.51</td>
<td>0.51</td>
<td>0.07</td>
</tr>
</tbody>
</table>

### 5.2. Result

Although we used Naive Bayes, ANN, and SVM models, SVM provided the best accuracy, but finding data to utilize was challenging due to Amharic's complicated morphology.

The outcome demonstrates that, when compared to other models, the Support Vector Machine (SVM) model produces the best results for Amharic sentiment analysis.

## 6. Recommendation And Conclusion

### 6.1. Recommendation

As Amharic sentimental analysis is new or not well developed point of view in the field, any interested ML engineer can proceed by using our work.

### 6.2. Conclusions

Amharic is one of the low-resource languages. Because of the scarcity of labeled data, it's been quite difficult to make an NLP model for sentiment analysis. Other main point we learned is that the most difficult part of NLP is the data extraction and data cleaning than creating the actual models.


<br/><br/>

### Follow me on:
[LinkedIn](https://www.linkedin.com/in/belay-birhanu-506809207/)
[GitHub](https://github.com/AdgehTech)
[Telegram](https://t.me/adgehTech)
[Gmail](mailto:belaybirhanu407@gmail.com)