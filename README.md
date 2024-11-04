
# Rainfax June Dashboard

Rainfax is an imaginary delivery company based out from Bengaluru. It works as delivery agents for their clients handling the entire delivery cycle from start to end. They have employed runners whose job is collected items from client and delivering it to where ever they want it delivered. Each runner is deployed in different locations ensuring they have proper connectivity. Each runner is assigned different duty and location as per the cycle of delivery. They now have an issue of tracking runners with excel sheets and want a single page power BI dashboard for the month of June which maps all the required data of each runner in an interactive way.

## Preview

![Preview](Rainfax_june.pdf)

![Click here for the pbix file](Rainfax_June.pbix)

## Requirements

•	A single page interactive power bi dashboard which shows important details regarding file collection for each runner.

•	Runners join and leave in between so the dashboard will have to map that automatically and map the days present and absent through cards.

•	Build a Gauge chart to map the issues caused my each runner in the respective month.

•	Name of the Runner selected by the slicer has to be shown at the top of the dashboard.

•	There is two slots A and B for each runner per day, Show the total Collection during A and B through cards. Also mention the time for each runner of both A and B slot through cards. Make sure the time is formatted properly.

•	The count of files for each slot is 8 and total percentage above 89% so map values of each runner and his verdict that is good or bad collection. Calculate the percentage as well. Map a card for the total verdict for a whole month for each runner as well.

•	Create a line chart with tooltips for A, B and total count of collection of files for each day for each runner as per the slicer. Create a scatter chart for percentage collection and a donut chart with actual count and required count as per the required value given.

## Process

### Data Cleaning and Transformation

•	Cleaning the excel sheet provided by filling out the missing values with the median of the respective column and removed all the unnecessary columns.

•	Appending the columns for each runner for all the 31 days for the month of July.

•	Changing the data type of the time columns. Creating a new column to add the counts of A and B slot for each runner each day using advance excel formulas.

•	Created a column which resulted in good or bad as a verdict by comparing the total file count and the value given by the company for each slot. Created a column for percentage and percentage verdict according to the value given by the company.

•	Created another worksheet to store the total value for each runner for the whole month combined with the following set of columns:

o Runner Name: Name of each runner.

o	AADT: A slot arrival time.

o	AAFDT: B slot arrival time.

o	Days_Present: Number of days each runner is present in a month.

o	Days_Absent: Number of days each runner is absent in a month.

o	Percentage, OG Verdict, Issue count – To calculate percentage, Total verdict and issue count.

o	CA, CB, CA_Max, CB_Max, CA_Perc, CB_Perc – Total collection of files for June for A slot, B slot, and Max collection required for both slots, Percentage collection for both slots.

o	CA_V, CB_V, Percentage Contribution – Total verdict and percentage contribution.

### Data Visualization

•	Loaded two sheets to power BI, Made all the necessary transformation and then loaded the data.

•	Created a slicer with runner name, a gauge chart to find issue count for each runner and a card showing total verdict for the selected runner.

•	A line chart, a scatter char and a donut chart was made as per the requirements.

•	All the insights asked for was mapped as cards in power BI.

## Conclusion & Insights

•	Significant number of absentees in the month of June.

•	Shashank Jois and Praveen KM had bad collection verdict for the month of June.

•	Sharath Kumar had the highest percentage collection for the month of June.

•	Cherun SP and Nagendra Prasad caused the highest amount of issues for the month of June.

•	Hruthviraj and Kanaj Kumar have highest collections in A and B slot respectively for the month of June.

•	All the runners had good verdict in A slot and Naeem Pasha, Shashank Jois, Naveen KM and Theja had bad collection for B slot.

•	Hruthviraj, Kanaj Kumar and Sharath Kumar have the highest file contribution for the month of June.

## Inspiration

When I was working as a data analyst in an AI / ML startup, I was handling a task similar to this for each month where we worked on the AI devices that were used in different client location. We were tasked to map the data collection and accuracy through Power BI, MYSQL and Python. This project is an inspiration and a spin off from what I was working on in the company.


