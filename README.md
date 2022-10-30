# Drug-Classification-Model-Deployment-Using-Flask-Ngrok
Drug Classification by Supervised Machine Learning Algorithm Random Forest Classifier and Deployment of The Model With Flask-Ngrok.

What is Flask-Ngrok?

A simple way to demo Flask apps from your machine. Makes your Flask apps running on localhost available over the internet via the excellent ngrok tool.

Compatability
Python 3.6+ is required.

We are going to build model and deploy the machine learning model into the Google Colab.

First, we have to build a Machine Learning Model with Random Forest Classifier which we want to deploy in Google Colab, and save that model using pickle.

Now we have the pickle file with the name ‘model.pkl’.

Deployment Level :

In the new python file first of all we have to mount our Google Drive Account.

We will install the flask-ngrok using the following command

!pip install flask_ngrok

Following that we will install ngrok via Apt.

Then we connect Ngrok to Google Drive Account.

![IMG_1](https://user-images.githubusercontent.com/116178688/198880013-b94a0612-0c43-4a9c-87bf-7e2ebd52d335.jpg)

Also we will install pyngrok from which ngrok will be imported.

For creating the webserver we need an HTML file

The code for the HTML file named ‘index.html’.

We will create a new folder named ‘templates’ and put our HTML file named ‘index.html’ inside that and make a zip file of this ‘templates’ folder.

After that, we will upload both the files ‘model.pkl’ and ‘templates.zip’ in our Google Colaboratory.

After successfully uploading the files we can go to check the files section for confirmation. It will look like this

![1](https://user-images.githubusercontent.com/116178688/198877483-a697f127-82d4-4b04-9c9c-534fcbc8fbf5.png)

As we have uploaded the zip file and therefore we have to unzip it.

After unzipping we see that a new directory is created in the files section with the name ‘templates’.

![2](https://user-images.githubusercontent.com/116178688/198877540-acc09a06-b178-4d81-ada6-1c3952b2331f.png)

After that, we will import the necessary libraries and run the Flask app.

Here, we will have to use the personal Authtoken for ngrok

![IMG_2](https://user-images.githubusercontent.com/116178688/198879965-7ed39935-da6c-43f9-afb7-3b13b1ab0278.jpg)


After executing the cell we will get a url running http with ngrok.io which remains valid for 6hrs.

When we run the url we get an output as follows

![3](https://user-images.githubusercontent.com/116178688/198877666-2d06f6a2-23f0-4407-97f5-43814af2c09e.JPG)


When we click on the ngrok.io file we will get directed to the webpage as follows in which we can feed the values and get the predictions.


![C-0](https://user-images.githubusercontent.com/116178688/198877685-0c51f626-e0fd-4dca-a140-038529b08d28.JPG)


Hence, we finally deployed our Machine Learning Model using Google Colab successfully.


Key Note:

In IMG_1 and IMG_2 it shows the personal Authtoken for ngrok will be diiferent for each person.

To get the personal Authtoken for ngrok one has to open an account on ngrok.com



