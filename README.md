# Web-Scraping

## What Is Web Scraping?
Web scraping is the process of gathering information from the Internet or extraction of data from a website, in other words Web scraping is the process of collecting and parsing raw data from the Web. Even copy-pasting the lyrics of your favorite song is a form of web scraping! 


## APIs: An Alternative to Web Scraping
Some website providers offer Application Programming Interfaces (APIs) that allow you to access their data in a predefined manner. With APIs, you can avoid parsing HTML and instead access the data directly using formats like JSON and XML. 

-------------------------------------------------------------------------------------------------------------------------------------------------------

## Website - Metacritic
Metacritic is a website that aggregates reviews of films, TV shows, music albums, video games and formerly, books. For each product, the scores from each review are averaged.

<img width="1240" alt="Screen Shot 2021-06-01 at 5 09 30 PM" src="https://user-images.githubusercontent.com/58945964/120397612-39ac3180-c2fe-11eb-81d9-3f442a52f833.png">


-------------------------------------------------------------------------------------------------------------------------------------------------------

## Program Execution Steps:

1. Click on >> or Restart and Rerun the Kernel or Run all cell.

2. Ask the user to enter a Valid movie name. 

3. Ask the user to enter either a cast or director name. 

4. Ask the user to enter a valid actor name.
If one of the actor name is wrong it will ask for that particular actor name

-------------------------------------------------------------------------------------------------------------------------------------------------------

## Reading Into CSV:

First line will be the heading ['Movie Name', 'Movie Detail Link' 'Directors','Casts']
Next 500 line will be there associated information. So total 501 lines [ 1 header + 500 movies ]

-------------------------------------------------------------------------------------------------------------------------------------------------------


## Reading Into Database:

First line will be the heading ['Movie Name', 'Movie Detail Link' 'Directors','Casts']
Next 500 line will be there associated information.


-------------------------------------------------------------------------------------------------------------------------------------------------------

## Program Flow: 

1] Import all the necessary library.
2] By pass the SSl.
3] Create a user agent. 
4] Now go through all the 5 pages and scrape out information from each of the 5 page and store it in a container.
5] Now container contains 5 pages. So go through each page and scrape out movie name from there 5 pages and store it in a list
6] Similarly in order to get detailed information about director and cast wee got to visit the detailed link page. Link for this detailed page is present in our container.
7] From the detailed page we can now scrape out. Director , main and primary cast.
8] our cast will be a combination of main and primary cast.


---------------------------------------------------------------------------------------------------------------------------------
9] Append to csv:
1] once we have information about Movie Name, Director and Cast. We can now append them in our csv file.

--------------------------------------------------------------------------------------------------------------------------------------

9] Append to Db:
1] once we have information about Movie Name, Director and Cast. We can now append them in DB.

-----------------------------------------------------------------------------------------------------------------------------------



10] Extracting 2 Piece of Information:
1] user is asked to enter the movie information he requires.
2] The Program goes through each movie. Check if the user entered movie match the movie that is present container. If present extract the information.

-----------------------------------------------------------------------------------------------------------------------------------------------

## Question One: 
Program will analyze how many times has each actor/actress appeared in these top 500 movies, and analyze how many times has each director appeared in these top 500 movies.

The actor and director with maximum count will be the actor who has acted/ Director maximum movie. Hence they are more popular.

-------------------------------------------------------------------------------------------------------------------------------------------------

## Question Two: 
User is asked to choose 2 director. If the directors are present in the 500 movies list then
Program creates a dictionary of actors/actresses that the directors have worked together with in each movie, then calculate their cosine similarity, which directors work with similar groups of actors/actresses.

The Maximum cosine similarity is a famous director


-----------------------------------------------------------------------------------------------------------------------------------------

## Question Three:
Program pick 5 of your favorite actors/actresses from this list of top 500 movies. Then create a dictionary of all the actors/actresses that they have collaborated with in a movie. 

It then create a cosine similarity of each actor. The Actor with maximum cosine similarity has worked with maximum number of actor and is the famous one.

------------------------------------------------------------------------------------------------------
