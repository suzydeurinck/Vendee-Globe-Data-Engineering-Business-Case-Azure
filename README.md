# Vendee-Globe-Data-Engineering-Business-Case-Azure

## Overview
I present the "Microsoft Azure Certified Data & AI Track Vendée Globe Business Case" repository, which represents a significant project completed during my participation in the Data & AI bootcamp at Techionista Academy. This project was inspired by the Vendée Globe, a challenging solo non-stop round-the-world sailboat race, and involved building a cloud-based Lambda Architecture in Azure to process telemetry data from sailing boats. The Lambda Architecture includes both real-time and batch-processing paths, facilitating the collection and analysis of sailing boat data. The primary objective is to deliver this data to a PowerBI dashboard, offering spectators a captivating view of the race's progress. Despite the absence of actual race data, I employed a Python application to simulate boat telemetry data for a fleet of 10 race participants. This data is sent to Azure's cloud infrastructure, where it is processed and displayed on the PowerBI dashboard.

This repository serves as a demonstration of my technical skills and ability to tackle complex real-world data engineering challenges. It showcases the successful completion of the Microsoft Azure Certified Data & AI Track Vendée Globe Business Case, highlighting the development of a Lambda Architecture, PowerBI dashboard, and integration of a Python race simulation app for data generation.

![Lambda Architecture Azure](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/b34b48804549bad9369d92f5edc31ce1ea3f8b98/LambdaArchitectureAzure.png)

## Objective
Our primary objective was to develop a cloud-based Lambda Architecture on Microsoft Azure, incorporating Stream Analytics Job, Power BI, and Data Lake Gen 2. This architecture enables real-time and batch processing of telemetry data from sailing boats in the Vendée Globe race. The ultimate goal was to create an engaging Power BI dashboard, providing users with real-time race position tracking and rankings, despite the absence of live race data.

## Features
- **Real-Time Telemetry Data:** Our system seamlessly processed real-time telemetry data from sailing boats participating in the Vendée Globe race, providing instant updates on their positions.
- **PowerBI Dashboard:** We've created a dynamic PowerBI dashboard that offers a visual representation of the race. It displays the current locations of racing teams on a world map and in the future will rank them in real-time.
- **Azure-Powered Lambda Architecture:** Leveraging Microsoft Azure services, including Stream Analytics Job, Power BI, and Data Lake Gen 2, we built a robust Lambda Architecture that enables both real-time and batch data processing.
- **Simulated Data Integration:** Despite the absence of live race data, we integrated a Python race simulation application to generate telemetry data, allowing us to demonstrate the functionality of our data processing pipeline.
- **Data Insight:** Our system provides valuable insights into the Vendée Globe race, even with simulated data. It showcases our expertise in data engineering and Azure services, offering a glimpse into the potential of real-world applications.

## Technologies Used
- **Azure Event Hub:** Used as our data ingestion service to collect telemetry data from sailing boats participating in the Vendée Globe race.
- **Azure Stream Analytics Job:** Employed for real-time data processing and transformation, ensuring that data was available for visualization.
- **Azure Data Lake Gen 2:** Served as our data storage solution, housing data for subsequent analysis.
- **Azure Synapse Analytics:** Utilized for analytics and querying capabilities, particularly with the serverless SQL pool.
- **Power BI:** Employed for dynamic data visualization and interactive dashboard creation, enabling users to monitor the Vendée Globe race in real time.
- **Python:** Leveraged Python to develop a simulation application for generating telemetry data, bridging the gap when live race data was unavailable.
- **GitHub:** Utilized GitHub as a collaborative platform for project management, ensuring seamless teamwork throughout the project.
- **Azure Portal:** Used Azure Portal for configuring and managing Azure resources.

## Methodology

## Report Results

## Contributors
Javeria Umer, Vidisha Gedam, Lavanya Laxmi Uppara, Suzy Deurinck

## Contact
Feel free to reach out to me at suzydeurinck@gmail.com for any inquiries or collaborations.
