# Use Case
## Planning and Monitoring Dredge Maintenance Operations

### Description

Dredge maintenance is an essential operation to ensure navigable waterways. Tasks and planning associated with dredge maintenance is the responsibility of the United States Corps of Engineers (USCAE), who has regularly partnered with academic researchers to improve how dredge decisions are made. A vital component to annual dredge planning is the scheduling of a dredge fleet to job locations throughout the year. These decisions rely on information regarding waterway network connectivity, dredge fleet production rates and capacity, environmental limitations from protected animal species throughout the year, and federal budget limitations. Existing planning tools that assist USACE in these planning efforts rely on regular and reliable access to these data sets. This use case will demonstrate how the TransMAP Hub will be used to support existing dredge planning efforts and expand the capabilities for users to monitor and adjust these plans throughout the year.


### Target User(s)

TransMap Hub hosts USACE databases for environmental restrictions, dredge fleet characteristics and existing dredge operations plans.  

The external TransMap Hub users for this use case are both the USACE leadership and operations teams, as well as industrial and civil engineering researchers from academia.  TransMap will also enable interested industry representatives from the dredge industry to better plan for dredge bids and improve partnerships with the government.  

### Pre-TransMAP Hub Conditions

The information made available through the TransMAP Hub in this use case is currently not available to users in a single platform. The task of dredge planning currently requires the technical capabilities needed to access 3rd party APIs, existing relationships within the USACE to obtain off-line spreadsheets with key data, and a computer system that can interact with the ArcGIS platform. Beyond these access limitations, planners and researchers are also currently hindered by the inability to monitor updates in the information they are using and often are left to determine which data set found in an online repository is accurate.


### Post-TransMAP Hub Conditions

First, waterway network information is maintained through automated resources in TransMAP.  Second, dredge financial data (e.g. bid information, operating costs), existing dredge operation plans (e.g. updated schedules from USACE logistic planners and academic researchers incorporating TransMAP information into their decision-making tools) and environmental requirements (updated irregularly by the Environmental Protection Agency) must be retrieved from the source and uploaded on a regular schedule.  

### Advantages & New Capabilities

#### _Visualization Component_

**Users can view the following maritime network characteristics in the TransMap Hub user interface**

- Historical dredging locations
- Location of locks, dams, and any other critical infrastructure
- Waterway pathways for possible flow of dredeges between potential jobs

**Users can view the following characteristics associated with a current dredge** schedule being executed at the time the user is accessing the TransMap Hub
  
- User can view dredge jobs of interest
- Users can view characteristics of dredge fleet executing the most dredge plan currently in operation

#### _Analysis Component_

In addition to viewing historical dredge information, a researcher can make use of information accessible in TransMAP Hub to make operational decisions.  In the provided Jupyter Notebook environment, this use integrated TransMAP Hub information with open-source optimization tools to assist decision makers in assigning and scheduling dredges to maximize cubic yards dredged over a specified period.  The Dredge Optimization Dashboard allows the research to quickly modify scheduling parameters (e.g. number of jobs, speed of dredge operations).  The optimization implementation implemented in a Jupyter Notebook then solves the associated scheduling problem in less than ten minutes.  Results are viewable directly in the Dredge Optimization Dashboard and specify when a job is completed and which dredge is assigned to each job.

### Challenges

The main challenges for the user to have a successful experience with accessing dredging information from TransMAP Hub is their existing level of dredge knowledge. For example, if a user is not aware of the role of environmental protections on dredge schedules, they may fail to access that information when visualizing or downloading information for their analysis.

The main challenge for TransMAP Hub in this use case will be establishing and maintaining a formal acquisition relationship with key USACE contacts in order to regularly populate TransMAP Hub with the most current operational and planning information.

### Frequency of Use

Planning efforts at USACE typically are done by region and occur at multiple times throughout the year. Therefore, it is anticipated that this use case would be exercised approximately once per month. However, maritime researchers seeking to assist USACE with tools to improve dredge operations planning will likely utilize the resource on a more frequent basis.

### Contacts

**Chase Rainwater**

Associate Professor, Department of Industrial Engineering, University of Arkansas, Fayetteville

**Center for Advanced Spatial Technologies (CAST)**



