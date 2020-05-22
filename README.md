# FIU-Capstone-2020
A senior design capstone project done in conjunction with Charlie Ramirez and Sephora Jean-Mary, two senior Computer Science students at Florida International University (FIU). Mitre team members included Ali Zaidi, Joe Garner, and Naz Haq. 

See below for instructions on how to run the code for this project: 

The purpose of this README is to explain the directory structure for "Code".

Our project "ai for all" is composed of three major parts: 

	1. A Web Scraper, used to collect information from the web. For this project, 
we scraped Amazon.com for information (product title, price, rating, product info, 
number of reviews, etc.) on a variety of products. 

	2. A website, www.itsaiforall.com (alternatively: https://aiforall.herokuapp.com/) 
coded from scratch. In this website, we explain what "ai for all" is all about. While
our project is ultimately a product that a business or consumer can make use of, a large 
part of our project involves TEACHING. When we first accepted this project, it was on the
premise that we would be creating a machine learning lesson for college students all across
the country. While this is a a major part of the project, in time it expanded into something 
much greater. The website serves a great purpose in explaining, teaching, and guiding users
to something they have the option of themselves expanding on.   

	3. A web app, where dynamic content is the key. The website serves its function of teaching
and guiding, while the web app allows for the project to have dynamic visualizations and dynamic content
via the web scraper and "Anvil" working together.

The website and the web scraper directories will be visible once you open the source code folder. 
You will be met with two folders (one for each part) that include the code for that particular part and the relevant user manual and
installation guide. Additionally, you will see a folder titled "anvil web app" which only contains 
a short word document with some of the source code of the forms built on anvil. 
Following is an explanation of the structure of each directory.

Web Scraper
===========

Once you open the web scraper directory, you will be met with a couple of files and folders. The first file
"logs" are some of the sample outputs scrapy saved. These files are mostly irrelevant but I left them in 
so that, if it would be of help, one would be able to see some of the earlier outputs of the scraper. note that
these outputs are from one of the earlier versions of the scraper.  

The "manuals" directory includes two files: our installation guide and our user manual both saved as pdf files.

"ws_seniorproject" contains the scrapy files that allow the scraper to run. The more important files such as 
testfile.py in the spiders subdirectory and items.py are included in this directory.

Thie web scraper directory also includes the configuration file (which should remain untouched) and a results 
json file which shows ~50 sample outputs of the latest version of the scraper. 


Website
===========

The website was coded using standard lanaguages such as html, css, and javascript. The web framework we used was
"Flask" (python as programming language). Flask requires that we have a "static" folder to house javascript/css files
and a "templates" folder to hold our html files. 

Our first folder is the "datasets" folder which holds all the json and csv files we scraped using our web scraper. These
files are called in the website to display their contents (specifically in the "web scraper" page of our website). 

The "manuals" directory includes two files: our installation guide and our user manual both saved as pdf files.

Our "static" folder holds our css files, files for images displayed throughout the website, our javascript files, and 
a folder for videos displayed in the top parts of most of the pages of our website.

The "templates" folder is another requirement of flask and it holds the five html files for the 5 pages in our website.

The "venv" folder contains the files created when one first creates a virtual environment. We used this virtual environment
to develop and to publish our web app to "heroku" cloud services for hosting. This folder is mostly irrelevant and we 
weren't sure if to add it to this directory but we decided to go through with it in case the professor would want to take a 
look at it. 

The remaining three files in the website directory are the app.py file (the home of our flask app), Procfile (required by 
heroku to "guide" it and tell it what file to look for when it runs (the app.py file)), and the requirements.txt file 
(another file required by heroku to know what dependencies it has to install to run the app). 


Anvil web app
=============

A word document with code for anvil forms.

This concludes the contents of this README file.
