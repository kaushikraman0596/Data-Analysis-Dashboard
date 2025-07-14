# Data-Analysis-Dashboard
Crime Trends Analysis in Vancouver (2003–2017)
Crime Trends Analysis in Vancouver (2003–2017)

Project Title
Crime Trends Analysis in Vancouver (2003–2017)
Introduction
Crime prevention and community safety are critical concerns for urban centers around the world. Vancouver, a major metropolitan city in Canada, has faced persistent challenges with crime incidents ranging from property theft to violent offenses. Understanding the spatial and temporal trends of crime is essential for effective policing, urban planning, and public safety policy.

This report analyzes over 530,000 police-reported crime incidents in Vancouver between 2003 and 2017, using open data from the Vancouver Police Department via the City of Vancouver’s Open Data Catalogue. The goal is to uncover patterns in crime over time, identify hotspot neighbourhoods, and reveal the distribution of crime types.

By transforming raw incident data into actionable insights, this project supports evidence-based decision-making by law enforcement, city planners, policymakers, and community organizations. This data-driven approach aims to improve resource allocation, inform urban design for crime prevention, and increase public awareness, ultimately fostering a safer and more resilient Vancouver.
Business Impact
Crime imposes significant social, economic, and psychological costs on communities. For municipal governments and law enforcement agencies, strategically reducing crime rates can save millions in policing costs, reduce victimization, and enhance overall quality of life.

This analysis provides several key benefits.

1. Optimized Resource Allocation. By identifying crime hotspots and peak times, the Vancouver Police Department (VPD) can allocate patrol units more efficiently, reducing response times and deterring offenses in high-risk areas.

2. Informed Urban Planning. City planners can use geographic crime patterns to guide improvements in lighting, surveillance infrastructure, and environmental design, adopting principles of Crime Prevention Through Environmental Design (CPTED).

3. Community Engagement and Safety Awareness. Residents and local businesses can better understand crime risks in their neighbourhoods, enabling proactive measures such as neighbourhood watch programs, improved property security, and targeted outreach.

4. Data-Driven Policymaking. Policy analysts and municipal decision-makers can base strategies on empirical evidence rather than anecdotal perceptions, ensuring interventions are equitable and effective.

By transforming a large, complex dataset into accessible insights, this project empowers diverse stakeholders to work collaboratively toward a safer, smarter, and more responsive city environment.
Data
The analysis relies on the Crime in Vancouver dataset originally hosted on Kaggle and derived from the City of Vancouver Open Data Catalogue.

Source: Vancouver Police Department (via Open Data)
License: Open Government License / Open Database License
Coverage: January 2003 to mid-2017
Size: Approximately 530,000 crime incident records

Key Variables
- TYPE: Crime category (for example, Theft from Vehicle, Assault, Mischief)
- YEAR, MONTH, DAY, HOUR, MINUTE: Date and time of incident
- HUNDRED_BLOCK: Approximate street address (anonymized)
- NEIGHBOURHOOD: Vancouver neighbourhood where crime occurred
- Latitude and Longitude: Geographic coordinates for mapping
Strengths of the Dataset
- Large temporal range (over 14 years)
- Detailed location data enabling geospatial analysis
- Broad crime type coverage
Limitations
- Missing or “Null” neighbourhoods for some records
- No demographic details about offenders or victims
- No qualitative narratives about incidents
Data Analysis and Computation
1. Data Cleaning and Preparation
- Removed duplicates and checked for corrupt rows.
- Parsed date and time fields to create usable datetime formats.
- Standardized crime type labels to correct for inconsistent naming.
- Identified and flagged missing neighbourhood data (noting the high “Null” count observed in initial dashboards).
2. Exploratory Data Analysis (EDA)
- Distribution of crime types showed that theft-related offenses (such as Theft from Vehicle and Other Theft) were the largest categories.
- Temporal trends were charted, showing annual crime counts from 2003 to 2017 with a significant decline of around 50 percent over the period.
- Hourly patterns revealed peaks during evening hours for certain offenses.
3. Visualization in Tableau
A multi-component dashboard was developed to make findings accessible.
a. Street-Level Hotspot Map
- Plotted crimes using latitude and longitude on a city map.
- Density heatmap revealed clear clusters, particularly in Downtown, East Vancouver, and commercial corridors.
- Visual hotspots correspond to known high-activity zones, informing patrol planning and urban design needs.
b. Crime by Neighbourhood Bar Chart
- Compared total incidents across neighbourhoods.
- Top areas included Downtown, Fairview, Grandview-Woodland, and Strathcona.
- A large “Null” category highlighted data quality issues requiring cautious interpretation.
c. Crime Type Comparison Over Time
- Stacked area chart of crime counts by year and type.
- Visualized the sharp decline in overall crime from 2003 to approximately 2011, followed by stabilization.
- Showed relative proportions of different crime types over time.
d. Filters and Interactivity
- Dashboard included filters for year range, neighbourhood, and crime type.
- Enabled users to explore specific questions such as “Which neighbourhoods had rising assaults after 2010?”
4. Key Insights
- Long-term Decline. Overall crime fell significantly between 2003 and 2017, suggesting successful policing and community strategies.
- Persistent Hotspots. Downtown, East Vancouver, and some arterial streets maintained high crime densities despite overall declines.
- Dominance of Property Crime. Theft from Vehicle and Other Theft were consistently the most frequent types, highlighting the need for targeted theft-prevention strategies.
- Data Quality Challenge. The high number of “Null” neighbourhood entries suggests that future data collection should improve address accuracy.
Conclusion and Future Work
This analysis confirms that crime in Vancouver has declined substantially over the studied period, while also identifying persistent spatial concentrations and crime type patterns that merit targeted intervention. By providing a clear view of where, when, and what crimes are most prevalent, this report offers actionable insights for public safety stakeholders.

Key recommendations include:
1. Prioritize patrol resources in identified hotspot areas, particularly during peak hours.
2. Focus theft-prevention campaigns in neighbourhoods with high property crime rates.
3. Incorporate CPTED principles in urban design for hotspots.
4. Address data gaps by improving neighbourhood-level address recording to reduce “Null” values.
5. Maintain public dashboards to promote transparency and community engagement.

Future work could expand on this analysis by:
1. Integrating socio-economic and demographic data to identify structural risk factors.
2. Developing predictive models to forecast crime hotspots based on historical trends.
3. Evaluating policing interventions over time to measure their impact.
4. Including post-2017 data to capture recent trends and assess whether patterns have changed.

By continuing to invest in data-driven public safety analysis, Vancouver can support smarter, more effective crime prevention strategies, enhancing safety and quality of life for all its residents.











