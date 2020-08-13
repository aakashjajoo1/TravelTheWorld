# TravelTheWorld
=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=
PennKey: aakashj1 & yathu
=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=:=

===================
=: User Manual :=
===================
- Run the "Main" class
- The program will run in the console
- Enter the amount of airports you want to be loaded (it will load the most popular x airports); be wary, the time to scrape the data grows quadratically
- The airports will have a corresponding number displayed in console
- Follow the console commands to either quit, have a flight with layover, or a flight with no layover
- Enter the airports with their corresponding number printed above
- The flights and total cost will be printed
- You can continue to choose flights until you decide to terminate the program

NOTE: if numerous/all searches fail, visit https://www.kayak.com/flights/ATL-CTG/2020-06-01?sort=price_a
and submit the recaptcha form. 

===================
=: Assumptions :=
===================
- Flight data is obtained for June 1st 2020 // to modify this, adjust the scraper in Matrix class
- Prices are obtained from Kayak and are the associated one-way ticket flights
- The cheapest path including a layover is simply the cheapest path from source to layover merged with the path from layover to target


===================
=: Links to Data :=
===================

- Popularity of airports was determined by: https://raw.githubusercontent.com/jpatokal/openflights/master/data/routes.dat
- Flight prices were obtained from Kayak.com

===================
=: Project Summary :=
===================

Authors: Aakash Jajoo and Yathushan Nadanapathan

Project Name: Cheaply Travel the World 

Project Description:

Our project determines the cheapest path from airport a to airport b. Frequently, the cheapest flight isn't always
the direct flight. Our project takes in the first n popular international airports and finds the cheapest flights
that go from the user's choice departing location to their choice destination. The user is also provided with the option
to choose a layover if he/she desires. Our code outputs both the path in addition to the cost. If there is no such flight,
our code states so. 

Categories:

Graphs & Graph Algorithms:
We build a graph for the n airports with directed weighted edges, where the weight is the cost of the flight between the two airports.
We used Dijkstra's Algorithm to determine the shortest path, since edge weights are non-negative.

Document Search / Information Networks:
We scrape the web for each flight's cost.

Work Breakdown:

Aakash Jajoo: Determining the n most popular airports. Creating the graph, which includes obtaining all the prices for each flight.

Yathushan Nadanapathan: Implementing Dijkstra's on the graph and creating the basic user interface.

Combined: Editing each other's work



