***Project Information*** 

* What is the project name?
  
  Boston City Councilor Ben Weber: Vacant and Elderly Housing in Boston’s District 6

* What is the link to your project’s GitHub repository?

  GitHub `dev` branch: https://github.com/BU-Spark/dd4g-bcc-weber-gentrification/tree/dev

* What is the link to your project’s Google Drive folder? \*\**This should be a Spark\! Owned Google Drive folder \- please contact your PM if you do not have access\*\**

  Google drive folder: https://drive.google.com/drive/folders/10NNv3Zh96TmddmrtEzz00FpnkOMekB4a

* In your own words, what is this project about? What is the goal of this project?

  This project aims to investigate the elderly housing in District 6. It analyzes the current and planned housing with a specific focus on vacancy rates and housing suitable for elderly residents. 
  
* Who is the client for the project?

  The client is City Councilor Benjamin Weber. 
  
* Who are the client contacts for the project?

  jordan.frias@boston.gov and bonnie.delaune@boston.gov.
  
* What class was this project part of?

  Spring 2025 Data Days for Good.

***Dataset Information***

* What data sets did you use in your project? Please provide a link to the data sets, this could be a link to a folder in your GitHub Repo, Spark\! owned Google Drive Folder for this project, or a path on the SCC, etc.

  GitHub `dev` branch: [link](https://github.com/BU-Spark/dd4g-bcc-weber-gentrification/tree/dev/dataset)
  Google drive folder: [link](https://drive.google.com/drive/folders/10NNv3Zh96TmddmrtEzz00FpnkOMekB4a)
  
* Please provide a link to any data dictionaries for the datasets in this project. If one does not exist, please create a data dictionary for the datasets used in this project.

  Property Assessment FY2025: [link](https://data.boston.gov/dataset/property-assessment/resource/6b7e460e-33f6-4e61-80bc-1bef2e73ac54)
  Approved Building Permit: [link](https://data.boston.gov/dataset/approved-building-permits)
  Live Street Address Management (SAM) Addresses: [link](https://data.boston.gov/dataset/live-street-address-management-sam-addresses/resource/6d6cfc99-6f26-4974-bbb3-17b5dbad49a9)
  City Council District Shape File: [link](https://data.boston.gov/dataset/city-council-districts-2023-2032)
  Residential List: [link](https://docs.google.com/spreadsheets/d/1dB7RO-scCLbRU-5hZqq2nnrZX06iW974/edit?rtpof=true&sd=true)
  Housing List: [link](https://drive.google.com/file/d/10QWfF1z6iJMB4kXjMyPUooQjnYVyBq18/view)

  The following datasets do not provide a data dictionary. We will describe them by providing a dictionary on relevant columns used as a part of the analysis.

  **Live Street Address Management (SAM) Addresses**
  | Column Name | Data Type | Description |
  |---|---|---|
  | `FULL_ADDRESS` | String | The complete address, including street number, street name, and unit number. |
  | `FULL_STREET_NAME` | String | The full name of the street, including any prefixes or suffixes. |
  | `STREET_BODY` | String | The main portion of the street name, excluding prefixes or suffixes. |
  | `POINT_X` | Float | The X coordinate (longitude) of the address location in the spatial reference system. |
  | `POINT_Y` | Float | The Y coordinate (latitude) of the address location in the spatial reference system. |

   **Residential List**
  | Column Name | Data Type | Description |
  |---|---|---|
  | `LAST_NAME` | String | Last name of the individual. |
  | `FIRST_NAME` | String | First name of the individual. |
  | `MI` | String | Middle initial of the individual, if available. |
  | `TITLE` | String | Title (e.g., Mr., Mrs., Dr.), if applicable. |
  | `DOB` | Date | Date of birth (MM/DD/YYYY format). |
  | `OCCUPATION` | String | Listed occupation of the individual. |
  | `FULL_ADDRESS` | String | The complete residence address, including house number, street name, and unit number. |
  | `STREET_NUMBER` | String | House number of the residence address. |
  | `STREET_SUFFIX` | String | Street suffix (e.g., Ave, St, Blvd), if applicable. |
  | `STREET_NAME` | String | Name of the street. |
  | `APT_NUMBER` | String | Apartment or unit number, if applicable. |
  | `CITY` | String | City of the residence address. |
  | `STATE` | String | State abbreviation (e.g., MA for Massachusetts). |
  | `ZIP` | String | ZIP code of the residence address. |
  | `MAIL_ADDRESS` | String | Mailing street address, if different from residence. |
  | `MAIL_APT_NUMBER` | String | Mailing apartment or unit number, if applicable. |
  | `MAIL_CITY` | String | City for the mailing address. |
  | `MAIL_STATE` | String | State for the mailing address. |
  | `MAIL_ZIP` | String | ZIP code for the mailing address. |
  | `PARTY` | String | Political party affiliation. |
  | `VS` | String | Voter status indicator. |
  | `WARD` | Integer | Voting ward in which the individual is registered. |
  | `PRECINCT` | String | Voting precinct number. |
  | `REG_DATE` | Date | Voter registration date. |
  | `RES_ID` | String | Unique residence identifier. |

  **Housing List**
  | Column Name | Data Type | Description |
  |---|---|---|
  | `NAME_OF_DEVELOPMENT` | String | The name of the housing development. |
  | `MASSHOUSING_NUMBER` | String | The MassHousing identification number for the development. |
  | `SITE_ADDRESS` | String | The physical address of the housing development. |
  | `SITE_TELEPHONE` | String | Contact telephone number for the site. |
  | `MANAGEMENT_COMPANY` | String | The company responsible for managing the development. |
  | `MANAGEMENT_TELEPHONE` | String | Contact telephone number for the management company. |
  | `PB_SUBSIDY` | Boolean | Indicates if the development receives project-based subsidy (`☑` for Yes, `☐` for No). |
  | `MH_FINANCED` | Boolean | Indicates if the development is MassHousing financed (`☑` for Yes, `☐` for No). |
  | `FAM` | Integer | The number of family-designated units in the development. |
  | `ELD` | Integer | The number of elderly-designated units in the development. |
  | `BEDROOM_SIZE_0_1` | Integer | The number of units with 0 or 1 bedroom. |
  | `BEDROOM_SIZE_2_3` | Integer | The number of units with 2 or 3 bedrooms. |
  | `BEDROOM_SIZE_4+` | Integer | The number of units with 4 or more bedrooms. |
  | `ACCESS_UNITS` | Integer | The number of accessible units in the development. |
      
* What keywords or tags would you attach to the data set? 

  Elderly resident, Boston housing, housing availability, housing options

*The following questions pertain to the datasets you used in your project.*   
*Motivation* 

* For what purpose was the dataset created? Was there a specific task in mind? Was there a specific gap that needed to be filled? Please provide a description.

  All datasets are published or shared for transparency in fair assessment of property availability and options. It establishes compliance of housing work and allows elderly individuals to gain a more comprehensive view of available residency based on their needs. 

*Composition*

* What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? Are there multiple types of instances (e.g., movies, users, and ratings; people and interactions between them; nodes and edges)? What is the format of the instances (e.g., image data, text data, tabular data, audio data, video data, time series, graph data, geospatial data, multimodal (please specify), etc.)? Please provide a description.

  Most of our datasets are tabular data or geospatial data, which is divided into two categories:
  
  Housing: Property Assessment,  Approved Building Permit, Residential List, and Housing List, which was transformed from a PDF into Excel then CSV file. 
  Geospatial: Live Street Address Management (SAM) Addresses and City Council District Shape File. 
  
* How many instances are there in total (of each type, if appropriate)?

  We have around hundreds of thousands of instances of tabular data points and geospatial data points.
  
* Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set? If the dataset is a sample, then what is the larger set? Is the sample representative of the larger set? If so, please describe how this representativeness was validated/verified. If it is not representative of the larger set, please describe why not (e.g., to cover a more diverse range of instances, because instances were withheld or unavailable).

  All datasets contain all possible instances known to the distributor.
  
* What data does each instance consist of? “Raw” data (e.g., unprocessed text or images) or features? In either case, please provide a description.

  All datasets are a mixture of raw data. 
  
* Is there any information missing from individual instances? If so, please provide a description, explaining why this information is missing (e.g., because it was unavailable). This does not include intentionally removed information, but might include redacted text.

  The Housing List dataset is limited to the year 2023, meaning that we could not complete analysis on the latest deed-restricted housing for elderly individuals. 
  
* Are there recommended data splits (e.g., training, development/validation, testing)? If so, please provide a description of these splits, explaining the rationale behind them.

  Not applicable to our project as we are only analyzing the data. 
  
* Are there any errors, sources of noise, or redundancies in the dataset? If so, please provide a description.

  Not applicable to our project as the datasets are mainly accurate. The challenge is defining the boundary of District 6 and it was resolved using addresses and SAM IDs. 
  
* Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g., websites, tweets, other datasets)? If it links to or relies on external resources,   
  * Are there guarantees that they will exist, and remain constant, over time;  
  * Are there official archival versions of the complete dataset (i.e., including the external resources as they existed at the time the dataset was created)?  
  * Are there any restrictions (e.g., licenses, fees) associated with any of the external resources that might apply to a dataset consumer? Please provide descriptions of all external resources and any restrictions associated with them, as well as links or other access points as appropriate.

  The datasets are both self-contained and reliant on internal sources. The former should remain constant as a public record, and the latter should remain available by requesting from the client team. 
    
* Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals’ non-public communications)? If so, please provide a description.

  Most data are made public with no license required. Residential List may be confidential as it is shared from the client team. 
  
* Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety? If so, please describe why.

  Not applicable to our datasets as all contents are neutral. 
  
* Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset? If so, please describe how.

  Yes. Some housing datasets contain the resident's name, the property owner, and the addresses where they can be contacted. However, we did not include such information in our analysis. 
  
* Dataset Snapshot, if there are multiple datasets please include multiple tables for each dataset. 


Property Assessment FY2025
| Size of dataset | 80.5MB |
| :---- | :---- |
| Number of instances | 183,445  |
| Number of fields  | 67 |
| Labeled classes | 0 |
| Number of labels  | 0 |

SAM Address Database
| Size of dataset | 114.4MB |
| :---- | :---- |
| Number of instances | 399,842 |
| Number of fields  | 32 |
| Labeled classes | 0 |
| Number of labels  | 0 |

City Council District Shape File
| Size of dataset | 131KB |
| :---- | :---- |
| Number of instances | 9 |
| Number of fields  | 15 |
| Labeled classes | 0 |
| Number of labels  | 0 |

Residential List Data
| Size of dataset | 5.3MB |
| :---- | :---- |
| Number of instances | 51,959 |
| Number of fields  | 24 |
| Labeled classes | 0 |
| Number of labels  | 0 |

Housing List Data
| Size of dataset | 8KB |
| :---- | :---- |
| Number of instances | 22 |
| Number of fields  | 18 |
| Labeled classes | 0 |
| Number of labels  | 0 |
  
*Collection Process*

* What mechanisms or procedures were used to collect the data (e.g., API, artificially generated, crowdsourced \- paid, crowdsourced \- volunteer, scraped or crawled, survey, forms, or polls, taken from other existing datasets, provided by the client, etc)? How were these mechanisms or procedures validated?

  Most datasets are directly sourced and downloaded from Analyze Boston. Residential List is a Google sheet provided to us by the client team. 
  
* If the dataset is a sample from a larger set, what was the sampling strategy (e.g., deterministic, probabilistic with specific sampling probabilities)?

  Not applicable to our project.
  
* Over what timeframe was the data collected? Does this timeframe match the creation timeframe of the data associated with the instances (e.g., recent crawl of old news articles)? If not, please describe the timeframe in which the data associated with the instances was created. 

  The dataset's timeframe varies, but we focused on the most recent dataset, meaning years from 2023 to 2025. 
  
*Preprocessing/cleaning/labeling* 

* Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.

  We renamed or restructured the data columns for some datasets. We also imputed the missing geographical field by joining the address with Boston SAM Addresses to get the coordinates, which is then used to plot against the City Council District shapefile to determine District 6.
  
* Were any transformations applied to the data (e.g., cleaning mismatched values, cleaning missing values, converting data types, data aggregation, dimensionality reduction, joining input sources, redaction or anonymization, etc.)? If so, please provide a description.

 We converted data types, especially those that derive from loading CSV data. For instance, zip codes are often loaded as a numeric value, which we convert to strings and retain the 0 in the front. All steps are included in notebooks. 
  
* Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? If so, please provide a link or other access point to the “raw” data, this could be a link to a folder in your GitHub Repo, Spark\! owned Google Drive Folder for this project, or a path on the SCC, etc.

 Yes. The raw data can be found in the project description under `Data Sets + Data Dictionary` section, or in the Google drive folder: [link](https://drive.google.com/drive/folders/1g9X-ejbomg7jXDzrUzcb6xHyTybwhV0N) with the naming convention of `*-raw-data`. 
  
* Is the code that was used to preprocess/clean the data available? If so, please provide a link to it (e.g., EDA notebook/EDA script in the GitHub repository).

  Yes. The EDA notebooks can be found in GitHub `dev` branch under the `notebook` folder: [link](https://github.com/BU-Spark/dd4g-bcc-weber-gentrification/tree/dev/notebook)

*Uses* 

* What tasks has the dataset been used for so far? Please provide a description.

  The datasets have been used to provide insights into housing options, availability, and construction in District 6. The cleaned datasets are also used to visualize the analysis.
  
* What (other) tasks could the dataset be used for?

  The datasets can be used for exploring vacancy rate, availability, income level, and more demographic factors. 
  
* Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?

  Some properties are merged unsuccessfully from the table if coordinates cannot be found from Boston SAM Addresses, as we cannot know for sure if they are in District 6.
  
* Are there tasks for which the dataset should not be used? If so, please provide a description.

  The dataset should not be used for tasks that could breach privacy, perpetuate biases, or lead to unethical outcomes. 

*Distribution*

* Based on discussions with the client, what access type should this dataset be given (eg., Internal (Restricted), External Open Access, Other)?

  Most datasets used are public, besides the Residential List data provided by the client team. All datasets could be public if the residents' identities are protected properly. 

*Maintenance* 

* If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so? If so, please provide a description.
  All datasets are uploaded to GitHub in the `dataset` folder and the Google Cloud Folder owned by Spark!.

  The datasets are available in the `dataset` folder under the `dev` branch.

*Other*

* Is there any other additional information that you would like to provide that has not already been covered in other sections?

  No. 
