## Building-an-Azure-Data-Warehouse-for-Bike-Share-Data-Analytics

## Project Overview

Divvy is a bikesharing program in Chicago, Illinois USA that allows riders to purchase a pass at a kiosk or use a mobile application to unlock a bike at stations around the city and use the bike for a specified amount of time. The bikes can be returned to the same station or another station. The City of Chicago makes the anonymized bike trip data publicly available for projects like this where we can analyze the data. Since the data from Divvy are anonymous, we have created fake rider and account profiles along with fake payment data to go along with the data from Divvy.

### The goal of this project is to develop a data warehouse solution using Azure Synapse Analytics and more specifically to:

- Design a star schema based on the business outcomes listed below;
- Import the data into Synapse;
- Transform the data into the star schema;
- View the reports from Analytics.

### The business outcomes we are designing for are as follows:

1. Analyze how much time is spent per ride
- Based on date and time factors such as day of week and time of day
- Based on which station is the starting and/or ending station
- Based on the age of the rider at the time of the ride
- Based on whether the rider is a member or a casual rider
2. Analyze how much money is spent
- Per month, quarter, year
- Per member, based on the age of the rider at the account start
3. Analyze how much money is spent per member
- Based on how many rides the rider averages per month
- Based on how many minutes the rider spends on a bike per month


##### Dataset

The dataset looks like this:
![divvy-erd](https://video.udacity-data.com/topher/2022/February/6205b1d2_divvy-erd/divvy-erd.png)

The Star schema looks like:
![star_schema](./star_schema.jpeg)

The extract step looks like:
![star_schema](./extract_img.jpeg)

The Delta transform step looks like:
![star_schema](./delta_transform.png)
