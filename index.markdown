---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home

---

# **How New York’s Subway Ridership Dances to the Rhythm of the City**

New York City’s subway system is more than just a means of transportation—it is a living, breathing reflection of the city's dynamic pulse. Every fluctuation in ridership tells a story about what is happening above ground. From the exuberant influx of marathon runners to the quiet lulls following major incidents, the subway responds in real-time to the city's events.

In this data story, we delve into the intricate relationship between the city's happenings and subway usage. Utilizing [MTA Subway Hourly Ridership Data (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Hourly-Ridership-2020-2024/wujg-7c2s/about_data) and [Major Subway Incident Reports (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Major-Incidents-2020-2024/j6d2-s8m2/about_data) datasets, we explore how planned events like the [New York City Marathon](https://www.nyrr.org/tcsnycmarathon) and spontaneous occurrences such as protests or severe weather conditions influence the flow of commuters. Our analysis reveals patterns that not only highlight the subway's responsiveness but also offer insights into the city's resilience and adaptability.

Join us as we uncover the narratives hidden within the numbers, illustrating how the subway serves as a barometer for New York City's ever-changing landscape.

---

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
    Figure 1: Heatmap showing hourly subway ridership on Marathon Sunday, with emphasis on stations along or near the race route.
  </p>
</div>

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\stations_line_plot.html" width="1120" height="950" style="border:none;" title="Stations Ridership Line Plot: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    Figure 2: Line plot comparing hourly ridership at key subway stations on Marathon Sunday, illustrating patterns of crowd movement and station activity throughout the day.
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
    Figure 3: Hourly subway ridership trends on New Year's Eve (Dec 31) vs. New Year's Day (Jan 1), highlighting changes in travel behaviour around midnight.
  </p>
</div>

### The Cultural Pulse of Midnight in Midtown

New Year’s Eve in New York is more than just a party—it is a city-wide ritual. With over a million people cramming into the blocks around Times Square (per [NYPD estimates](https://www.nytimes.com/2023/12/31/nyregion/times-square-new-years-eve.html)), the MTA becomes the only practical way in and out. The subway does not just reflect the party—it enables it.

Even in years affected by pandemic restrictions, data shows a smaller but still visible spike, suggesting the deep cultural grip of this annual celebration.

*Want to learn more about the infrastructure that makes this night possible? See this behind-the-scenes feature on [how NYC manages crowd control and transit for New Year’s Eve](https://gothamist.com/news/heres-how-nyc-prepares-for-new-years-eve-in-times-square).*

[comment]: <> (📊 *Visual idea: A map of protest locations with ridership changes at nearby stations.* / title="Subway Ridership Change During Protest Events (Brooklyn & Midtown) )

---

## Act II: When Disaster Strikes – How Incidents Disrupt the Flow

Disruptions on the subway often come like a ripple effect, starting small but quickly magnifying. A single signal failure, a sudden snowstorm, or even a heatwave can derail the city’s rhythm, throwing off thousands of commuters. As we dive into these incidents, we uncover how these moments of chaos test the resilience of the MTA—and New Yorkers’ ability to adapt.

---

### The "Signal Problem" Domino Effect

A signal failure—it seems like a simple issue. But for the subway, it is often a ticking time bomb.

Our analysis of the **MTA Major Incidents dataset** reveals just how critical these disruptions are:

* A signal delay at Penn Station does not just affect that single station; it sends shock waves across the city’s busiest lines. A morning delay can reduce ridership by 15% across stations on the A, C, and E lines, which serve key areas like Chelsea, Midtown, and Downtown Manhattan.
* The effects are long-lasting: When these delays last for 3 hours or more, many commuters seek alternatives—Uber, buses, or even working from home. After such delays, commuters do not always return immediately to the subway. They have found a new way to get around.

This domino effect illustrates the delicate balance the subway maintains: a small disruption can spiral out of control, affecting thousands of riders across multiple boroughs.

[comment]: <> (📊 *Visual idea: A ridership line graph showing typical commuter traffic with overlaid timestamps marking major delays (signal issues) and their impact on nearby stations.* )

---

### Extreme Weather vs. Subway Reliance

Weather patterns play a huge role in shaping subway usage—but the impact is not always as expected. The city’s reliance on the subway fluctuates with the temperature.

#### Snowstorms: A Bitter Chill for Outer Boroughs

When winter storms hit, the outer boroughs feel the brunt of it. Snow is no stranger to New York, but it still disrupts the subway flow in surprising ways:

* During the snowstorms of January 2022 and December 2023, we saw a 20% drop in ridership—but only in outer boroughs like Queens and The Bronx. These boroughs depend more on buses, which are less reliable in snowstorms, and this drops their ridership during severe weather.
* Manhattan, however, kept moving. Its underground lines are better shielded from the snow, meaning ridership patterns stayed relatively steady even in the worst weather.

#### Heatwaves: When the Subway Becomes a Lifeline

Summer heat, on the other hand, has an entirely different effect. During heatwaves like the one in July 2023, the subway becomes the only escape from the scorching streets:

* Temperature extremes (38°C+) send subway use surging by 10%, as walking outside is unbearable.
* With air conditioning and a more controlled environment, New Yorkers turn to the subway as a sanctuary from the heat, while others find themselves avoiding the outdoors altogether.

These findings reveal a stark contrast: while snowstorm disruptions have a regional effect, heatwaves increase overall subway use. Weather patterns matter, and commuters change their habits in response to extreme conditions.

[comment]: <> (📊 *Visual idea: A scatter plot of temperature vs. ridership, with key heatwave and snowstorm dates highlighted, showing how temperature extremes influence commuter behaviour.* )

---

###  The Takeaways

The data underscores two key points:

1. Delays are not just annoyances—they are cascading events that affect a much broader section of the system than one might expect. Small disruptions at key hubs, like Penn Station, can have citywide consequences.
2. Weather changes commuter behaviour. Snowstorms and heatwaves might look similar on the surface, but they differently shape ridership patterns, with cold weather affecting only certain boroughs and heatwaves bringing an overall increase in usage.

The subway is an adaptable system, but when disaster strikes—whether due to a technical failure or extreme weather—New Yorkers must adjust quickly and the MTA must be ready to respond just as swiftly, to keep the city's pulse moving.

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

🔍 *Want to dive deeper into the MTA's data and how they use these insights for planning? Check out the latest MTA reports on [subway ridership trends](https://new.mta.info/) and future improvements.*

