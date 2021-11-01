---
date: "22/10/2021"
output:
  pdf_document: default
  html_document: default
---

# **GEOG 712: Data in Brief**
##### Daniel Van Veghel -- October 25, 2021
***
  
### **In this Data in Brief (DiB):**
- Data Title
- Authors
- Keywords
- Data Specification Table
  1. Subject Area
  2. Specific Subject Area
  3. Type of Data
  4. Data Acquisition
  5. Data Formats
  6. Data Collection
  7. Data Storage
  8. Data Source Location
  9. Data Accessibility
- Data Importance
- Figures

### **Data Title:**
"Route Patterns and Characteristics of Bike Share Trips"
  
### **Author:**
Daniel Van Veghel, _M.Sc. Candidate in the School of Earth, Environment and Society -- McMaster University_
_1280 Main St. W., Hamilton, ON, L8S 4V8_
_Email: vanveghd@mcmaster.ca_
  
### **Keywords:**
_BikeShare, Route Choice, Cycling, Route Characteristics_

### **Data Specification**
  
**Subject Area**: Geography; Social Sciences

**Specific Subject Area**: Transportation Geography; Geographic Information Science; Active Transportation; Cycling

**Type of Data**:
- Tables (.csv format)
- Shapefiles (.shp format)
- Graphs, Histograms other data visualizations (Derivatives of the .csv files)
- Text files (.docx or .txt format)

**Data Acquisition**:
Raw data was acquired via Hamilton BikeShare cycle unit GPS units, which log location points of the BikeShare units during trips between Origin and Destination Hubs, and submit them to _TransLAB_ as _.gpx_ files. However, due to confidentiality agreements with Hamilton BikeShare (which allows only aggregated, anonymized route data to be shared), the data presented is for one selected Hub Pair (origin and destination). This data was acquired via _TransLAB_'s aggregation process -- converting raw GPX files into Line Shapefiles for analysis. An example route shapefile image can be seen as Figure 1 in the _Figures_ section of this DiB.  The aggregation process is done via `Python,` and `R`.

**Data Formats**:
- **Raw Data**: GPX Point Files (.gpx format); Trip Logs (.csv format)
- **Processed Data**: ESRI Shapefiles (.shp format); Detailed Trip Log Data (CSV files)
- R Codes used to present histograms or maps to be publicly available via _Github_
  
**Data Collection**: Data collection occurs constantly via Hamilton BikeShare GPS, for every trip a BikeShare user takes in the city of Hamilton. Hamilton Bikeshare records every single trip taken; however, the dataset is limited in geographic location to only the City of Hamilton (including BikeShare Hubs in Ancaster, Dundas, and Stoney Creek). The information provided by dataset
  
While the exact data variables are still yet to be determined _(and this information will be updated when more is known)_, for the purpose of this particular project, the main factors will be route lengths, characteristics (i.e. number of arterial roads along route, number of minor roads, etc.), and choice frequencies of users (for example, is the distribution of routes skewed away from the shortest route?).  The Hub pair is to be chosen if it has a sufficient sample size of routes for a particular month, as well as a significant variety of potential route choices (that is, there are many links in the cycling network between Hub A and Hub B).

**Definition of Variables**: While exact variables in CSV or Shapefiles used (that meet Ethics' clearance) are still being finalized, variables will reflect saftey of routes -- such as number of arterial roads along route, number of minor roads, etc. -- and route distributions -- route lengths (km), number of turns/intersections, etc.

**Data Storage**: Stored on cloud drives in _TransLAB_, the data generally ranges from hundreds of MB to GB of storage space required -- per month. The data for this project in particular will only be routes between one hub pair for one month, and as such -- while still stored securely on the lab's storage drives -- the storage requirements for the project's data will be in megabytes (MB), or non more than one or two gigabytes (GB). It will exist locally on a lab computer in an appropriately named folder as a backup for added security. 
  
**Data Source Location**: _McMaster University, Hamilton, Ontario, Canada_. Samples were collected across cycling network of the city of Hamilton, Ontario. 
  
**Data Accessibility**: The raw Hamilton BikeShare data is stored in cloud drives housed at McMaster University's _TransLAB_. These drives act as the primary data repository for all Hamilton BikeShare data. They are named and labeled by their dates of acquisition, and whether they are records or the trips or the GPS points themselves.  Due to the location and therefore personal route information in the raw data, it is confidential and not publicly available. 
  
Requests for access to some or any of the Data are to be made to the both the Lab and to Hamilton BikeShare.
**Hamilton BikeShare Contact Info**: [Website](https://hamilton.socialbicycles.com); **Phone**: (289)-768-2453
**TransLAB Contact Info**: _To be provided at a later date_
  
The code used to create descriptive statistics of the Hub-pair routes and then display maps or charts/histograms will be made publicly available -- as will all figures themselves -- using GitHub as a repository. [Click to access the link to the Github Repository](https://github.com/vanveghd/My-First-Repository)

**Collaboration**: Drafts and subsequent steps of the project will be made available to my supervisor via email. Additionally, each subsequent step in the project will be published on the publicly-available repository on Github -- this link will also be shared with my supervisor and can be checked at any time. Finally, data and the scripts used to present the data will be saved on the lab's cloud drive and can be accessed by other members of the lab at any time. 

### Data Importance: 
- Data is useful for determining cyclist route choices, route characteristics, route length distributions, 
- Can directly benefit urban planners, and policy-makers. With route data on cyclists being extremely difficult to retrieve (often involving qualitative travel surveys rather than precise spatial locations), the ability to analyze Bike Share users' precise routes is a crucial aspect to understanding the travel behaviour of cyclists.  
- Even the examination of the route characteristics between two hub pairs gives important insight to what affects Bike Share users' route choice -- do they avoid major roads? Are they more inclined to take more scenic trips? Do they avoid certain areas or landuses? 
- Can indirectly benefit community members and BikeShare users. Promoting, and providing insight into Active Transportation and BikeShare users' travel behaviour can help shape future research, investment and policy changes regarding these transportation modes: potentially improving health, wellbeing and the environment of urban regions.
An analysis of this route data, leveraging detailed route observations (with many route characteristic variables), and the multitude of statistical analysis packages/functions available in the `R` platform means visualizing and exploring the data is readily possible. 

### Ethics:
Datasets themselves are confidential as per agreements with Hamilton BikeShare and Ethics Agreements with the McMaster Research Ethics Board (MREB). Only aggregated data or visual data presentations (maps, charts and graphs) can be presented on the project's publicly-available [Github Repository Page](https://github.com/vanveghd/My-First-Repository).

### Competing Interests:
None. 


