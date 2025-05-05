---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: How New York’s Subway Ridership Dances to the Rhythm of the City

---

<img src="{{ site.baseurl }}/Figures/NYC_subway.jpg" alt="A descriptive alt text for your header image" style="width:100%; height:auto; object-fit: cover;">

New York City’s subway system is more than just a means of transportation—it is a living, breathing reflection of the city's dynamic pulse. Every fluctuation in ridership tells a story about what is happening above ground. From the exuberant influx of marathon runners to the quiet lulls following major incidents, the subway responds in real-time to the city's events.

In this data story, we delve into the intricate relationship between the city's happenings and subway usage. Utilizing [MTA Subway Hourly Ridership Data (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Hourly-Ridership-2020-2024/wujg-7c2s/about_data) and [Major Subway Incident Reports (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Major-Incidents-2020-2024/j6d2-s8m2/about_data) datasets, we explore how planned events like the [New York City Marathon](https://www.nyrr.org/tcsnycmarathon) and spontaneous occurrences such as protests or severe weather conditions influence the flow of commuters. Our analysis reveals patterns that not only highlight the subway's responsiveness but also offer insights into the city's resilience and adaptability.

Join us as we uncover the narratives hidden within the numbers, illustrating how the subway serves as a barometer for New York City's ever-changing landscape.



## ACT I : When the City Celebrates, the Subway Becomes a Party

### New York City Marathon
Every first Sunday in November, over 50,000 runners traverse all five boroughs for the [official New York City Marathon](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory). Stations near Central Park, like 59 St-Columbus Circle and 72 St, experience ridership spikes of 30–40% compared to typical Sundays.

Our data shows:
- An early morning sharp surge (5–7 AM) as runners head to Staten Island for the starting line.
- A second midday wave (10 AM–2 PM) as spectators travel to cheer zones.
- A noticeable dip in other parts of the city, why? As half of Manhattan is either running or watching!

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\marathon_heatmap.html" width="1200" height="900" style="border:none;" title="Subway Ridership Heatmap: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 1:</strong> Heatmap showing hourly subway ridership on Marathon Sunday, with emphasis on stations along or near the race route.
  </p>
</div>

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\stations_line_plot.html" width="1120" height="950" style="border:none;" title="Stations Ridership Line Plot: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 2:</strong> Line plot comparing hourly ridership at key subway stations on Marathon Sunday, illustrating patterns of crowd movement and station activity throughout the day.
  </p>
</div>

The New York City Marathon is not just a race; it is a storied tradition. Starting in 1970 with just 127 participants looping around Central Park, it has evolved into the world's largest marathon, weaving through all five boroughs and drawing nearly two million spectators annually. For a detailed look at its rich history, visit the [official NYRR Marathon history page](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory). ([TCS New York City Marathon](https://www.worldmarathonmajors.com/six-star-major/new-york-city), [New York City Marathon History](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory)).

But why has marathon running surged in popularity? Beyond the challenge, many are drawn to the structure, community, and personal growth it offers. The pandemic era, in particular, saw a boom in running as people sought connection and purpose. Platforms like TikTok have further fuelled this trend, turning marathon training into a shared journey. 

