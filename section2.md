# 3 When do accidents occur?

For both the police force as well as citizens of Tempe, it is valuable to know _when_ accidents happen. Toggle between the different calendar plots below to see when different types of accidents happen.

When we consider _All Traffic Accidents_, we see a significant increase in accidents during rush hours on weekdays. Here, significantly more crashes occur when people commute _from_ work rather than _to_ work. If assuming approximately the same number of people commute to and from work every day, this most likely means that drivers are less attentive in the afternoon. This conclusion fits well with an [investigation](https://injuryfacts.nsc.org/motor-vehicle/overview/crashes-by-time-of-day-and-day-of-week/) carried out by the National Safety Council in 2021, where between 4 p.m. and 7 p.m. was found to be the most dangerous time of the day to be on the road. Different reasons are given for this such as mid-afternoon energy slumps, sending text messages to partners, and general multitasking such as wrapping up the last work calls and emails. You can read more [here](https://www.fleschlawfirm.com/blog/your-afternoon-commute-is-more-dangerous-than-your-morning-drive/).

When considering _Severe Injury Traffic Accidents_ (serious/incapacitating injury or death), we see that the evenings and nights lead to more severe injury accidents. However, there is no apparent difference between a weekday and the weekend.

When considering crashes involving a pedestrian or a cyclist, occurrences are somewhat equally distributed along all hours of the day and all days of the week.

Crashes involving alcohol or drugs primarily occur during nighttime. Here, almost just as many crashes occur on weekdays as weekends, with the only major difference being the increased number of crashes between 4 a.m. and 5 a.m. on weekends. This makes sense as people generally are out later on weekends.

<iframe src="contents/interactive-calendar-plot.html"
    sandbox="allow-same-origin allow-scripts"
    width="100%"
    height="600"
    scrolling="no"
    seamless="seamless"
    frameborder="0"
    style="max-width: 100%;">
</iframe>

## 3.1 Alcohol and drugs

Now, knowing that both alcohol and drug-impaired crashes, as well as severe injury crashes, primarily occur at night, it would be interesting to investigate if the involvement of alcohol or drugs, in general, increases the likelihood of severe injuries or deaths. 
Below, we see the correlation between all severe injury crashes (normalized) and the number of crashes with drug and/or alcohol involvement. As all weekdays exhibit a similar trend in the "Alcohol/drug-impaired accidents" plot above, the correlation plot below pools all days of the week and simply considers the correlation over the 24 hours in a day. Next to the correlation plot, the mean daily distribution of all crashes is shown. This distribution is what the number of severe injury crashes is normalized by.

From the morning and throughout the day, a clear positive correlation is seen from the best-fit straight line (linear regression). However, when considering the value of R^2, it is apparent that the fit of the linear regression model is only moderate. This means that the number of crashes involving alcohol or drugs only moderately influences the normalized number of severe injury crashes. As many other hourly-dependent factors such as light conditions, road conditions, traffic density, driver alertness, etc., also influence the normalized number of severe injury crashes, a "moderate fit at best" is the expected outcome of a simple linear regression model.

<iframe src="contents/correlation_plot_severe_vs_alco_new.html"
    sandbox="allow-same-origin allow-scripts"
    height="400"
    scrolling="no"
    seamless="seamless"
    frameborder="0"
    style="max-width: 100%;">
</iframe>

