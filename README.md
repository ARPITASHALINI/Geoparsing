# Lab 7: Geoparsing with Python. 

This lab is our final lab for the submission for Programming for GIS (IDCE 30274), which is a course taken for the completion of MS in GIS from Clark University. 

In this lab we work through geoparsing, which is a technique of extracting place names from text and matching those names with spatial coordinates. The highest amount of geoparsing occurs with social media posts, where they extract the key information of a place and provide you with suggestions related to that place. 

This assignment works through two parts:
1. We are provided with the book The innocents abroad, we pass the url for the freely available .txt form and decode it in utf-8. We use geotext which allows us to extract city names. . Using the coordinates we try to map the places on the map. 
2. The second part works as a challenge where we are required to select a book of our choice and geoparse it. I chose The Bleak house by Charles Dickens.


There were many challenges that I came across the code. The first being trying to fond a book which has various city names and the code being able to read it. I am still facing an issue where my code uses 'OF' as city name. I had to use a lot of stckoverflow to decode most of the errors. Our CA Shashank was the most helpful, he guided along the code and explained why and how we were using certain function. The code was developed by taking inspiration from our Professor's code which he shared for the major assignment. 

Certain questions need to be answered as we move along with the code:

  1. Is the gazetteer we're using appropriate for the text? What might be some of the challenges of using Nominatim with a book published in 1859?
  The gazetteer we are using, uses coordinates from the present city while the city names present in the book are from 1859. Certain boundaries have been drawn since 1859, the cities have fragmented into smaller parts, some cities have also changed their names. So using this gazetteer for the text is inappropriate. 
  
  2. How accurate do you think the outputs are? Are there any city names that seem suspect? If so, what are some Natural Language Processing methods that you could use to filter words that might be city names, but probably weren't intended as city references in the text?
  The output we ave obtained could be a little bias. We received 'OF' as a city name which I believe is abrupt. We could use Named Entity Recognition, which is a basic and useful technique in extracting the entities in text. It identifies such as people, locations, organisations. 
  
 3. What are some alternative approaches to mapping the data? The tutorial here uses duplicate entries and opacity to present a type of "color ramp": could this be done better?
  This is something which I am researching more about. Ihaven't been able to find other useful approaches to map the data. 