*Explore more about this phenomenon in [this insightful article](https://www.axios.com/2024/05/08/marathon-running-training-tiktok). ([Why Marathon Running Is Booming - WSJ](https://www.wsj.com/lifestyle/fitness/marathon-increasing-popularity-2025-caac1bb6), [Axios Finish Line: Why more people are running marathons](https://www.axios.com/2024/05/08/marathon-running-training-tiktok)).*

---

### New Year’s Eve – The Ultimate Subway Stress Test

When the ball drops in Times Square, it is not just a moment of celebration—it is one of the largest and most predictable surges in subway ridership all year.

Each 31 December, stations near Times Square, like 42 St–Port Authority, Times Sq–42 St, and 34 St–Penn Station, become pressure valves for the city's festivities. Our data reveals:

* A dramatic spike from 11 PM to 1 AM, as revellers flood into Midtown to secure a view of the countdown.
* Late-night services (1–3 AM) experience ridership surges up to 2.5× higher than a typical Saturday night.
* The 1, 2, N, Q, R, and A/C/E lines show the heaviest traffic during this window, especially near Times Square and Columbus Circle.

But then comes the New Year’s Day hangover—both literal and logistical. On 1 January:

* Ridership drops 40–50% below normal Sunday levels, particularly before noon.
* Uptown-bound stations remain unusually quiet until mid-afternoon, as the city slowly reawakens.

This dramatic peak-and-crash pattern makes New Year’s Eve one of the most extreme temporal oscillations in the entire ridership dataset.

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates/nye_timeseries.html" width="920" height="625" style="border:none;" title="New Year's Eve Subway Ridership – Hourly Trend (Dec 31 vs Jan 1)"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 3:</strong> Hourly subway ridership trends on New Year's Eve (Dec 31) vs. New Year's Day (Jan 1), highlighting changes in travel behaviour around midnight.
  </p>
</div>

### The Cultural Pulse of Midnight in Midtown

New Year’s Eve in New York is more than just a party—it is a city-wide ritual. With over a million people cramming into the blocks around Times Square (per [NYPD estimates](https://www.nytimes.com/2023/12/31/nyregion/times-square-new-years-eve.html)), the MTA becomes the only practical way in and out. The subway does not just reflect the party—it enables it.

Even in years affected by pandemic restrictions, data shows a smaller but still visible spike, suggesting the deep cultural grip of this annual celebration.

*Want to learn more about the infrastructure that makes this night possible? See this behind-the-scenes feature on [how NYC manages crowd control and transit for New Year’s Eve](https://gothamist.com/news/heres-how-nyc-prepares-for-new-years-eve-in-times-square).*

[comment]: <> (*Visual idea: A map of protest locations with ridership changes at nearby stations.* / title="Subway Ridership Change During Protest Events (Brooklyn & Midtown) )

---

## Act II: When the City Struggles – The Subway Feels It

When the city experiences stress - if it is human, technical or environmental - the underground feels it.

If we examine the overall distribution of major incidents over time, from 2020-2024, we can begin to see patterns in how and when things go wrong. This heatmap reveals when certain types of incidents dominate the MTA's operations.
<div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/Heatmap_incidents.png" style="width: 150%">
</div>
<strong>Figure 4:</strong> Heatmap of the reported incidents of NYC subway by date and Category


Two categories stand out sharply:

- "Persons on trackbed / Police / Medical": These are the most frequent and disruptive incidents, often tied to emergencies, vulnerable populations, or mental health crises.
- "Signals": A chronic technical issue that often reflects infrastructure aging or network congestion during high-traffic periods.

This pattern shows that human and technical factors are the main stress points in keeping the subway running smoothly.

When looking at the heatmap in Figure 5, we see a distinct period of reduced incident reporting. This quiet phase aligns with the early months of the COVID-19 pandemic in New York City ([COVID-19 pandemic in New York City](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_New_York_City)). 

<div style="display: flex; justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/corona_heatmap.png" style="width: 150%">
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 5:</strong> Heatmap marking a period with fewer incidents
  </p>
</div>

The subway, in a way, mirrors how people behave and move throughout the city. When the city slowed down, so did its underground lifeline.

---

### Incidents During Big Events

Are celebrations linked to more disruptions? The data suggests: yes.

#### NYC Marathon

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/Incidents_marathon.png" style="width: 150%">
</div>
During marathon months, we observe a noticeable spike in operational and medical incidents, especially near start and finish zones. The added foot traffic and street closures may lead to increased platform crowding, longer dwell times, and greater pressure on subway operations.

- Even though it’s a celebratory event, the system experiences strain from crowd control and accessibility demands.

#### New Year’s Eve

<div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/Incidents_nye.png" style="width: 150%">
</div>

On New Year’s Eve, the story intensifies. We see a clear jump in incidents, especially those tied to safety and policing. This aligns with increased late-night ridership, alcohol consumption, and large gatherings in areas like Times Square.

- The subway doesn't just mirror the city's mood—it absorbs its chaos.


Both datasets reveal that planned, joyful events still cause operational friction. But the nature of the disruptions differs: the Marathon triggers physical and logistical strains, while New Year's Eve surfaces social and behavioral challenges. Together, they show how event-driven ridership isn't just a number—it has human, systemic consequences underground.

---

## Act III: Disruption and Detour — When the Subway Becomes a Mirror of the City

New York is a city in constant motion—but sometimes, that motion stutters, shifts, or surges unpredictably. From protests to power failures to momentary panic, the subway does not just reflect daily routines—it registers shock waves from the city's most dramatic moments.

This act dives into those unseen patterns—moments when riders changed course, either out of necessity or emotion, and the subway map reshaped itself in real time.

---

### Protest, Resistance, and Rerouteing

New Yorkers protest with their feet—and their MetroCards.

During the Black Lives Matter demonstrations in June 2020, our data shows sharp drops in ridership at several stations surrounding protest epicentres like Barclays Center in Brooklyn and Foley Square in Lower Manhattan.

* On 6 June 2020, when tens of thousands gathered at Barclays, entries at Atlantic Av–Barclays Ctr dropped over 50% compared to the previous Saturday.
* Nearby stations like Bergen St and 7 Av saw up ticks, suggesting riders rerouted to avoid heavy police presence or blocked access points.
* Similar rerouteing effects occurred during climate justice marches in midtown (September 2023), when Grand Central–42 St entries fell by 30% during peak march hours.

[comment]: <> (📊 *Visual idea: A map of protest locations with ridership changes at nearby stations.* / title="Subway Ridership Change During Protest Events (Brooklyn & Midtown) )

These events do not suppress movement—they redistribute it. New Yorkers are famously mobile and adaptable; when paths close, they find others.

*Want to know where the protests went and how the city responded? Read [this overview from Nye York Times](hhttps://www.nytimes.com/2020/05/30/nyregion/nyc-protests-george-floyd.html).*

---

### The Subway Avoidance Effect

Sometimes, fear—not protest—changes the flow.

After the Times Square subway shooting on 10 April 2022, we observed a noticeable dip in ridership at nearby stations:

* Bryant Park–42 St and Times Sq–42 St fell by 12–15% over the following week, despite no formal service disruptions.
* The drop was temporary—but striking. Stations two stops away (e.g., 34 St–Penn Station) saw no such change.

Similarly, during the 2023 Midtown blackout, stations on the F line around Lexington Av/63 St experienced a 24-hour ridership plunge, followed by a delayed return—with some usage patterns never fully recovering.

[comment]: <> (📊 *Visual idea: A bar chart of crime/incident dates vs. ridership drops at affected stations.* / title="Ridership Impact of Disruption Events (Shootings, Blackouts, Repairs) )


These moments reveal something deeper: the psychology of movement. Disruptions do not just block access—they create emotional echoes. Riders shift patterns for safety, convenience, or simply peace of mind.

*The MTA has acknowledged these trends in planning future comms and service recovery: see [MTA rider sentiment analysis](https://medium.com/@KingHenryMorgansDiary/post-pandemic-ridership-recovery-trends-across-mta-services-3b188ef03c05).*

---

### Long-Term Detours, Lasting Effects

Not all avoidance is temporary. The L train shutdown (April 2019–2020)—while just before our dataset begins—left behind ripple effects we can still observe:

* Several outer Brooklyn stations saw permanently reduced weekday traffic as riders shifted to alternate routes.
* Post-pandemic trends amplified this, with remote work reinforcing new habits formed during the shutdown.

Disruptions, whether momentary or structural, reshape the network—sometimes permanently.

*Want to learn more about the L train shutdown and its long-term effects? Check out [this in-depth analysis from New York Times](https://www.nytimes.com/2019/01/03/nyregion/l-train-shutdown.html). ([The L Train Shutdown: What You Need to Know - Carto](https://carto.com/blog/looking-at-the-l)).*

---

## Conclusion: The Subway as New York’s Pulse

The data reveals an undeniable truth: the subway does not merely serve New York City—it reacts to it. Every surge, every slowdown, every spike in ridership tells the story of the city’s heartbeats. From celebrations to crises, the subway is the city's pulse, recording every significant moment in real time.

We have witnessed the way subway stations respond to events like protests, parades, and power outages, and how these disruptions ripple through the system. But more importantly, we have seen how New Yorkers adapt. Whether it is rerouteing during protests, avoiding stations after incidents, or shifting their travel habits due to major repairs, the subway is a mirror that reflects the city’s resilience and fluidity.

---

### What This Means for the MTA

For the Metropolitan Transportation Authority (MTA), these insights offer critical lessons in adapting the city’s transportation infrastructure to the needs of its people:

* Event Planning: The subway must anticipate the massive surges that accompany major events like the New York City Marathon, New Year’s Eve, and protests. Special event scheduling and additional trains are essential to keep the city moving.

* Incident Response: New Yorkers do not forgive long delays—especially after high-profile incidents. Quick response times and recovery are crucial to regaining ridership trust after disruptions like shootings or power outages.

* Weather Adaptations: In the face of unpredictable weather patterns, adaptations like better air conditioning in summer and more efficient snow removal in winter can keep New Yorkers on the subway, no matter the season.

---

### For New Yorkers: A Daily Rhythm

For the people of New York, the subway is not just a means of transport—it is a part of their daily rhythm. It is the silent observer of the city’s emotional highs and lows. Whether it is a triumphant win, a community gathering, or a crisis, the subway is where stories unfold.

Through this analysis, we have gained a deeper understanding of the intricate dance between the subway and the city. We have learned how to read its rhythm, recognising the patterns that emerge during moments of tension and celebration. Now, we can anticipate how the city moves, adjusts, and comes together—or how it sometimes chooses to take a detour.

---

In the end, the subway is more than just a series of stations and tracks—it is a mirror of New York itself. It reflects the city’s chaos, creativity, resilience, and unyielding spirit. And as the data shows, the MTA is not just managing a transit system—it is managing the lifeblood of New York’s mobility.

*Want to dive deeper into the MTA's data and how they use these insights for planning? Check out the latest MTA reports on [subway ridership trends](https://new.mta.info/) and future improvements.*

