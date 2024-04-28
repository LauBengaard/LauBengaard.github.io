---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# Run local: bundle exec jekyll serve
layout: default
---

# Introduction

In this project, we delve into crime data from the San Francisco Police Department to uncover meaningful trends. The data spans from 2003 to 2017 and consists of just over 2 million incident reports. Each incident is associated with thirty-five attributes, including crime category, date and time, location (longitude, latitude), police district, and a crime description.

For our analysis, we have opted to concentrate on a subset of crimes, referred to as _focus crimes_ hereafter, to narrow the scope of our investigation. The crime types included in _focus crimes_ are listed below:

```
focuscrimes = ['WEAPON LAWS', 'PROSTITUTION', 'DRIVING UNDER THE INFLUENCE', 'ROBBERY', 'BURGLARY', 'ASSAULT', 'DRUNKENNESS', 'DRUG/NARCOTIC', 'TRESPASS', 'LARCENY/THEFT', 'VANDALISM', 'VEHICLE THEFT', 'STOLEN PROPERTY', 'DISORDERLY CONDUCT']
```

Our investigation aims to link three key aspects:

*   What crimes occur?
*   Where do the crimes occur?
*   When do the crimes occur?

We aspire that our findings can assist the citizens of San Francisco and tourists in avoiding crime, and we will provide our recommendations on how to do so effectively in a witty fashion.

* * *

# When to be aware?

Living in a big city, one must constantly be alert. While navigating the city, one must be aware of traffic, keeping one's belongings safe, worrying if we really did lock the door at home, or considering just how many drinks we can get away with having during happy hour and still drive home. It can be stressful worrying about all of these things all the time, so we decided to look into each of the focus crimes so that the citizens of San Francisco can worry about the right things at the right time—or simply do something to combat them.

The figure below shows how many incidents occur of each crime type on each day of the week. Many interesting trends can be identified, and for your convenience, we have listed the most important ones:

*   If you want to avoid falling for the temptation of driving under the influence, leave the car at home on Thursdays through Sundays. Happy hours on Mondays through Wednesdays are apparently not all that exciting, and you should be fine driving to those.
*   Cook your significant other a showstopping candlelight dinner on Tuesdays through Thursdays (not weekends!), as these are the days they are most inclined to, ahem, seek intimate connections elsewhere.
*   Work from home on Fridays! This is the day of the week where you are most likely to get a visit from a burglar. The same goes for having your car stolen!
*   Lastly, if your idea of a good time is being surrounded by overly drunk people, Saturdays and Sundays are your time to leave the house.

We hope these tips where helpful, feel free to draw further conclusions from the figure below!



![Ask Ubuntu image](/assets/png/focuscrime_occurences_barplot.png){: 
style="float: center; margin: 0 2rem 0 0;" width="100%" }


# Where to go or not to go?

Now, you might wonder which route home from the bar you're heading to next Friday would be the safest? Or which area you should stay in for your first trip to San Fransisco? Is it even necessary to do the planning and avoid areas you are not familiar with? 

Looking into the last question first, San Fransisco had a crime rate of 715 incidents per 100,000 citizens in 2017, which was 181% greater than the average of US and 158% greater than the average of California[^1], so the city definitely has a considerable number of crimes. 

Though, when looking into the different areas of San Fransisco, some areas are considerable more safe than others, so there is light ahead if you plan to move safely around in the city of Silicon Valley. The map below shows the density of crimes related to prostitution in the city for each day in the week: red areas have a higher density of crimes and areas with no coloring has no recorded crimes on that day. Some of the key takeaways from the plot is listed below:

*   Areas in and around Tendorloin, Mission and Chinatown seems to have a high density of crimes related to prostitution in every day of the week.
*   The safest day to visit SoMa, the home of great internet and software companies, is Sunday. 
*   If you are going for a taste of the famous seafood in Fisherman's Wharf avoid weekdays.
*   Twin Peaks seems to not have any crimes related to prostitution. 

Feel free to further go into details by going choosing a specific weekday (1=Monday, 2=Tuesday etc.) and adjusting the zoom on the map.


<iframe src="/assets/html/HeatMapWithTime_prostitution.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>

# Which crimes should you actually fear?

We all have irrational fears that consume unnecessary energy every day. We're here to show you which crimes you can safely ignore and which ones you should actually worry about.

The interactive plots below allow you to see the likelihood of each _focus crime_ occurring in relation to each other. Feel free to play around with the plot and select those crimes of interest to you!

Have you ever had anything stolen? Or do you know someone who has? If yes, there is a good explanation, since we can see that almost half of all crimes that occur in San Francisco are related to theft. Our advice: keep your valuables safely tucked away or keep them where you can see them at all times!

Ever feared spending a night in a cell after a wild evening out with your mates? No need to worry, less than 1% of all crimes are related to drinking too much. You are much more likely to get in trouble for narcotics, actually ten times as likely! So stick to beer and cocktails on your nights out!

Lastly, you are actually slightly more likely to have your vehicle stolen than your house robbed. So maybe consider using parking garages over street parking next time you drive into town and invest not only in the security of your home but also take extra steps to keep your car safe.



<iframe src="/assets/html/focuscrime_frequency_interactive_piechart.html" 
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0">
</iframe>


# References
[^1]: Macrotrends, [_San Francisco CA Crime Rate 1999-2018_](https://www.macrotrends.net/global-metrics/cities/us/ca/san-francisco/crime-rate-statistics), Accessed:28-03-2024.