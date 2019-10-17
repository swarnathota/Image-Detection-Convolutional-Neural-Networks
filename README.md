# Photography Learning App

## Why this project

I am a photographer and I enjoy photography. When I started learning photography, I found it was difficult to get judgement on the photos whether they are good or bad with aesthetics. I uploaded my photography pictures to famous photography websites and wait for the likes or comments, that was the only judgment I or anyone could get. It is a time consuming for the photography amateurs. A thought flashed in my mind, what if the famous photography blogs, such as 500px or flicker, has a web application that could decide the photo is good or bad instantly when it is uploaded. This project could be applied to various image analyses across diverse fields.

## How the project is made

#### Getting and cleaning  data

**.** BeautifulSoup and Selenium are used for webscraping

**.** Images were collected from 500px from from two categories editer's choice and popular photos respectively for **Good** category and **bad** category photos were taken from facebook pages. 

**.** Collected a total of 18,000 pictures and cleaned manually and categorized into Good and Bad classes.

**.** Code to this section is in [Web_scraping_images.ipynb](http://localhost:8888/notebooks/swarna-DS/Metis/Metis_BC/Challenges/Project5/Project5_github/Web_scraping_images.ipynb) 

#### Pre-processing and modeling

**.** Images were split into train = 70%, validation = 15% and test = 15% sets.

**.** Image proceesing and modelig is performed  on AWS using Tensorflow (keras and CNN).

**.** Feature extracted using pretrained VGG16 and used as input to the fully connected network.

**.** Fine tune the model to improve accuracy

**.** Code to this section is in [Project5.ipynb](http://localhost:8888/notebooks/swarna-DS/Metis/Metis_BC/Challenges/Project5/Project5_Metis/Project5.ipynb)

#### load and test the model

**.** Accuracy is measured on test set 

**.** Flask app is  launched using jupyter notebook and tested on different photographs that are not part of test set.

**.** Model is able to detect composition, color balance, greyscale photos and color balance

**.** Code to this section is in [Project5.ipynb](http://localhost:8888/notebooks/swarna-DS/Metis/Metis_BC/Challenges/Project5/Project5_Metis/Project5.ipynb)

## What needs to be improved

**.** This model is unable to detect story telling pictures, this can be improved by adding these pictures into the model and train further.

**.** I made this project as  binary classification model (Good and bad images) which can be made into multi class by categorising the pictures different classes and run the model.

## Uses of image analysis

 Image analyses can also be applied to related fields such as:

**.** Immuno-histopathology image processing to identify the different stages of cancer.

**.** In fashion industry,  where image processing is used to automate search for designer outfits.

**.** Security industry where image processing is used for face recognition.





