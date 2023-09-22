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
- **Power BI:** Employed for data visualization and interactive dashboard creation.
- **Python:** Leveraged Python to develop a simulation application for generating telemetry data.
- **GitHub:** Utilized GitHub as a collaborative platform for project management, ensuring seamless teamwork throughout the project.
- **Azure Portal:** Used Azure Portal for configuring and managing Azure resources.

## Methodology
1. **Python Simulator Setup**:
Launched the Python simulator for telemetry data generation using Windows Power Shell and these lines of code:
     py -m pip install azure-eventhub and python .\race_simulator.py
![Python Simulator](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/1015b15241b38b13fe8f8cb1319a7a7a75f459fe/PythonSimulator.png)

2. **Event Hub Configuration**:
Created and configured Event Hub Namespace and added a new Event Hub
Established a Shared Access Policy for data transmission

3. **Stream Analytics Job**:
Set up Stream Analytics Job with an input and two outputs: one for the Data Lake, and one for PowerBI.

4. **Stream Analytics Query**:
Cleaned the garbled data by changing the query into
SELECT
    *
INTO
    [outputdatalake]
FROM
    [inputevent]
WHERE latitude > -10000 AND longitude > -10000 and SELECT *
INTO
    [outputpowerbi]
FROM
    [inputevent]
    WHERE latitude > -10000 AND longitude > -10000

5. **Data Lake Gen2**:
   - Created and named Azure Storage Account for Data Lake Gen2.
   - Utilize the Data Lake in Azure Synapse Analytics to create a serverless SQL pool.
   - Created an external table for ranking boat data, leveraging Data Lake Gen2 as a data source.

6. **Power BI Dashboard**:
   - Created a workspace in Power BI Service.
   - Developed real-time data visualization, including a maps and a live tile.

These steps highlight the key actions undertaken in the Vendée Globe Data Engineering Business Case.

## Report Results

![VendeeGlobeOverview](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/e1f20a30149192c2c4cb581dda29755945703bc4/VendeeGlobeOverview.png)

![VendeeGlobeMap](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/e1f20a30149192c2c4cb581dda29755945703bc4/VendeeGlobeMap.png)

![ExternalTable](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/e1f20a30149192c2c4cb581dda29755945703bc4/ExternalTable.png)

![OverviewProcessMiro](https://github.com/suzydeurinck/Vendee-Globe-Data-Engineering-Business-Case-Azure/blob/e9967f8e5726cea6d55b08d85ddda41e8641cd7c/OverviewProcessMiro.png)

## Contributors
Javeria Umer, Vidisha Gedam, Lavanya Laxmi Uppara, Suzy Deurinck

## Contact
Feel free to reach out to me at suzydeurinck@gmail.com for any inquiries or collaborations.
