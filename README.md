# Welcome to Intro to ML for everyone! 🤖📊✨

![welcome](https://github.com/ccstan99/introML/blob/main/images/welcome.png?raw=true)

We're your hosts, [ChengCheng Tan](https://www.linkedin.com/in/cheng2-tan/) and [Philippa Burgess](https://www.linkedin.com/in/philippaburgess/)!

Our goal is to share how easy it is to get started with ML. Thanks to awesome resources online and the amazing advancement in tools, anyone can get started with ML!

## Intro to Machine Learning - Agenda 🤖

Here's what we will cover today:

1. What is ML? 🤔💭🤖
2. Data prep 🐧🐧🐧
3. Training your model 🏋🏻‍♀️💪
4. Model evaluation 📊🔍👀
5. Next steps... and more! 🏆✨

In this notebook, we'll walk through a high level overview of how ML models *generally* work - esp. what are the different steps we take in order to build a model. This lays the foundation for talking about ML, key terms, and how to help you learn!

Hopefully at the end, you are able to better understand how models are made, and the vocabulary used in ML and AI, and have a little more confidence to start your ML journey 🏆

## What is machine learning? 🤔💭 🤖

Machine learning is the process of teaching a computer to learn patterns from data and then to apply those patterns to make preditions on new data. In traditional programming, you write rules to tell the computer exactly what to do. For example, if you want to write a program that converts temperature from Celsius to Fahrenheit, you would write a function that computes the following equation:

<center>
<img src="https://github.com/ccstan99/introML/blob/main/images/io_programming.png?raw=true" width="40%"/>
<img src="https://github.com/ccstan99/introML/blob/main/images/io_ML.png?raw=true" width="40%"/>
</center>

But in ML, instead of writing the rule, you provide the computer a lot of examples of input data as well as the desired output, say pairs of celsius and fahrenheit data. Then let the computer learn the rule itself.

This particular case is very simple but imagine if you had to write a program to recognize cat images or generate languages. You'd have to write many rules. You can see how the list of rules and their exceptions could grow very quickly.

ML is ideal for these types of problems, where you have lots of data that have complex relationships that would be very difficult for humans to manually create rules for.

* Image and video recognition
* Language generation
* Recommendations
* etc

If you're interested in a more in depth look at these concepts - check out the [Intro to ML](https://developers.google.com/machine-learning/intro-to-ml) course on the Google developer site!

## ML Model and Dataset 📊

Now that you've seen the difference between ML and traditional programming, let's get started on programming, or training, our own model!

For this workshop, we'll be using the [Palmer's Penguins](https://allisonhorst.github.io/palmerpenguins/articles/intro.html) dataset to train a decision forest model to predict the penguin species.

<center><img src="https://allisonhorst.github.io/palmerpenguins/reference/figures/lter_penguins.png" width="100%"/></center>

A decision tree is an algorithm that learns by splitting the data into smaller and smaller subsets. The splits are determined by how well each subset helps to predict the desired outcome. Here's a simple decision tree for predicting different types of penguins! Let's presume class 0 is Adelie, class 1 is Gento, and Type 2 is Chinstrap.

<center><img src="https://github.com/ccstan99/introML/blob/main/images/decision_tree.png?raw=true" width="50%"/></center>

Decision Forests (`DF`) are a large family of Machine Learning algorithms for
supervised classification, regression and ranking. As the name suggests, DFs use
decision trees as a building block.

<center><img src="https://github.com/ccstan99/introML/blob/main/images/decision_forest.png?raw=true" width="100%"/></center>

[TensorFlow Decision Forests (`TF-DF`)](https://www.tensorflow.org/decision_forests) is a library for the training Decision Forest models.

## Notebook

Try out some code by running the [Intro to ML Colab Notebook](./WTM23_introML.ipynb)