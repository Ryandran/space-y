# space-y
In this capstone, we will predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch. In this lab, you will collect and make sure the data is in the correct format from an API. The following is an example of a successful and launch.
## Data Wrangling
In this lab, you will make a get request to the SpaceX API. You will also do some basic data wrangling and formating. 
- Request to the SpaceX API
- Clean the requested data
Takes the dataset and uses the rocket column to call the API and append the data to the list :
- "https://api.spacexdata.com/v4/rockets/"
- "https://api.spacexdata.com/v4/launchpads/"
- "https://api.spacexdata.com/v4/payloads/"
- "https://api.spacexdata.com/v4/cores/"
- "https://api.spacexdata.com/v4/launches/past"
## Webscraping
### **Space X  Falcon 9 First Stage Landing Prediction**
In this lab, you will be performing web scraping to collect Falcon 9 historical launch records from a Wikipedia page titled `List of Falcon 9 and Falcon Heavy launches`

### Objectives
Web scrap Falcon 9 launch records with `BeautifulSoup`: 
- Extract a Falcon 9 launch records HTML table from Wikipedia :
  https://en.wikipedia.org/wiki/List_of_Falcon_9_and_Falcon_Heavy_launches
- Parse the table and convert it into a Pandas data frame
