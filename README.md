# Point-to-point graphs for football table data

How did Union Berlin - the German capital's "other" team - manage to make it into the Europa League while their rivals from the westside of town only just avoided relegation?

These point-to-point graphs show how much advantage Union got from playing at their "fan-built" stadium - even with barely anyone there.

In fact, no other team bar Eintracht Frankfurt had a more disproportionate home ground advantage.

![image](https://user-images.githubusercontent.com/69304112/130336648-ae7f8496-b39b-412b-8928-a4d54727c26a.png)

This script that takes a 'wide' table of a football season and returns a quartet of point-to-point graphs. Point-to-point graphs are an effective of showing how various values have changed over time, or here, how various values change for a team at home and on the road.


**About**

Created using Plotly (.go) with table data from Soccerway.com.

In this example, it looks at the final 2020-2021 Bundesliga season.

Four custom style functions have been built into the graph function: 'Minimalist' (above), 'Default', 'Pastely', 'LightBlueBack'.

![newplot (5)](https://user-images.githubusercontent.com/69304112/130306831-58551689-2bb1-456d-a38d-50d7d4ea6d95.png)
![newplot (3)](https://user-images.githubusercontent.com/69304112/130306759-74e8ced4-a0f7-4346-94e5-a8b76b12da86.png)
![newplot (4)](https://user-images.githubusercontent.com/69304112/130306757-1e4931be-af19-411f-9c83-1dc02179752a.png)

Before starting, use the soccerwayWideTableScraper to scrape the wide table data (which includes breakdowns of home and away season tallies) to create a CSV of this data. 

Then run the main script, which will begin by making a number of simple calculations (eg goals for per home match) based on that data.  

The allPlots function then creates the quartet of slope graphs, with two teams able to be highlighted. These two teams are noted as 'home' and 'away' as this function is designed to be be used automatically each matchday to produce slope graphs for that round's various opponents. These two teams are positioned on top of all the other teams' lines (in other words, they are moved to the bottom of the dataframe table).

Four custom style functions have been built into the graph function: 'Default', 'Minimalist', 'Pastely', 'LightBlueBack'. Access these via the chosen_style variable.
