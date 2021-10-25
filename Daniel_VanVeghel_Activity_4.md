# **GEOG 712: Data in Brief**
##### Daniel Van Veghel -- October 25, 2021
***
  
### **In this Data in Brief (DiB):**
- Proposed Project Title
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

### **Proposed Project Title:**
"Route Patterns and Characteristics of Bike Share Trips"
  
### **Author:**
Daniel Van Veghel, _M.Sc. Candidate in the School of Earth, Environment and Society -- McMaster University_
  
### **Keywords:**
_BikeShare, Route Choice, Cycling, Route Characteristics_

### **Data Specification**
  
**Specification** | **Information**
--|--
**Subject Area** | Geography; Social Sciences
--|--
**Specific Subject Area** | Transportation Geography; Geographic Information Science; Active Transportation
--|--
**Type of Data** | The project could contain Tables, Graphs (Particularly Line, Bar and Histogram), as well as figures such as anonymized maps -- where exact location is not disclosed. All code used in the data visualization and analysis process will be made available to the public via the project's Github Repository -- to be discussed in a later section of this DiB. The data presented in this project will be the aggregated and analyzed data. Raw data will not be publicly available due to security and confidentiality agreements with Hamilton BikeShare.
--|--
**Data Acquisition** | Raw data was acquired via Hamilton BikeShare cycle unit GPS units, which log location points of the BikeShare units during trips between Origin and Destination Hubs, and submit them to _TransLAB_ as _.gpx_ files. However, due to confidentiality agreements with Hamilton BikeShare (which allows only aggregated, anonymized route data to be shared), the data presented is for one selected Hub Pair (origin and destination). This data was acquired via _TransLAB_'s aggregation process -- converting raw GPX files into Line Shapefiles for analysis. An example route shapefile image can be seen as Figure 1 in the _Figures_ section of this DiB.  The aggregation process is done via `Python,` and `R`.
--|--
**Data Formats** | Raw data is confidential as per agreements with Hamilton BikeShare. Aggregated/filtered data will be formatted as either Shapefiles or aggregated shapefiles into maps generated via `R`, with proper data acknowledgement. All charts, graphs and tables will be derived from these aggregated shapefiles, and created via `R`.  The data will not have explicit locations associated with it; instead it will be presented as all routes between a random BikeShare hub pair.
--|--
**Data Collection** | Data collection occurs constantly via Hamilton BikeShare GPS, for every trip a BikeShare user takes in the city of Hamilton. The aggregation process generally occurs on a monthly basis, converting the trip points to shapefiles, which can allow routes to be analyzed. While the exact data variables are still yet to be determined _(and this information will be updated when more is known)_, for the purpose of this particular project, the main factors will be route lengths, characteristics (i.e. number of arterial roads along route, number of minor roads, etc.), and choice frequencies of users (for example, is the distribution of routes skewed away from the shortest route?).  The Hub pair is to be chosen if it has a sufficient sample size of routes for a particular month, as well as a significant variety of potential route choices (that is, there are many links in the cycling network between Hub A and Hub B).
--|--
**Data Storage** | Stored on cloud drives in _TransLAB_, the data generally ranges from hundreds of MB to GB of storage space required -- per month. The data for this project in particular will only be routes between one hub pair for one month, and as such -- while still stored securely on the lab's storage drives -- the storage requirements for the project's data will be in megabytes (MB), or non more than one or two gigabytes (GB). It will exist locally on a lab computer in an appropriately named folder as a backup for added security. 
--|--
**Data Source Location** | _McMaster University, Hamilton, Ontario, Canada_. Samples were collected across cycling network of the city of Hamilton, Ontario. 
--|--
**Data Accessibility** | The raw Hamilton BikeShare data is stored in cloud drives housed at McMaster University's _TransLAB_. These drives act as the primary data repository for all Hamilton BikeShare data. They are named and labeled by their dates of acquisition, and whether they are records or the trips or the GPS points themselves.  Due to the location and therefore personal route information in the raw data, it is confidential and not publicly available. Requests for access to some or any of the Data are to be made to the both the Lab and to Hamilton BikeShare. This information will be described in detail in the final project, so that all data will receive proper accreditation, confidentiality and proprietary agreements and confidentiality are upheld, and researchers interested in learning more about the data have the ability to contact the organizations with greater knowledge about the data. The code used to create descriptive statistics of the Hub-pair routes and then display maps or charts/histograms will be made publicly available -- as will all figures themselves -- using GitHub as a repository. [Click to access the link to the Github Repository](https://github.com/vanveghd/My-First-Repository)
--|--
**Collaboration** | Drafts and subsequent steps of the project will be made available to my supervisor via email. Additionally, each subsequent step in the project will be published on the publicly-available repository on Github -- this link will also be shared with my supervisor and can be checked at any time. Finally, data and the scripts used to present the data will be saved on the lab's cloud drive and can be accessed by other members of the lab at any time. 

### Data Importance: 

With route data on cyclists being extremely difficult to retrieve (often involving qualitative travel surveys rather than precise spatial locations), the ability to analyze Bike Share users' precise routes is a crucial aspect to understanding the travel behaviour of cyclists. This can help improve cycling infrastructure, direct funding to the most appropriate locations and affect policy-making to enhance cycling investments in the community. 
  Even the examination of the route characteristics between two hub pairs gives important insight to what affects Bike Share users' route choice -- do they avoid major roads? Are they more inclined to take more scenic trips? Do they avoid certain areas or landuses? 
An analysis of this route data, leveraging detailed route observations (with many route characteristic variables), and the multitude of statistical analysis packages/functions available in the `R` platform means visualizing and exploring the data is readily possible. 

### Figures
***
![Example cyclist routes image.](https://github.com/vanveghd/My-First-Repository/blob/main/CycleRoute_Example.PNG)
  _Figure 1: Retrieved from: Lu, Scott & Dalumpines (2018)_
  Available at: [https://doi.org/10.1016/j.jtrangeo.2018.07.012](https://doi.org/10.1016/j.jtrangeo.2018.07.012)

