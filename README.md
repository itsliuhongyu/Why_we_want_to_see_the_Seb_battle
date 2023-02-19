# What is this?

This is a data project visualizing the racing career of Sebastien Loeb and Sebastien Ogier, the two most legendary rally racers in the past two decades.

# Gather the data

The data of this project comes from [ewrc-results.com](https://www.ewrc-results.com/). This is a database of all rally result founded by a group of rally fans. This is the best free data I can find about the WRC as the official website hosted by FIA requires a media key to access the historical results.

To scrape the data, I used Python and pandas to create a loop appending the urls of all the events a driver have participated. Then, I used python to go to the php database of all the events, and gathering the ranking the driver in each stages. I have saved the rankings of the drivers in each events as well.

For my visualization, I individually scraped all the WRC events taking place since 2000, and I assigned an unique serial number for each of them.

# What analysis did I do?

First of all, I did some basic analysis comparing the event winning rate and event retirement rate of Loeb and Ogier. Using ggplot, I created some basic visualizations. I used red for Loeb, and blue for Ogier, not only becuase red and blue has a meaning of rivalry in WRC, but also they are the team color for Citroen where Loeb raced for throughout his career, and Volkswagen which Ogier represented.

For the timeline visualization, I used Altair to create a bump chart with serial number of the events as x axis, and the ranking as the y axis. Then, I used rectangle demand to highlight all even years in gray so that it will be easier for readers to differentiate the years each event took place.

At first, I hoped to plot some of the other drivers in gray as comparison. But it made the visualization very noisy so I droped it. 

I decided to start my visualization in 2002 because it is the year when Loeb first raced in WRC.

In the end, I exported my visualizations, and using Adobe Illustrator to add annotations. I rotated the timeline visualization for 90 degrees so that it is easier for the readers to navigate through the long timeline.

# Create the website

I used the css format from Bulma, but drew inspiration from the official WRC website. I used its font and color tone so that the website looks like a part of the official reportage.
