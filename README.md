# J124-Final

# Story Pitch
## Summary
Data support that West Oakland has the greatest amount of diesel particulate matter (PM) emissions at 10.41 tons per year in comparison to the rest of Oakland. Diesel PM most often comes from trucks, ships, buses, and cars. In 1963, an [ordinance](https://dot.ca.gov/programs/traffic-operations/legal-truck-access/restrict-route-580) was passed prohibiting trucks weighing more than 4.5 tons from traveling on I-580, a prominent Oakland freeway. This consequently pushes large trucks to travel on I-880, another prominent Oakland freeway, where the surrounding neighborhoods of West and East Oakland consist of mostly people of color. In addition to the disproportionate exposure to current traffic-caused air pollutants, these communities have a greater health burden due to historical systemic barriers like redlining, which situated people of color near places high in pollutants. In addition to redlining, these neighborhoods deal with health disparities that have resulted from barriers such as medical mistrust, a greater likelihood to be uninsured, lower income, and lower educational attainment. When combined, these barriers form a greater health burden. The data support the need for investigation into the 1963 ordinance, current barriers, and solutions for decreasing air pollution and improving health for these communities.

With West Oakland, large trucks not only primarily travel on I-880, but they also cut through the neighborhood streets to transport cargo to the nearby Port of Oakland, further exposing residents to pollutants. Concentrations of black carbon along I-880 are roughly 80% higher than average concentrations along I-580, further showing environmental disparities [(Environmental Defense Fund)](https://www.edf.org/airqualitymaps/oakland/tale-two-freeways). Making up a significant portion of diesel PM, black carbon has been linked to cardiovascular diseases, respiratory diseases, and cancer. Long-term exposure is also associated with all-cause and cardiovascular mortality [(Yang et al.)](https://www.sciencedirect.com/science/article/pii/S016041202100430X?via%3Dihub). On average, residents living within 10 miles of I-880 have twice the cancer risk and are nearly twice as likely to develop respiratory illnesses than those living within 10 miles of I-580 [(Glover)](https://abc7news.com/west-oakland-air-pollution-black-and-latino-residents-abc-equity-report-bay-area-quality/11058102/). Data analyses show higher rate of emergency department visits for heart attacks and asthma in West and East Oakland—more so in East Oakland, which may be partially attributable to its proximity to the airport and can be further analyzed. 


## Data Sources Used
### CalEnviro Screen 4.0
* [Website](https://calenviroscreen-oehha.hub.arcgis.com/)
* [Data Download Page](https://calenviroscreen-oehha.hub.arcgis.com/documents/be09f14bef6244e8af4da6aeed89ec03/about)
* [My Sheets + Data from Questions](https://docs.google.com/spreadsheets/d/1cr5x867EFzqWaoWRUPhzBA8yon8mgeRPIO9JRlD5MDQ/edit?usp=sharing)

## Potential Sources
### Margaret Gordon
* Gordon is a community activist, a West Oakland resident since 1992, and co-director of the West Oakland Environmental Indicators Project(WOEIP), which works to increase public health and environmental justice awareness. Gordon would be an ideal source to interview as a resident herself and to help gain insight into what the WOEIP-provided advocacy tools, research, and political education look like for West Oakland residents.
* Contact information
  * (510)257-5640
  * margaret.woeip@gmail.com
### Adrian James
* Dr. James is the Chief Medical Officer and primary care physician at West Oakland Health. Having worked at West Oakland Health since 1994, Dr. Apte has a unique perspective of West Oakland’s needs and health outcomes—especially over time—that would add local health expertise to the story.
* Contact information
	* (510)835-9610 ext.3660
	* adrianj@wohc.org
### Joshua Apte
* Dr. Apte is a professor of Civil and Environmental Engineering at UC Berkeley whose research focuses on air pollution and reducing inequities in environmental contaminant exposure in low-resource communities. Dr. Apte would be an ideal source to interview to better understand the scope of environmental racism and air pollution disparities in areas of historical redlining—areas in which he has done research.
* Contact information
	* apte@berkeley.edu

## Additional Sources
### “Owning Our Air: The West Oakland Community Action Plan Volume 1”
(https://www.baaqmd.gov/~/media/files/ab617-community-health/west-oakland/100219-files/final-plan-vol-1-100219-pdf.pdf?la=en) 
* This report details the disproportionate air pollution and health disparities experienced by West Oakland residents. This report is useful due to the large number and variety of stakeholders—especially the residents that make up the community itself—involved to generate a plan for pollution reduction in West Oakland. The report details the major sources of air pollution in that neighborhood, which contributes heavily to the research aspect of reporting. Additionally, the report details the disparities in health outcomes, ranging from increased cancer risk to asthma emergency room visits.
### “Association between Traffic Related Air Pollution Exposure and Direct Health Care Costs in Northern California” by Stacey E. Alexeeff, Ananya Roy, Jun Shan, G. Thomas Ray, Charles Q. Quesenberry, Joshua Apte, Christopher J. Portier, Stephen K. Van Den Eeden
(https://doi.org/10.1016/j.atmosenv.2022.119271)
* This research finds that exposure to traffic pollution increases the costs of health care for Northern California elderly residents with greater costs due to outpatient fees and emergency room visits. This research supports the high rates of emergency department visits for heart attacks and asthma observed in this project’s data analyses. It would also be a good starting point for the data collection and analysis of health care costs for non-elderly residents, especially children.


# Data Visualization
![datawrapper](https://github.com/kmiglesias/J124-Final/assets/140004469/c962df9a-3b67-4989-a6ac-4cb006b87a7a)
[Link to interactive](https://datawrapper.dwcdn.net/BVIvx/1/)


# Data Analysis Questions
Note: Before any questions were completed, the downloaded spreadsheet was filtered to only include data for the cities of Oakland and Piedmont (a city that is surrounded by Oakland and shares zip codes). This was done by duplicating the original spreadsheet (“CES4.0FINAL_RESULTS”) onto a new sheet titled “Oakland Filtered.” The column “Approximate Location” was filtered to show Oakland and Piedmont, and the remaining rows with data from other cities were removed. All other column data was kept.

## 1. Which Oakland zip code has the highest amount of diesel particulate matter emissions (tons/year)? Which zip code has the least?
#### 94607 has the highest amount of diesel particulate matter emissions, while 94613 has the least.
![/J124_Ques1Answer.png)](https://github.com/kmiglesias/J124-Final/blob/main/J124_Ques1Answer.png)


#### Process
1. Using the “Oakland Filtered” sheet, click “Insert” and select “Pivot Table.” Make sure the data range includes the whole sheet and reads, “'Oakland Filtered'!A1:BF342.” Under “Insert to,” select “New sheet” — which should be the default.
2. In the pivot table editor unde “Filters,” select the “Clear” option in blue. Search “946” and select all the zip codes that begin with that. There should be 15 total that were available from this dataset.
3. Under “Rows,” select “ZIP” for the zip codes.
4. Under “Values,” select “Diesel PM.”
5. In the “ZIP” box from Step 3, change the option under “Order” from “Ascending” to “Descending.” Then change the option under “Sort by” from “ZIP” to “SUM of Diesel PM.”

## 2. What is the percent difference in diesel particulate matter emissions between the zip code with the most and the zip code with the least?
#### There is a 185.70% difference in diesel particulate matter emissions between the zip code with the most (94607) and the zip code with the least (94613).

#### Process
1. Using the pivot table from Question 1, copy and paste the top and bottom values (which should be for the zip codes 94607 and 94613) into a new sheet.
2. In a new column, calculate the percent difference between the two diesel PM values using the formula “=(ABS(B2-B3))/((B2+B3)/2).”
3. Clicking the new value that results from that formula, click “Format,” then “Number,” and finally, “Percent.”
![J124_Q2Process.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q2Process.png)

## 3. What is the percentage of people of color in the zip codes with the highest and lowest amount of diesel particulate matter emissions?
#### 74.29% of people in 94607 are people of color. 68.84% are people of color in 94613.

#### Process
1. Copy the first 5 columns (Census Tract, Total Population, California County, ZIP, and Approximate Location) from “Oakland Filtered” to a new sheet. 
![J124_Q3P1.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q3P1.png)

2. In the new sheet, use the formula “=VLOOKUP(A2, 'Demographic Profile'!$A$4:$O$363, 11, FALSE)” in a new column in the second cell (F2). This connects the new sheet to the sheet called “Demographic Profile” that comes with the original downloaded dataset. Double-click the corner of the cell to fill the rest of the column. This new column returns the percentage of white people per census tract.

![J124_Q3P2.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q3P2.png)

3. Label the VLOOKUP column “% White.” For the next column, write the formula “100-F:F). That returns the percentage of non-white people or people of color. Note: The category of “Other/Multiple” was included as people of color because the database dictionary definites the category as “2019 ACS population estimates of the percent per census tract of those who identify as non-Hispanic ‘other’ or as multiple races.”

![J124_Q3P3.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q3P3.png)

4. Create a pivot table using this sheet. Use “ZIP” for the rows and “%BIPOC” for the values. For the values, summarize by “AVERAGE.” Optional for curiosity purposes: Order by descending values, and sort by the “AVERAGE of %BIPOC” for the “ZIP” box to see which zip codes have the largest and smallest BIPOC populations.

![J124_Q3P4.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q3P4.png)

5. Going back to Question 1, the zip code 94607 has the highest amount of diesel particulate matter emissions, while 94613 has the least. The zip code 94618 has the second lowest amount of diesel particulate matter emissions. This zip code was included because 94613 is a very small zip code area mainly encompassing the Mills College campus, which may be an outlier in the dataset. Filter the pivot table to show only 94607, 94613, and 94618.
![J124_Q3P5.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q3P5.png)

## 4. Which census tract and zip code has the highest age-adjusted rate of emergency department visits for asthma? 
#### Census tract 6001410300/zip code 94603 has the highest age-adjusted rate of emergency department visits for asthma at 226.34.

#### Process
1. Create a pivot table from “Oakland Filtered.”
2. Use “Census Tract” and “ZIP” for the rows.
3. Use “Asthma” for the values.
4. Order the census tract in descending order and sort by the “SUM of Asthma.”
![J124_Q4.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q4.png)

5. Optional: See the data by zip code by looking at the average.
![J124_Q4Optional.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q4Optional.png)

## 5. Which census tract and zip code has the highest age-adjusted rate of emergency department visits for heart attacks (per 10,000)?
#### Census tract 6001409500/zip code 94621 had the highest age-adjusted rate of emergency department visits for heart attacks at 21 per 10,000.

#### Process
1. Create a pivot table from “Oakland Filtered.”
2. Use “Census Tract” and “ZIP” for the rows.
3. Use “Cardiovascular Disease” for the values.
4. Order the census tract in descending order and sort by the “SUM of Cardiovascular Disease.”
![J124_Q5.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q5.png)

5. Optional: See the data by zip code by looking at the average.
![J124_Q5Optional.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q5Optional.png)

## 6. What is the average percent of the population living below two times the federal poverty level for each zip code?
![J124_Q6.png](https://github.com/kmiglesias/J124-Final/blob/main/J124_Q6.png)

#### Process
1. Create a pivot table from “Oakland Filtered.”
2. Use “ZIP” for the rows.
3. Use “Poverty” for the values.
4. Order the zip codes in descending order and sort by the “AVERAGE of Poverty.”
