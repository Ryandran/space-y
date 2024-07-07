<h1 align=center><font size = 5>Applied Data Science Capstone</font></h1>
## Introduction
In this capstone, we will predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch. In this lab, you will collect and make sure the data is in the correct format from an API. The following is an example of a successful and launch.
## Lab 1 : Data Wrangling
In this lab, you will make a get request to the SpaceX API. You will also do some basic data wrangling and formating. 
- Request to the SpaceX API
- Clean the requested data
Takes the dataset and uses the rocket column to call the API and append the data to the list :
- "https://api.spacexdata.com/v4/rockets/"
- "https://api.spacexdata.com/v4/launchpads/"
- "https://api.spacexdata.com/v4/payloads/"
- "https://api.spacexdata.com/v4/cores/"
- "https://api.spacexdata.com/v4/launches/past"

## Lab 2: Data wrangling 
In this lab, we will perform some Exploratory Data Analysis (EDA) to find some patterns in the data and determine what would be the label for training supervised models. 

In the data set, there are several different cases where the booster did not land successfully. Sometimes a landing was attempted but failed due to an accident; for example, <code>True Ocean</code> means the mission outcome was successfully  landed to a specific region of the ocean while <code>False Ocean</code> means the mission outcome was unsuccessfully landed to a specific region of the ocean. <code>True RTLS</code> means the mission outcome was successfully  landed to a ground pad <code>False RTLS</code> means the mission outcome was unsuccessfully landed to a ground pad.<code>True ASDS</code> means the mission outcome was successfully landed on  a drone ship <code>False ASDS</code> means the mission outcome was unsuccessfully landed on a drone ship. 

In this lab we will mainly convert those outcomes into Training Labels with `1` means the booster successfully landed `0` means it was unsuccessful.

## Webscraping
### **Space X  Falcon 9 First Stage Landing Prediction**
In this lab, you will be performing web scraping to collect Falcon 9 historical launch records from a Wikipedia page titled `List of Falcon 9 and Falcon Heavy launches`

### Objectives
Web scrap Falcon 9 launch records with `BeautifulSoup`: 
- Extract a Falcon 9 launch records HTML table from Wikipedia :
  https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches
- Parse the table and convert it into a Pandas data frame
  
<h1 align=center><font size = 5>Assignment: SQL Notebook for Peer Assignment</font></h1>
