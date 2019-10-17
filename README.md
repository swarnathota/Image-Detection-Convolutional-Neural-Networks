# Photography Learning App

## Why this project

I enjoy pjotography and when I started learning photography, I found it was difficult to get judgement on the  photos (atleast good or bad) instantly. I upload pictures to any famous photography websites and wait for the likes or comments, that was the only judgment one could get. It is painful  and time consuming for the photography amateurs. What if the famous photography blogs, such as 500px or flicker, has a web application that could decide the photo is good or bad instantly whaen it is uploaded.

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

**.** flask app is  launched using jupyter notebook and tested on different photographs that are not part of test set.

**.** Code to this section is in [Project5.ipynb](http://localhost:8888/notebooks/swarna-DS/Metis/Metis_BC/Challenges/Project5/Project5_Metis/Project5.ipynb)

## Uses of image analysis

With this experience I can also analyse images related to other areas such as:

**.** Cancer histopathology image processing to identify the stages of cancer.

**.** In fashion industry  where image processing is used to automate search for designer outfits.

**.** Security inductry where image processing is used for face recognition.





