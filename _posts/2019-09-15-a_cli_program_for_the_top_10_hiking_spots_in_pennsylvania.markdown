---
layout: post
title:      "A CLI Program for the Top 10 Hiking Spots in Pennsylvania"
date:       2019-09-15 20:06:21 +0000
permalink:  a_cli_program_for_the_top_10_hiking_spots_in_pennsylvania
---


I recently created a CLI program using Ruby that shows the top 10 hiking spots in PA based upon an article from 2015 on a  website called onlyinyourstate.com. The program list the top 10 hiking spots in order and then lets you choose a number between 1-10 to view a description of the selected spot. All of the data was scraped from the website and then stored in HikingSpot object so that it could be used by the CLI. I first started by creating a Scraper class to retrieve the data from the website using Nokogiri and Open-URI. After that I created the HikingSpot class to store the data that was scraped. The HikingSpot class uses class methods from the Scraper class to retrieve the data and instantiate new HikingSpot objects with the attributes of a title and a description. The HikingSpot class also keeps track of all HikingSpot objects that are instantiated so that data can we used in the CLI. Once I had the HikingSpot class finished, I went and created the CLI. The CLI will list all the titles of the HikingSpot objects in order from 1 to 10, and then will ask you to select a number between 1-10 to view a description. The CLI will loop through as many times as the user the pleases, until the user decides to exit the program when prompted by CLI. 
