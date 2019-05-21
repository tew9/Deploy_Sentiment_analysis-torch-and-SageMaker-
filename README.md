# Deploy_Sentiment_analysis-torch-and-SageMaker-
This project deployed a sentiment analaysis model 
with a simple cstom website that send a areview to the model 
and the model (hosted through amazon AWS) will do return back the prediction and displays it 
to the user using the created website.


**Creating a Sentiment Analysis Web App
Using PyTorch and SageMaker
Deep Learning Nanodegree Program | Deployment**
________________________________________
Now that we have a basic understanding of how SageMaker works we will try to use it to construct a complete project from end to end. Our goal will be to have a simple web page which a user can use to enter a movie review. The web page will then send the review off to our deployed model which will predict the sentiment of the entered review.
Instructions
Some template code has already been provided for you, and you will need to implement additional functionality to successfully complete this notebook. You will not need to modify the included code beyond what is requested. Sections that begin with 'TODO' in the header indicate that you need to complete or implement some portion within them. Instructions will be provided for each section and the specifics of the implementation are marked in the code block with a # TODO: ... comment. Please be sure to read the instructions carefully!
In addition to implementing code, there will be questions for you to answer which relate to the task and your implementation. Each section where you will answer a question is preceded by a 'Question:' header. Carefully read each question and provide your answer below the 'Answer:' header by editing the Markdown cell.
Note: Code and Markdown cells can be executed using the Shift+Enter keyboard shortcut. In addition,
a cell can be edited by typically clicking it (double-click for Markdown cells) or by pressing Enter while it is highlighted.

**General Outline**
**Recall the general outline for SageMaker projects using a notebook instance.**

1.	Download or otherwise retrieve the data.
2.	Process / Prepare the data.
3.	Upload the processed data to S3.
4.	Train a chosen model.
5.	Test the trained model (typically using a batch transform job).
6.	Deploy the trained model.
7.	Use the deployed model.
For this project, you will be following the steps in the general outline with some modifications.
First, you will not be testing the model in its own step. You will still be testing the model, however, you will do it by deploying your model and then using the deployed model by sending the test data to it. One of the reasons for doing this is so that you can make sure that your deployed model is working correctly before moving forward.
In addition, you will deploy and use your trained model a second time. In the second iteration you will customize the way that your trained model is deployed by including some of your own code. In addition, your newly deployed model will be used in the sentiment analysis web app.

**Dependencies**
1. Make sure you have an access to amazon SageMaker.
2. Most of the frameworks used in this project are already included with SageMaker
3. install them if they’re using SageMaker terminal

**Important Requirements**
pandas
numpy
nltk
beautifulsoup4
html5lib
