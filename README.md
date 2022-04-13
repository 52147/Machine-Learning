# Machine-Learning

## Introduction to Artificial Intelligence and Machine Learning
![image](https://user-images.githubusercontent.com/79159894/163271163-8ce4c67b-0caa-45b6-9a08-01ee49075b07.png)

### Artificial Intelligence
Artificial Intelligence is a branch of computer science dealing with the simulation of intelligent behavior in computers. Machines mimic cognitive functions such as learning and problem solving. 

ex: Any program that can sense, reason, act, and adapt.
### Machine learning
Machine learning is the study of programs that are not explicitly programmed, but instead these algorithms **learn patterns from data.** 

### Deep learning
Deep learning is a subset of machine learning in which **multilayered neural networks** learn from vast amounts of data.   
Neural Networks, and Deep Learning in particular, are the leading algorithms that power **Computer Vision.**

## History of AI 

Turing Test:
- In 1950, Alan Turing developed the Turing test to test a machine's ability to exhibit intelligent behavior. 
- Alan Turing's test has served as a foundational threshold for artificial intelligence.

AI has experienced cycles of AI winters and AI booms. 

AI solutions include speech recognition, computer vision, assisted medical diagnosis, robotics, and others.   


Why did AI flourish so much in the last years?
Faster and inexpensive computers and data storage
- Modern AI 
Factors that have contributed to the current state of Machine Learning are:  
 - bigger data sets, 
 - faster computers, 
 - open source packages, 
 - and a wide range of neural network architectures.   

## Machine Learning Workflow 
- The machine learning workflow consists of: 

  - 1. Problem statement

  - 2. Data collection

  - 3. Data exploration and preprocessing
    - Determine how to clean your data such that you can use it to train a model 

  - 4. Modeling

  - 5. Validation

  - 6. Decision Making and Deployment

## This is a summary of the common taxonomy for data in open source packages for Machine Learning: 
![image](https://user-images.githubusercontent.com/79159894/163274903-a9e6859c-f789-4f7f-910c-c342c2cca1fa.png)

- target: category or value you are trying to predict

- features: explanatory variables used for prediction

- example: an observation or single data point within the data

- label: the value of the target for a single data point


## two types of Machine Learning
- Let's first go over the type of datasets that each is going to need. 

- There are supervised learning and unsupervised learning.
![image](https://user-images.githubusercontent.com/79159894/163275080-0c6126f6-2ff5-47aa-8792-57c2cea63a47.png)

### 1. supervised learning
- For supervised learning, we will have a target column or labels similar to what we just saw with the email spam and iris flower classification examples, and then for unsupervised learning on the other hand we will not have a target column. 
- How this comes into play will make more sense in just a second. 
- The goal for supervised learning is going to be able to **predict that label.**
- Is it spam or is it not spam? 
- Is it's versicolor or another one of the different flower species? 

- An example of supervised learning is fraud detection. 
- We may have a large dataset where we have labels of either this transaction is fraud and this transaction is not fraud. 
- We would learn from all the features related to fraud detection and be able to predict as new credit card transactions come in whether those are fraud or not fraud. 

### 2. unsupervised learning
- For unsupervised learning, the goal is going to be to find an underlying structure of the dataset without any labels, and this will be clear with our examples. 
- For unsupervised learning, an example would be customer segmentation. 
- For this, you can think about customer segmentation to find similar groupings within your dataset for a marketing campaign, you have this e-commerce data and you want to separate them out into groups in order to target them accordingly. For unsupervised learning, there's going to be no right or wrong answer. 
- So the user will need to test different models and see which results tend to make the most sense. 
- We'll get into this we have an entire lecture where we discuss different algorithms and techniques found to accomplish this task. 


### common Machine Learning problem : detecting fraud
- So suppose you wanted to identify fraudulent credit card transactions, detecting fraud is going to be a common Machine Learning problem, - You can define your features to be 
  - transaction time, 
  - transaction amounts, 
  - transaction location, 
  - category of purchase. 
- Combining all of these features together, we should be able to predict in the future with transaction time, the amount location in the category of purchase, whether there's unusual activity, and whether this transaction is fraud versus not fraud. 

![image](https://user-images.githubusercontent.com/79159894/163274754-815bade7-9f77-4fc4-9ab5-39a325410115.png)



### Machine Learning limitation
- Now, defining features in an image, on the other hand, is a much more difficult and involved task and has been a defining issue of the limitations of our Traditional Machine Learning techniques that Deep Learning has now done a good job of addressing. 
- So suppose you want to determine if an image is a cat or a dog, so what features should we use? 
- For images, the data is taken as numerical data to reference the coloring of each individual pixel within our image. So a pixel then could be used as a feature. 
- So we saw the features before in our dataset. 
- But if you imagine even a small image will have 256 by 256 pixels, which will come out to over 65,000 pixels. 
- Sixty five thousand pixels mean 65,000 features which is a huge amount of features to be working with. Another issue is that using each pixel as an individual, you lose the spatial relationship to the pixels around it. 
- In other words, the information of a pixel makes sense relative to its surrounding pixels. 
- So you have the different pixels that make up the nose perhaps, or the different pixels that make up the eyes, and then separating that out according to where they are in relation to the face, so on and so forth. 
- This is where Deep Learning can come in.
- Deep Learning techniques will give you the capability to learn these features on its own and combine these pixels to define these spatial relationships.

# Deep Learning


- Deep learning is going to be Machine Learning that involves using very complicated models called **deep neural networks.**
- Deep Learning is a subset of Machine Learning. 
- So then the models themselves will be able to determine the best representation of our original data. 
- In classic Machine Learning, humans have to come up with these features and this will allow us to solve complex problems such as what we just saw with the image classification. 
- Deep Learning is the cutting edge and is where most of Machine Learning research is focused as blown away the performance of other algorithms when you're **dealing with larger datasets.** 
- But it is very important to note that you'll often be working with **smaller datasets, and standard Machine Learning algorithms will often perform significantly better than working with Deep Learning techniques**. 
- Also, if the data is changing a lot over time and you don't have a steady dataset, again Machine Learning will probably do a better job of actually being able to have better performance over time. 


## Difference between Machine Learning and Deep Learning
- So let's briefly discuss some differences between the classic Machine Learning Techniques and Deep Learning. So as discussed in the Classical Machine Learning model, we are going to have to define these features ourselves a priority before we feed the data to our actual model, so determining the features that make up the nose, the eyes, so on and so forth. 
- We can then use the features and include them in a Machine Learning algorithm. If a data scientist is lucky, he may be able to guess good features, but this is a really challenging to do well. 
- Then they can use that to predict that this is a picture of Arjun. Now Deep Learning will combine this two-step process. The neural network receives these pixels of an image as an input. 
- The neural network learns how to extract these features that are meaningful from the image by combining them together in different complex combinations. 
- Now, these features may not always make much sense when we try to interpret them in these intermediate layers. But ideally, they will first highlight edges and then combine those edges to make up shapes like nose, eyes, lips. 
- But whether or not the intermediate steps are interpretable, they can be very useful for completing tasks such as image classification and coming up with the intermediate feature engineering steps, and then eventually predicting Arjun. 


## Artificial Intelligence Application
- Now let's briefly highlight the degree to which artificial intelligence is already present in our day-to-day lives.

### AI in transportation
- Let's think about artificial intelligence in regards to our personal transportation. 
- So figuring out the shortest distance between two points is a classic problem since before the introduction of artificial intelligence. -- And today, we also add the complexity of knowing traffic information or predicting it based on historical data and weather conditions, so on and so forth. 
#### Navigation:
- Google and Waze have been able to incorporate all these factors to constantly improve their algorithm for fastest means of getting from point A to point B.
#### ride-sharing
For ride-sharing, Uber and Lyft is able to price their rides according to supply and demand, instead of a flat rate. And the supply and demand can be updated in real-time using artificial intelligence techniques.
### AI in transportation social media industry
- We see artificial intelligence in the booming social media industry.
#### Audience
- Social networking is one of the newest businesses that is exploring artificial intelligence. 
- Artificial intelligence can now identify content relevant to an individual, recommendations for people or groups to connect with targeted advertisement delivery. 
#### Content
- We also see image recognition and sentiment analysis to ensure that the content is appropriate mood that we want to be served. 
- Artificial intelligence has been successful at identifying the sentiment of content, such as the review of a restaurant.
-  Is that a positive or negative sentiment?
### AI in transportation in daily life
#### natural language
- We have in our daily life. We think about 
processing. 
- Today, we have products, like Siri on our phones or **Alexa** in our homes that can **recognize our voice and answer questions** or do tasks for us.
#### object detection
- With object detection, this is important for self-driving cars. Facebook is able to recognize faces and pictures and suggest who that person is so photos can be easily shared with friends.

### AI in computer vision
- And with computer vision, when we talked about this pretty thoroughly throughout, we saw how deep learning is proven to work for image classification, able to outperform humans and many image classification tasks. 
- And today, we see it doing live detection, which is going to be very important as we try to roll out self-driving cars.

- And moving into the future, how we can use this for things such as abandoned baggage detection.
  - For example: abandoned baggage detection:
    - We can automatically detect when baggage has been left unattended, and this can potentially save lives.

    - And this system is going to rely on **cutting-edge object detection ran in real time.**
