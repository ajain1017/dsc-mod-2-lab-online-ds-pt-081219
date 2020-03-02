
# Mod 2 SQL/API Database Lab

## Goal

We will examine an SQL database consisting of historic match data for the German Bundesliga and English Premier League from 1993 up to 2016, as well as a web-based system, Dark Sky, containing historical weather data on various locations at various times. Using these databases, we will calculate summary statistics and create a NoSQL databse for the 2011 season.

## Process

#### Query SQL database
- Extract, Transform, and Load

#### Get the weather data from the DarkSky API
- Make API calls to store weather data for gamedays

#### Calculate and display summary statistics
- The total number of goals scored by each team during the 2011 season  
- The total number of wins each team earned during the 2011 season  
- The team's win percentage on days where it was raining during games in the 2011 season  
- A histogram visualization of the team's wins and losses for the 2011 season

#### Load the data into MongoDB
- Create object-oriented, simple and dynamic NoSQL database
- Store each team as object in database including the summary statistics desired

--**Assumptions:--**  
Note that each game is played in a different location, and this information is not contained in our SQL database. However, since most teams are from Germany, we will use the weather in Berlin, Germany as a proxy for this information. Also, we will count the weather to be raining if it was raining in Berlin on the day the game was played, rather than finding the actual weather at the time of each game at its specific location.