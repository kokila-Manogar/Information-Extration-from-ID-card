## Overview
This is a simple image classification Flask app trained on the top of Keras API. The trained model (`app/model/model.h5`) takes an image (Indian Paper Currency) as an input and predict the class of image from __10, 20, 50, 100, 200, 500, 2000__ denomination.

## Motivation
What could be a perfect way to utilize unfortunate lockdown period? Like most of you, I spend my time in cooking, Netflix, coding and reading some latest research papers on weekends. The idea of classifying indian currency struck to me when I was browsing through some research papers. I couldn't find any relevant research paper (and of course dataset!) associated with it. And that led me to collect the images of Indian currency to train a deep learning model using [this](https://github.com/hardikvasa/google-images-download) amazing tool.

## Technical Aspect
This project is divided into two part:
1. Training a deep learning model using Keras. (_Not covered in this repo. I'll update the link here once I make it public._)
2. Building and hosting a Flask web app on Heroku.
    - A user can choose image from a device or capture it using a pre-built camera.
    - Used __Amazon S3 Bucket__ to store the uploaded image and predictions.
    - Used __CSRF Token__ to protect against CSRF attacks.
    - Used __Sentry__ to catch the exception on the back-end.
    - After uploading the image, the predictions are displayed on a __Bar Chart__.

## Installation
The Code is written in Python 3.7. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```

## To Do
1. Convert the app to run without any internet connection, i.e. __PWA__.
2. Add a better vizualization chart to display the predictions.


## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://keras.io/img/logo.png" width=200>](https://keras.io/) [<img target="_blank" src="https://flask.palletsprojects.com/en/1.1.x/_images/flask-logo.png" width=170>](https://flask.palletsprojects.com/en/1.1.x/) [<img target="_blank" src="https://number1.co.za/wp-content/uploads/2017/10/gunicorn_logo-300x85.png" width=280>](https://gunicorn.org) [<img target="_blank" src="https://www.kindpng.com/picc/b/301/3012484.png" width=200>](https://aws.amazon.com/s3/) 

[<img target="_blank" src="https://sentry-brand.storage.googleapis.com/sentry-logo-black.png" width=270>](https://www.sentry.io/) [<img target="_blank" src="https://openjsf.org/wp-content/uploads/sites/84/2019/10/jquery-logo-vertical_large_square.png" width=100>](https://jquery.com/)


## Credits
- [Google Images Download](https://github.com/hardikvasa/google-images-download) - This project wouldn't have been possible without this tool. It saved my enormous amount of time while collecting the data. A huge shout-out to its creator [Hardik Vasa](https://github.com/hardikvasa).
