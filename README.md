# ESRI-GPSA-S3-Cattle-Grazing-Allotments
This exercise demonstrates using ArcGIS Online for water quality monitoring, identifying hydrologic basins and impacted streams within grazing allotments. It illustrates overlay analysis within spatial analysis for addressing such issues. The data is real, but the scenario, analysis, and decisions are hypothetical.

Using overlay analysis, I was able to identify the allotments located inside of the Oregon basins that were mostly within the central/western part of the state. If field tests find a water quality issue with a particular stream or hydrologic basin, the biologists can filter the results layer to find out which allotments are within a particular basin or which allotment the stream passes through.

## Section 3 ##
**Exercise 1: Determining How Places are Related: Cattle Grazing Allotments**
1. Scenario: The Department of Environmental Quality in Oregon aims to monitor livestock grazing's impact on water quality, noting previous studies confirming sediment and waste pollution in grazing areas' streams.
2. Grazing Allotments: Federal agencies manage grazing lands via allotments, issuing permits or leases to ranchers for each allotment.
3. Monitoring Approach: State biologists monitor water quality by hydrologic basins, intending to identify all grazing allotments within basins with water quality issues for intervention.
4. GIS Use: Utilizing GIS, state biologists aim to determine which hydrologic basins and streams require monitoring based on livestock grazing's impact on water quality.
5. Questions to Address:
  - Identification of grazing allotments within hydrologic basins.
  - Determination of streams or basins necessitating monitoring or testing.

6. Exercise Steps
   
   **Data Exploration and Preparation:**
   - Examined layer information (Grazing Allotment, Hydrologic Unit and Streams)
   <img width="1242" alt="Screenshot 2024-02-08 111708" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/106b93bb-46d2-4e79-a4a4-5e3a96797020">
   
  **Data Analysis and Modeling:**
  - Combine information from three different layers through overlay analysis.
  - Utilize the Overlay Layers analysis tool to overlay the Grazing Allotment and Hydrologic Unit layers.
    <img width="1249" alt="Screenshot 2024-02-08 112109" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/645be80d-2f4c-44ec-904a-980e900f3617">

  - Generate a new layer indicating overlaps between input features (allotments and basins).
    <img width="1244" alt="Screenshot 2024-02-08 112444" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/af34ff20-c764-4417-b31c-e7ec32a47c1f">

  - Conduct a second overlay analysis, combining the output of the first overlay with the Streams layer for further insight.
    <img width="1244" alt="Screenshot 2024-02-08 113154" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/e371ced5-c961-4ef5-890b-880445e850d5">

  **Interpretation of Results:**
  - Requested Information: Biologists request data on the Middle Fork John Day basin area after initial overlay analysis.
    <img width="1247" alt="Screenshot 2024-02-08 115050" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/f78f21ad-8de4-4487-a6f2-05f9f98ea4dc">

  - Filtering Process: Filter layer features to identify allotments within the Middle Fork John Day basin.
    <img width="1244" alt="Screenshot 2024-02-08 115613" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/10856e02-fafb-4960-ba2f-a0ea0c310b71">

  - Visualization: Visualize streams flowing through identified allotments for further analysis.
    <img width="1246" alt="Screenshot 2024-02-08 121535" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/fa801410-b021-4a9f-a2b0-b270512f52ad">

  **Prioritization Mapping**
  - Task Assignment: Create a prioritization map of grazing allotments within hydrologic basins based on stream length relative to allotment size.
  - Analysis Tool: Utilize the Summarize Within tool to summarize the total stream length within each allotment.
    <img width="1245" alt="Screenshot 2024-02-08 162135" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/96a44a00-49c6-478b-af24-ed12b22a0c87">
    <img width="281" alt="Screenshot 2024-02-08 162212" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/a53c2155-0385-4db9-ad4c-3d7b550b8407">
    <img width="1245" alt="Screenshot 2024-02-08 162447" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/46e06fba-82cb-4988-abf5-b00e5f69cfb7">

  - Considerations: Prioritize allotments based on the sum of stream lengths (more than five miles of streams), not the number of streams within each allotment.
    <img width="1246" alt="Screenshot 2024-02-08 162712" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/271babf2-d3ba-457e-b249-b1a7b62946be">

  **Choropleth Mapping for Priority Assessment**
  - Priority Determination: Identify allotments prioritized for consistent water sampling based on the longest total stream length relative to allotment size.
  - Resource Optimization: Biologists seek to optimize stream monitoring efforts with limited resources by assessing stream length relative to allotment size.
  - Style Adjustment: Change the style of Summarize Within results to create a choropleth map.
    <img width="1243" alt="Screenshot 2024-02-08 163242" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/be3acabb-7b5a-4896-9ab3-018548b60994">
    <img width="1249" alt="Screenshot 2024-02-08 163551" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/16d0402a-4d50-4458-afca-d2f7045f0943">
    <img width="1244" alt="Screenshot 2024-02-08 163844" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/02a49aea-01e3-4b10-91c3-1eecce31ea60">

  - Map Purpose: Assist biologists in determining the priority of grazing allotments within hydrologic basins for effective water sampling efforts.

  **Downstream Impact Assessment**
  - Area of Interest: Biologists focus on identifying downstream impacts of streams flowing through high-priority allotments.
    ![image](https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/7fcc8ad5-88fb-4ca7-bee9-b12bb9762f30)

  - Objective: Determine downstream flow paths to assess potential pollution impacts from runoff.
  - Methodology: Identify and analyze downstream flow paths to understand potential environmental consequences.
    <img width="1246" alt="Screenshot 2024-02-08 164623" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/8f60f90e-c27f-4087-9497-4c9712c188bf">
    <img width="1243" alt="Screenshot 2024-02-08 164844" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/54f27158-f3da-4285-9ed9-7a61ec60cf4e">

  **Stream Allocation Mapping**
  - Stakeholder Visualization: Fulfill biologists' request for a map displaying intersecting stream names within the specific basin for stakeholders (HUC 17120003).
    - Intersect Of Streams And Allotments layer
    - From the Settings pane, click Styles button.
    - Because you only want to apply unique symbol symbology to the streams in HUC 17120003, you will create an expression using Arcade.
    - Under Choose Attributes, click + Expression. 
    <img width="1051" alt="Screenshot 2024-02-08 165310" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/6113a58b-08d8-4c88-b2f8-404229a86c12">
    <img width="1246" alt="Screenshot 2024-02-08 165752" src="https://github.com/marianahiroki/ESRI-GPSA-S3-Cattle-Grazing-Allotments/assets/110165879/04e47bab-e77f-4c4c-8589-b760c16d25fb">

    - The map and legend display the names of the streams that pass through the allotments in HUC 17120003 and the downstream flow of the streams. The team of biologists can use this map to identify the name of the stream that intersects allotments that could potentially carry harmful runoff downstream. 
