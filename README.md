# Latvia-Bike-Usage-Analysis
Latvia Bike Usage Analysis - Power BI Dashboard 🚴‍♂️📊

📢 Project Overview

This project provides an interactive Power BI dashboard that analyzes bike usage trends in Latvia using real-world data. The dashboard includes key insights into seasonal patterns, weather impact, hourly trends, and city-wise rentals, focusing on Riga and other major cities.

📊 Key Features & Visuals

🚴 Bike Rentals Over Time → Line chart showing daily/monthly trends.

🌦️ Weather Impact on Bike Usage → Bar chart comparing bike rentals on clear vs. rainy days.

🕒 Peak Usage Hours → Heatmap analyzing the busiest times for rentals.

🏙️ City-Wise Comparison → Map visualization of bike usage across Latvia, highlighting Riga.

📅 Weekend vs. Weekday Usage → Pie chart showing the percentage of rentals occurring on weekends.

📈 Monthly Trends → Column chart tracking rental fluctuations over different seasons.

📌 DAX Measures Used

Total Bike Rentals → SUM(BikeData[count])

Average Rentals Per Day → AVERAGEX(VALUES(BikeData[time]), SUM(BikeData[count]))

Peak Hour Usage → MAXX(VALUES(BikeData[time]), SUM(BikeData[count]))

Weather Impact on Rentals → Difference in rentals between rainy and clear days.

Weekend Rental Percentage → % of bike rentals that occur on weekends vs. weekdays.

Bike Usage by City → SUM(BikeData[count]) grouped by City.

📂 Dataset Overview

time → Date & time of rental.

count → Number of bikes rented per recorded time slot.

temp_real_C → Actual temperature in Celsius.

weather → Weather condition during rental time.

is_weekend → Boolean (1 = Weekend, 0 = Weekday).

is_holiday → Boolean indicating if the date is a holiday.

City → City where the bike was rented.

season → Winter, Summer, Spring, or Autumn classification.

🔧 How to Use the Dashboard

Load the dataset into Power BI.

Apply the provided DAX measures for calculated insights.

Customize filters (date range, weather conditions, city selection).

Analyze key insights through interactive visuals.

🚀 Future Enhancements

Integration of real-time bike rental data (if available).

Predictive modeling to forecast future bike rental trends.

User behavior segmentation (tourists vs. locals if applicable).

📌 Tools & Technologies Used

Power BI → Dashboard visualization.

DAX (Data Analysis Expressions) → Custom calculations.

Excel/Python (Pandas) → Data preprocessing and transformation.

📬 Contact & Contribution

Feel free to fork this repository, suggest improvements, or contribute additional features! If you have any questions or suggestions, reach out via   Linkedin : www.linkedin.com/in/oussama--seddik
