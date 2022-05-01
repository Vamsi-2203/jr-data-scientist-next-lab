# Evaluation-1
```
Name: Manaal Sxaena
Applied position: Jr.Data Science
Company: Next Growth Labs
```
## Installing
![](https://forthebadge.com/images/badges/made-with-python.svg)

The Code is written in Python 3.10. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```

# Part 1

## Question-1
1. Write a regex to extract all the numbers with orange color background from the below text in italics.
```python
{"orders":[{"id":1},{"id":2},{"id":3},{"id":4},{"id":5},{"id":6},{"id":7},{"id":8},{"id":9},{"id":10},{"id":11},{"id":648},{"id":649},{"id":650},{"id":651},{"id":652},{"id":653}],"errors":[{"code":3,"message":"[PHP Warning #2] count(): Parameter must be an array or an object that implements Countable (153)"}]}
```
Sol: Wrote a simple regex code to solve the given problem, To see the code solution check [(Part 1) Question-1](https://github.com/trickster-00/Evaluation-1/blob/d1673b5ef76c904c573bb6c7048b60a94a8dc211/(Part%201)%20Question-1.ipynb).

## Question-2
2. There are times when a user writes Good, Nice App or any other positive text, in the review and gives 1-star rating. Your goal is to identify the reviews where the semantics of review text does not match rating. 

Your goal is to identify such ratings where review text is good, but rating is negative- so that the support team can point this to users. 

Deploy it using - Flask/Streamlit etc and share the live link.

Sol: Analysed data to figure out users who give low rating but leave good review. Built a Streamlit web application that takes data as input and shows users that displays incorrect rating and let's users download the dataset. Deployed the application on Streamlit share.

Analysis - [(Part 1) Question-2](https://github.com/trickster-00/Evaluation-1/blob/cb062d9da83b1d6e29735b95c822569dd8154a7f/(Part%201)%20Question-2.ipynb)

Web Application- [App](https://github.com/trickster-00/Evaluation-1/blob/cb062d9da83b1d6e29735b95c822569dd8154a7f/app/main.py)

### Demo - 
Working link - [https://share.streamlit.io/trickster-00/evaluation-app/main/main.py](https://share.streamlit.io/trickster-00/evaluation-app/main/main.py)
![](https://github.com/trickster-00/Evaluation-1/blob/cb062d9da83b1d6e29735b95c822569dd8154a7f/img/3757f02a-1ce9-4edd-abd9-ac31035cecb7.png)

## Question-3
3. Ranking Data - Understanding the co-relation between keyword rankings with description or any other attribute. [Here’s the dataset](https://github.com/trickster-00/Evaluation-1/blob/cb062d9da83b1d6e29735b95c822569dd8154a7f/data/browser_rankings_data.csv).

Sol. To better understand co-relation among variables, performed corelation analysis using Spearman rank correlation coefficient amongst the variable to derive results, To check [(Part 1) Question-3](https://github.com/trickster-00/Evaluation-1/blob/cb062d9da83b1d6e29735b95c822569dd8154a7f/(Part%201)%20Question-3.ipynb)

### Suggested questions:
```
1. Is there any co-relation between short description, long description and ranking? Does the placement of keyword (for example - using a keyword in the first 10 words - have any co-relation with the ranking)?

A. The co-relation between short description, long description and ranking very minimal when compared other features. But, as per Spearman Rank Correlation the relation between Long/Short discription is a Non-monotonic relation which suggests that increase or decrese of one variable can implement of increment or decrement of other. Here adding a keyword in the first 10 words may increse the corelation with the ranking. It's safe to say that 'discriptions' don't carry a huge impact on 'Ranking' compared to others.
```

```
2. Does APP ID (Also known as package name) play any role in ranking?

A. Comparing to all features 'APP ID' is highly correlated to 'Ranking', according to Spearman rank correlation coefficient it has 'Weak monotonically increasing relationship' which proves that if either of variable increases then other will increse as well. 'APP ID' plays an important part in deciding ranking.
```

```
3. Any other pattern or good questions that you can think of and answer?

A. A question arises " Why is 'APP ID' so highly co-related to 'Ranking' than other features? " The answer to this might be, it's usage of 'keywords' in it. App ID uses keywords a lot more than the discriptions, that could be one of the reasons for it's high correlation rate.
```

# Part 2

## Question-1
1. Check if the sentence is Grammatically correct: Please use any pre-trained model or use text from open datasets. Once done, please evaluate the English Grammar in the text column of the dataset. [DataSet Link](https://github.com/trickster-00/Evaluation-1/blob/827108220770844b8435b13cd7059dc4531d104f/data/review_data.csv)

Sol. Built a function using Language Tool and TextBlob modules that can take text as input and run tests to check if the sentence is gramatically correct, then applied the function on given dataset. Generated a new dataset with all gramatically incorrect sentences. To check code solution see [(Part 2) Question 1](https://github.com/trickster-00/Evaluation-1/blob/22b5d044946f7fd11643c41fb19c5789cf83da17/(Part%202)%20Question-1.ipynb)


## Questions

1. Write about any difficult problem that you solved. (According to us difficult - is something which 90% of people would have only 10% probability in getting a similarly good solution). 

A. During a project where I given a task to build a machine learning model that predicts if a website domain is real or malicious, the model was also supposed to be deployed as an API which takes user input of an URL, The deployment process was particularly difficult as model had many features and data preprocessing was to be done on each feature to match user's input. After alot of time & effort we managed to get the work done.

2. Formally, a vector space V' is a subspace of a vector space V if
-  V' is a vector space
-  every element of V′ is also an element of V.

Note that ordered pairs of real numbers (a,b) a,b∈R form a vector space V. Which of the following is a subspace of V?

-  The set of pairs (a, a + 1) for all real a
-  The set of pairs (a, b) for all real a ≥ b
-  The set of pairs (a, 2a) for all real a
-  The set of pairs (a, b) for all non-negative real a,b

Answer - The set of pairs (a,b) for all real a >= b 
