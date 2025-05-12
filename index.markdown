---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# bundle exec jekyll serve 



layout: default
title: How New York’s Subway Ridership Dances to the Rhythm of the City

---
<style>
  .narrative-columns {
    display: flex;
    justify-content: space-between;
    gap: 20px;
    margin-top: 20px;
    flex-wrap: wrap; /* ensures responsive wrapping */
  }

  .narrative-container {
    flex: 1 1 48%; /* allows each box to take roughly half the row */
    box-sizing: border-box;
    padding: 10px;
    border-radius: 10px;
    min-width: 300px; /* helps with responsiveness */
  }

  .narrative-container h4 {
    margin-top: 0;
    font-weight: bold;
  }

  .narrative-container ul {
    padding-left: 20px;
  }

  .narrative-container li {
    margin-bottom: 10px;
  }
</style>

<img src="{{ site.baseurl }}/Figures/Subway.jpg" alt="A descriptive alt text for your header image" style="width:100%; height:auto; object-fit: cover;">

New York City’s subway system is more than just a means of transportation—it is a living, breathing reflection of the city's dynamic pulse. Every fluctuation in ridership tells a story about what is happening above ground. From the exuberant influx of marathon runners to the quiet lulls following major incidents, the subway responds in real-time to the city's events.

In this data story, we delve into the intricate relationship between the city's happenings and subway usage. Utilizing the two datasets: 
- [MTA Subway Hourly Ridership Data (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Hourly-Ridership-2020-2024/wujg-7c2s/about_data) 
- [Major Subway Incident Reports (2020–2024)](https://data.ny.gov/Transportation/MTA-Subway-Major-Incidents-2020-2024/j6d2-s8m2/about_data) 

We begin by analyzing everyday subway usage and how it varies across time and boroughs. Next, we dive into how large-scale planned events like the [New York City Marathon](https://www.nyrr.org/tcsnycmarathon) and [New years eve](https://www.timessquarenyc.org/nye/nye-landing) reshape the flow of commuters. Finally, we turn our attention to disruptions, exploring patterns in subway incidents to uncover what stresses the system and when. 

## ACT I : Understanding the subway usage

Before we dive into the bigger events in the Big Apple, we will first explore how the subway is used and how its ridership varies on a daily basis. Public transportation plays a vital role in New York City's rhythm, and the subway system is arguably its lifeline. Understanding its everyday usage provides critical context for interpreting how larger events influence movement across the city.

### Mapping the City’s Pulse

<div style="display: flex; justify-content: center; margin-bottom: 20px;">
  <div class="image-container">
    <iframe src="html_templates\nyc_subway_heatmap.html" width="600px" height="550px" style="border:none; margin-bottom: 20px;" title="Subway Ridership Heatmap: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-left:5px; margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 1:</strong> Heatmap illustrating subway ridership density across New York City, highlighting areas of concentrated activity.
  </p>
</div>

The heatmap in **Figure 1** captures ridership density across the subway system. As expected, Manhattan acts as the nucleus of subway traffic, pulsing with high-density flows, especially near business and tourism hubs.


### Borough-Level Ridership: Who Moves the Most?

To better understand how New Yorkers interact with the subway system, we examine both borough-level ridership patterns and the typical flow of commuters throughout the day.

We can now explore how the city uses the subway system across different boroughs and how ridership is distributed throughout the day.

<div style="display: flex; justify-content: center; margin-bottom: 20px;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures\Polar_Chart.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 2:</strong> The polar chart visualizes the total subway ridership by borough in New York City
  </p>
</div>

The plar chart in **Figure 2** confirms that Manhattan dominates subway usage, due to its concentration of offices, attractions, and transfer hubs. Brooklyn follows, while Staten Island and The Bronx show significantly lower ridership. The borough-level data aligns closely with the patterns seen in the heatmap in **Figure 1**, reinforcing Manhattan’s centrality in daily movement.

### Temporal Patterns: A Day in the Life of the Subway

<div style="display: flex; justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/Histogram.png" style="width: 200%;  margin-bottom: 10px;">
  </div>
</div>
<strong>Figure 3:</strong> The histogram shows the distribution of subway ridership across different hours of the day. 

In **Figure 3**, we see that subway activity starts rising sharply around 6 AM, aligned with the morning rush hour. Ridership peaks at 5 PM, during the evening commute, and then declines rapidly after midnight. The drop between 1 AM and 4 AM reflects the few hours when the city—and its commuters—finally rest, despite New York’s *“city that never sleeps”* reputation.

By understanding these baseline behaviors—where and when the subway is used, we establish a reference point for detecting anomalies caused by events and incidents. The next act will explore how specific moments (festive or stressful) reshape this daily rhythm.

## ACT II : When the City Celebrates, the Subway Becomes a Party

Large-scale city celebrations don’t just bring joy, they also transform mobility. During such moments, the subway acts as both a lifeline and a pressure valve, adapting to surges in human movement. In this section, we examine two of New York’s most iconic events: the New York City Marathon and New Year’s Eve in Times Square. Both reshape ridership patterns in unique ways, offering a window into how the subway supports, and strains under, the weight of collective celebration.

### New York City Marathon
Held every first Sunday in November, the [New York City Marathon](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory) attracts over 50,000 runners and nearly two million spectators, spanning all five boroughs. The subway becomes the artery through which runners, volunteers, and fans reach the course—especially in and around Central Park, where the race ends.

Stations like 59 St–Columbus Circle and 72 St see 30–40% more traffic compared to a regular Sunday.

<!--
<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\marathon_heatmap.html" width="1200" height="900" style="border:none;" title="Subway Ridership Heatmap: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 4:</strong> Heatmap showing hourly subway ridership on Marathon Sunday, with emphasis on stations along or near the race route.
  </p>
</div>
-->

In this interactive plot in **Figure 4**, we can explore how ridership is distributed throughout the day of the marathon.

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\stations_line_plot.html" width="1120" height="950" style="border:none;" title="Stations Ridership Line Plot: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 4:</strong> Line plot comparing hourly ridership at key subway stations on Marathon Sunday, illustrating patterns of crowd movement and station activity throughout the day.
  </p>
</div>

**Figure 4** reveals several key observations:
- **Early Morning (5-7 AM):** Runners travels to Staten Island for the starting line.
- **Late Morning to Early Afternoon (10 AM-2 PM):** Peak spectator traffic heading toward cheer zones. 
- **Evening (after 5 PM):** Noticeable decline in usage as the event concludes and crowds dissipate. 

The marathon began in 1970 with just 127 participants running loops around Central Park. Today, it’s the world’s largest marathon, a logistical feat that reorients the entire city’s flow for a single day. [Read more about the history here](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory).<!-- ([TCS New York City Marathon](https://www.worldmarathonmajors.com/six-star-major/new-york-city), [New York City Marathon History](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory)). -->

<!--But why has marathon running surged in popularity? Beyond the challenge, many are drawn to the structure, community, and personal growth it offers. The pandemic era, in particular, saw a boom in running as people sought connection and purpose. Platforms like TikTok have further fuelled this trend, turning marathon training into a shared journey. 

*Explore more about this phenomenon in [this insightful article](https://www.axios.com/2024/05/08/marathon-running-training-tiktok). ([Why Marathon Running Is Booming - WSJ](https://www.wsj.com/lifestyle/fitness/marathon-increasing-popularity-2025-caac1bb6), [Axios Finish Line: Why more people are running marathons](https://www.axios.com/2024/05/08/marathon-running-training-tiktok)).* -->

---

### New Year’s Eve – The Ultimate Subway Stress Test

When the ball drops in Times Square, so do the boundaries of normal subway operations. December 31 consistently produces one of the highest ridership spikes of the year—while January 1 shows one of the steepest drop-offs.

Key stations like Times Sq–42 St, 42 St–Port Authority, and 34 St–Penn Station become critical junctions as hundreds of thousands pour into Midtown.

We explore before and after midnight "A Tale of Two Days" in **Figure 5**

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates/nye_timeseries.html" width="920" height="625" style="border:none;" title="New Year's Eve Subway Ridership – Hourly Trend (Dec 31 vs Jan 1)"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 5:</strong> Hourly subway ridership trends on New Year's Eve (Dec 31) vs. New Year's Day (Jan 1), highlighting changes in travel behaviour around midnight.
  </p>
</div>

From **Figure 5**, we can extract distinct ridership behaviors:

<div class="narrative-columns">
  <div class="narrative-container">
    New Year’s Eve (Yellow Line):
    <ul>
      <li><strong>11 PM-1 AM: </strong> Massive ridership spike as crowds converge on Times Square.</li>
      <li><strong>1-3 AM</strong> Late-night services see 2.5× more passengers than on a regular Saturday.</li>
      <li>Lines <strong>1, 2, N, Q, R, A, C, and E</strong> carry the bulk of the load—especially around Midtown.</li>
    </ul>
  </div>

  <div class="narrative-container">
    New Year’s Day (Blue Line):
    <ul>
      <li><strong>Early morning (1 AM-12 PM):</strong> Ridership plummets to 40–50% below normal Sunday levels.</li>
      <li><strong>Afternoon:</strong> A gradual recovery begins, mirroring the city's slower awakening after the festivities.</li>
    </ul>
  </div>
</div>

Celebrations like the Marathon and New Year’s Eve vividly show the subway’s dual role: it must enable celebration while absorbing intense and temporary demand shocks. These events stretch the system in unique ways, revealing both its capacity and its vulnerabilities.

<!--
For New years eve (the yellow line) we can following:
* A dramatic spike in ridership from 11 PM to 1 AM, as revelers flood into Midtown to secure a view of the countdown.
* Late-night services (1–3 AM) experience ridership surges up to 2.5× higher than a typical Saturday night.
* The 1, 2, N, Q, R, and A/C/E lines show the heaviest traffic during this window, especially near Times Square and Columbus Circle.

But then comes the New Year’s Day (the blue line) we have these observations: 
* Ridership drops 40–50% below normal Sunday levels, particularly before noon.
* Uptown-bound stations remain unusually quiet until mid-afternoon, as the city slowly reawakens.

This dramatic peak-and-crash pattern makes New Year’s Eve one of the most extreme shifts in the entire ridership dataset.


### The Cultural Pulse of Midnight in Midtown

New Year’s Eve in New York is more than just a party—it is a city-wide ritual. With over a million people cramming into the blocks around Times Square (per [NYPD estimates](https://www.nytimes.com/2023/12/31/nyregion/times-square-new-years-eve.html)), the MTA becomes the only practical way in and out. The subway does not just reflect the party—it enables it.

Even in years affected by pandemic restrictions, data shows a smaller but still visible spike, suggesting the deep cultural grip of this annual celebration.

*Want to learn more about the infrastructure that makes this night possible? See this behind-the-scenes feature on [how NYC manages crowd control and transit for New Year’s Eve](https://gothamist.com/news/heres-how-nyc-prepares-for-new-years-eve-in-times-square).*

[comment]: <> (*Visual idea: A map of protest locations with ridership changes at nearby stations.* / title="Subway Ridership Change During Protest Events (Brooklyn & Midtown) )
-->

---

## Act III: When the City Struggles – The Subway Feels It

When the city is under stress, whether human, technical, or environmental, the subway feels it. The MTA’s incident data offers a window into how disruptions ripple through the system and reflect deeper vulnerabilities in New York's urban infrastructure.

This section draws from monthly data on reported subway incidents from 2020 to 2024, helping us understand how and when the system is most fragile.

---

### The Pulse of Disruption: Monthly Incident Trends
We begin by examining how major incident categories evolve over time. The heatmap in **Figure 6** shows the temporal distribution of disruptions, with notable seasonal and categorical patterns.

<div style="display: flex; justify-content: center; align-items: center;">
  <img src="Figures/Heatmap_incidents.png" style="width: 150%">
</div>
<strong>Figure 6:</strong> Heatmap of NYC subway incident frequency by category (2020–2024).

To interpret the patterns meaningfully, here’s a quick breakdown of what each category represents:

<table style="width: 100%; border-collapse: collapse;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="text-align: left; padding: 8px;">Incident</th>
      <th style="text-align: left; padding: 8px;">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding: 8px;"><strong>Track</strong></td>
      <td style="padding: 8px;">Problems involving the rail infrastructure—like obstructions, debris, or damage.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Signals</strong></td>
      <td style="padding: 8px;">Failures in systems that control train movement, often due to aging infrastructure or congestion.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Persons on Trackbed / Police / Medical</strong></td>
      <td style="padding: 8px;">Emergencies involving people on the tracks, law enforcement, or medical response.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Stations and Structure</strong></td>
      <td style="padding: 8px;">Incidents related to station facilities, power outages, or broken equipment.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Subway Car</strong></td>
      <td style="padding: 8px;">Mechanical faults on the trains—like doors, brakes, or ventilation systems.</td>
    </tr>
    <tr>
      <td style="padding: 8px;"><strong>Other</strong></td>
      <td style="padding: 8px;">Unusual or uncategorized disruptions still affecting normal subway operations.</td>
    </tr>
  </tbody>
</table>

Notable Takeaways:
- "Persons on trackbed / Police / Medical" incidents are the most frequent and disruptive, often reflecting emergencies, vulnerable populations, or mental health crises.
- "Signals" issues remain a persistent technical challenge, often linked to aging infrastructure and peak-hour strain.

These two categories represent the dual vulnerability of the subway: one rooted in human unpredictability, the other in infrastructural fatigue.

---

### A City on Pause: The COVID-19 Shadow

One of the most striking patterns appears in **Figure 7**, which marks a sharp drop in reported incidents during early 2020, aligned with the first wave of the ([COVID-19 pandemic in New York City](https://en.wikipedia.org/wiki/COVID-19_pandemic_in_New_York_City)). 

<div style="display: flex; justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/corona_heatmap.png" style="width: 150%">
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 7:</strong> Reduced incident reports during COVID-19 lockdown period (March–May 2020).
  </p>
</div>

As the city slowed to a near-halt, so did its subway. Fewer riders, fewer disruptions. The subway mirrored the stillness of the streets above.

---

### Highs and Lows: When Disruptions Spike (or Subside)

To better understand the extremes, **Figure 8** compares the two highest and two lowest incident months in 2024. This seasonal lens reveals how external factors—weather, holidays, operations—shape subway resilience.

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\nyc_subway_high_low_months_incidents_2024.html" width="1020" height="720" style="border:none;" title="Incidence monthly occurence "></iframe>
  </div>
  <p style="margin-top: 10px; margin-left: 5px; font-style: italic; color: #555;">
    <strong>Figure 8:</strong> Comparison of the two highest-incident and two lowest-incident months in the NYC subway system during 2024, broken down by incident category.
  </p>
</div>

What we see:

* **December 2024** had the highest number of incidents, likely due to increased traffic during the holiday season, colder weather stressing infrastructure, and more crowd-related disruptions.
* **January 2024** followed closely, possibly driven by harsh winter conditions and early-year operational resets.
* **October 2024** recorded the lowest number of incidents, suggesting a period of relative stability, milder weather, and fewer crowd-based events.
* **June 2024**, the second-lowest, may reflect reduced ridership during early summer breaks or operational improvements during that window.

Across all months, “Persons on Trackbed” and “Signal” problems dominate, signaling ongoing structural and societal tensions.

---

### Disruptions by Line: Where the Pressure Builds

Next, we zoom in on how incidents differ across subway lines and divisions. The NYC subway is split into:
- A Division (numbered lines: 1–7)
- B Division (lettered lines: A–Z)

Each has its own infrastructure, technology, and crowd dynamics. **Figure 9** maps the incident landscape by line and category for 2024.

<div style="display: flex; justify-content: center;">
  <div class="image-container">
    <iframe src="html_templates\nyc_subway_incidents_by_division_line.html" width="1120" height="620" style="border:none;" title="Incidence monthly occurence "></iframe>
  </div>
  <p style="margin-top: 10px; margin-left: 5px; font-style: italic; color: #555;">
    <strong>Figure 9:</strong> Distribution of subway incidents by line and division, categorized by type of incident (2024)
  </p>
</div>

Here we can obser following:

<div class="narrative-columns">
  <div class="narrative-container">
    <h4>A Division:</h4>
    <ul>
      <li><strong>Line 2</strong> reports the highest number of incidents, especially involving “Persons on Trackbed/Police/Medical” and “Other” categories.</li>
      <li><strong>Line 4</strong> is notable for a high number of “Track”-related incidents.</li>
      <li><strong>Line 7</strong> shows a wide distribution of incident types, possibly due to heavy usage and infrastructure strain.</li>
    </ul>
  </div>

  <div class="narrative-container">
    <h4>B Division:</h4>
    <ul>
      <li><strong>Line A</strong> has the most “Track” issues, along with a high number of “Persons on Trackbed/Police/Medical” incidents.</li>
      <li><strong>Line G</strong> records a high number of “Stations and Structure” incidents, likely pointing to aging facilities.</li>
      <li><strong>Lines J/Z</strong> and <strong>Line L</strong> report the second-highest number of “Persons on Trackbed/Police/Medical” incidents in the division.</li>
    </ul>
  </div>
</div>

**Patterns Across Categories:**
- *“Persons on Trackbed/Police/Medical”* incidents are notably high across both divisions, especially on high-traffic lines like 2, A, D, and J/Z.
- *"Signal"* and *"Track"* issues remain a common problem system-wide, supporting the MTA’s ongoing investment in modernization and maintenance.
- *"Stations and Structure"* issues seem disproportionately high in the B Division, especially on G, L, and M lines, potentially due to older infrastructure or less accessibility upgrades.

The data paints a picture of a system deeply interconnected with the city’s rhythms. When things go wrong above ground, be it weather, social strain, or economic pressure—the subway doesn’t just reflect it. It absorbs it.

Where ACT II showed celebration and movement, ACT III shows fatigue, tension, and stress. And yet, even in crisis, the subway continues, mirroring the resilience of the city itself.

---

## Summary 

Across these three acts, the subway emerges not just as a transit system, but as a living reflection of New York City.
It responds to movement, emotion, and crisis. It flows with the morning rush, surges during moments of joy, and falters under pressure. Each train, signal, and crowd movement tells part of the city’s larger story.

Through MTA data, we see the subway as a barometer of urban life, pulsing with energy, shaped by its people, and strained by the same forces that affect the streets above. The subway doesn’t just move people, it reveals what it means to live in a city this complex, intense, and alive.


<!--

### Incidents During Big Events

In the first act of this article, we looked into how if the subway ridership is reflected on bigger events in New York City. Will this also be reflected on the incident reports on the subway?

#### NYC Marathon

<div class="narrative-container">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="Figures/barplot_marathon.png" style="width: 150%">
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    <strong>Figure 8:</strong> Barplot displaying subway incidents over the years.
  </p>
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

[comment]: <> (*Visual idea: A map of protest locations with ridership changes at nearby stations.* / title="Subway Ridership Change During Protest Events (Brooklyn & Midtown) )

These events do not suppress movement—they redistribute it. New Yorkers are famously mobile and adaptable; when paths close, they find others.

*Want to know where the protests went and how the city responded? Read [this overview from Nye York Times](hhttps://www.nytimes.com/2020/05/30/nyregion/nyc-protests-george-floyd.html).*

---

### The Subway Avoidance Effect

Sometimes, fear—not protest—changes the flow.

After the Times Square subway shooting on 10 April 2022, we observed a noticeable dip in ridership at nearby stations:

* Bryant Park–42 St and Times Sq–42 St fell by 12–15% over the following week, despite no formal service disruptions.
* The drop was temporary—but striking. Stations two stops away (e.g., 34 St–Penn Station) saw no such change.

Similarly, during the 2023 Midtown blackout, stations on the F line around Lexington Av/63 St experienced a 24-hour ridership plunge, followed by a delayed return—with some usage patterns never fully recovering.

[comment]: <> (*Visual idea: A bar chart of crime/incident dates vs. ridership drops at affected stations.* / title="Ridership Impact of Disruption Events (Shootings, Blackouts, Repairs) )


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

*Want to dive deeper into the MTA's data and how they use these insights for planning? Check out the latest MTA reports on [subway ridership trends](https://new.mta.info/) and future improvements.*


-->

---

In the end, the subway is more than just a series of stations and tracks—it is a mirror of New York itself. It reflects the city’s chaos, creativity, resilience, and unyielding spirit. And as the data shows, the MTA is not just managing a transit system—it is managing the lifeblood of New York’s mobility.
