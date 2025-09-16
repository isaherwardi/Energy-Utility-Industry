# Energy Industry Overview

## Smart Grid

## Smart Home

## An architectural blue-print in the context of a utility company

A conceptual model of an example architecture is shown in Figure 1. When this model is applied in the context of a utility company, the most important elements can be explained and illustrated:

- Data sources

In recent years, the available dataset of utility companies has increased substantially. In the past, this was limited to mainly consumption data from meter readings and later through meter transmissions, non-exclusively today extended with:

- Smart meter data and sensor data from the grid
- Supervisory Control and Data Acquisition (SCADA systems)
- Social media and web statistics of (potential) customers
- Grid and asset outage management
- Wholesale and financial market data
- Asset tracking for consumers, power generation and electric grids (incl. GIS data)
- Weather data

 

- Data management

Data management as part of the existing operating model of the firm consists of three main components. Relational database management systems (RDBMS) and data warehouses are already known for years. However, to cope with the increased diversity of the data flows, these data warehouses need to be supplemented with data reservoirs and data factories. Data reservoirs contain data that do not have a stringent requirement regarding data formalization or modelling and allow for parallel processing. Typically non-structured data such as social media data, click data, photos, files, etc. can be gathered in data reservoirs. A well-known technology for capturing and processing of these types of data is the Hadoop Distributed File System (HDFS) but also other technologies such as Not Only SQL (NoSQL) data bases are gaining market share. The data factory represents the management and orchestration of the data into and between the Data Discovery and Development lab, as well as the provision of data to other systems for operational use.

 

- Fast data streams

Fast data contains data flows that require ‘in-flight’ processing and pre-determined analytics to identify any actionable events and next-best-actions to support fast decision making. For example grid-components’ sensor data that flag any unusual behavior, as an indicator for grid failure. When such an event is identified, automatically a chain of actions can be initiated to correct the issue at the maintenance department.  

 

- Data discovery and development lab

Besides using the data sources for operational purposes, a company with a focus on innovation should include a ‘playground’ for new (data driven) initiatives and experimentation in its enterprise architecture. Here defined as a data discovery and development lab, should offer the opportunity for data scientists and developers to work on new POCs. These new insights, products and services that can later be embedded into the operational model of the organization. For example, a utility company can create a POC for a new trading platform for peer-to-peer energy exchange and settlement or develop a new algorithm for electricity consumption forecasting.

 

- Analytics

The data processed through the operational chain of events can be used for business analytics. Business analytics mainly uses tools for standard BI activities, such as reporting, creating visuals and dashboards. The data sourced for these activities is therefore offered in a more structured format in contrast to the initial raw data where it originates from. For example, the imbalance position on the intra-day market of a utility company can be monitored via a dashboard at the dispatch department.

 

Due to the size and multidimensionality of the data available in the company, the ability to quickly interact with this data through visual drill-down capabilities and dashboards has become increasingly important to add value to the available data. Over the past years, the technology to quickly visualize data and create business reports and dashboards has rapidly improved, and new players (e.g. Qlikview, Tableau) have gained market share over the more traditional BI software suppliers. They stand out in terms of performance due to in-memory processing and reduce the dependency on the IT department for creating insightful reports and dashboards.

 

- Results and discovery output

A feedback loop that re-feeds the data sources from the results from the analytics and data discovery lab allows for evaluation and continuous improvement of the initiatives and operation.

 

![img](/images/Enterprise_Arch_Utilities.png)


Figure 1. Conceptual model of an example of next generation Enterprise Architecture as an enabler for digital transformation

