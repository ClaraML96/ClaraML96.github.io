---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home

---

# **How New York’s Subway Ridership Dances to the Rhythm of the City**

New York City’s subway system is more than just a means of transportation—it is a living, breathing reflection of the city's dynamic pulse. Every fluctuation in ridership tells a story about what is happening above ground. From the exuberant influx of marathon runners to the quiet lulls following major incidents, the subway responds in real-time to the city's events.

In this data story, we delve into the intricate relationship between the city's happenings and subway usage. Utilizing **Hourly Ridership Data (2020–2024)** and **Major Subway Incident Reports (2020–2024)** datasets, we explore how planned events like the [New York City Marathon](https://www.nyrr.org/tcsnycmarathon) and spontaneous occurrences such as protests or severe weather conditions influence the ebb and flow of commuters. Our analysis reveals patterns that not only highlight the subway's responsiveness but also offer insights into the city's resilience and adaptability.

Join us as we uncover the narratives hidden within the numbers, illustrating how the subway serves as a barometer for New York City's ever-changing landscape.

---

## **When the City Celebrates, the Subway Becomes a Party**

### **New York City Marathon**
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
    <iframe src="html_templates\stations_line_plot.html" width="1150" height="950" style="border:none;" title="Stations Ridership Line Plot: Marathon Sunday with Key Stations"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    Figure 2: Line plot comparing hourly ridership at key subway stations on Marathon Sunday, illustrating patterns of crowd movement and station activity throughout the day.
  </p>
</div>

The New York City Marathon is not just a race; it is a storied tradition. Starting in 1970 with just 127 participants looping around Central Park, it has evolved into the world's largest marathon, weaving through all five boroughs and drawing nearly two million spectators annually. For a detailed look at its rich history, visit the [official NYRR Marathon history page](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory). ([TCS New York City Marathon](https://www.worldmarathonmajors.com/six-star-major/new-york-city), [New York City Marathon History](https://www.nyrr.org/tcsnycmarathon/getinspired/marathonhistory)).

But why has marathon running surged in popularity? Beyond the challenge, many are drawn to the structure, community, and personal growth it offers. The pandemic era, in particular, saw a boom in running as people sought connection and purpose. Platforms like TikTok have further fuelled this trend, turning marathon training into a shared journey. Explore more about this phenomenon in [this insightful article](https://www.axios.com/2024/05/08/marathon-running-training-tiktok). ([Why Marathon Running Is Booming - WSJ](https://www.wsj.com/lifestyle/fitness/marathon-increasing-popularity-2025-caac1bb6), [Axios Finish Line: Why more people are running marathons](https://www.axios.com/2024/05/08/marathon-running-training-tiktok)).

---

### **New Year’s Eve – The Ultimate Subway Stress Test**

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
    <iframe src="html_templates/nye_timeseries.html" width="950" height="850" style="border:none;" title="New Year's Eve Subway Ridership – Hourly Trend (Dec 31 vs Jan 1)"></iframe>
  </div>
  <p style="margin-top: 10px; font-style: italic; color: #555;">
    Figure 3: Hourly subway ridership trends on New Year's Eve (Dec 31) vs. New Year's Day (Jan 1), highlighting changes in travel behaviour around midnight.
  </p>
</div>

### The Cultural Pulse of Midnight in Midtown

New Year’s Eve in New York is more than just a party—it is a city-wide ritual. With over a million people cramming into the blocks around Times Square (per [NYPD estimates](https://www.nytimes.com/2023/12/31/nyregion/times-square-new-years-eve.html)), the MTA becomes the only practical way in and out. The subway does not just reflect the party—it enables it.

Even in years affected by pandemic restrictions, data shows a smaller but still visible spike, suggesting the deep cultural grip of this annual celebration.

Want to learn more about the infrastructure that makes this night possible? See this behind-the-scenes feature on [how NYC manages crowd control and transit for New Year’s Eve](https://gothamist.com/news/heres-how-nyc-prepares-for-new-years-eve-in-times-square).




### **New Year’s Eve**  
When the clock strikes midnight in Times Square, the subway faces its biggest crowd surge of the year.

**DATA VISUALIZATION** *A before/after line chart showing NYE ridership vs. recovery the next day.*  

**Our data shows:** INPUT ANALYSIS OF RIDERSHIP
- **42 St-Port Authority** sees **triple its usual ridership** as revellers pour in.  
- **Late-night trains (1-3 AM)** are **50% busier** than an average Saturday.  
- But here’s the twist: **New Year’s Day** sees a **ridership crash**—because half the city is asleep by noon.

---

## **When the City Struggles**  

### **Incidents During Big Events**
Are celebrations linked to more disruptions?

**DATA VISULIZATION** 
- Incident timelines over Marathon & NYE
- Breakdown by incident type (e.g. crowding, medical, delays)

**Our dara shows:**
- Small spikes in medical/police-related incidents on NYE
- Minimal incidents on Marathon day - Has it gotten better over the years?


### **Weather Extremes vs. Subway Usage**
Snowstorms, heatwaves, and their underground echoes

**DATA VISULIZATION** 
- Scatter plot: temperature vs. ridership
- Annotated extremes (e.g. Jan 2022 snowstorm, July 2023 heatwave)

**Our dara shows:**
- Snow creates a big drop in Bronx/Queens ridership (outer boroughs)?
- Heat creates an increase in subway use (walking becomes unbearable)

### **9/11**  

**DATA VISULIZATION** 

**Our dara shows:** INPUT ANALYSIS OF Incidents
- **ipsum lorem** ipsum lorem
- **ipsum lorem** ipsum lorem  

---

## **System Under Stress**  
Using incident reports as a health monitor for the system

**DATA VISULIZATION** 
- *Monthly line chart of total incidents*  
- *Layered with key public events (e.g. COVID waves, protests, reopenings)*

**Our dara shows:** INPUT ANALYSIS OF Incidents
- Disruption dip in early COVID months (low ridership)
- Rebound in 2021–2022, but incident types shift
- Signals and mechanical issues rise as operations normalize
 
---

## **Conclusion: The Subway as New York’s Mirror**
Through these datasets, we see how the subway adapts, suffers, and recovers - just like the city it serves. From joyous marathons to snowy shutdowns, each turnstile click and incident log is a data point in New York's ongoing story. 
