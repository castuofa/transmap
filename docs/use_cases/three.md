# Use Case
## Constructing Event Level Time Series Datasets on Lock Unavailability

### Description

Navigation decision support to the US Army Corps of Engineers (USACE) is provided by the Navigation Civil Works Decision Support Center (NDC). NDC provides information on locks through the Lock Performance Monitoring System (LPMS). Its primary purpose is to act as a planning tool for vessel operators.

The goal and context of this use case is to provide navigation decision support via more detailed descriptions about vessels operating in US waterways, and usage of locks by vessel type.

For example, the Public Lock Usage Report generated by LPMS is a summary of lock usage by vessel type, by year. Because these data are reported on an annual basis it is not possible to do any meaningful analysis of lock usage with respect to seasonality and weather including surface – water data (e.g., streamflow and gage height). The objective of this use case is to show how external variables can help decision support analysts to better understand variation in lock usage given datasets that are high-resolution with respect to both place and time. There is an opportunity to make this kind of analysis possible by systematically collecting data from the Corps Locks website

### Target User(s)

- USACE,
- NDC,
- DOT MARAD,
- research centers and investigators (e.g., MarTREC),
- vessel operators

### Pre-TransMAP Hub Conditions

**Lock Queue Report**

> “The Corps Locks website contains lock and vessel information derived from the United States Army Corps of Engineers Lock Performance Monitoring System (LPMS). The information contained here represents an every 15-minute updated snapshot of Freedom of Information Act (FOIA) data on U.S. flag vessels and foreign vessels operating in U.S. waterways that transited a Corps-owned or operated lock structure.”

Information is organized into nine (9) reports that include a Lock Queue Report with the following Selection Criteria: “Select a river system and a lock, then click the Submit button to view a report of the most recent vessel traffic reported at the lock.”

The report includes

- Avg Processing in Minutes (Past 24 Hours),
- Avg Delay in Minutes (Past 4 Hours),
- Avg Delay in Minutes (Past 24 Hours),
- Last Updated (EST),
- and Most Recent Lockages.

They are described with the following columns:

- Vessel Name,
- Vessel No,
- Direction,
- Number of Barges Proc,
- Sol Date,
- End of Lockage,
- Timezone,
- Delay Minutes,
- Seq No.

> “A flashback query allows you to view data as it existed at a previous point in time. As of [0, 1, 2, …, 99] minutes ago.”

**Public Lock Usage Report**

The currently available, downloadable report has File Name: Lock Usage CY 1993-2019.XLXS

Its first sheet is Table of Contents – Locks by Waterway. The second sheet contains tables for All Waterways, each individual waterway, and every Waterway Lock. **Data are arranged inside of tables such that columns represent calendar years**, and rows represent the following usage variables

- Average Delay
- Average Processing Time
- Barges Empty and Loaded, Commercial Vessels, Flotillas, and Lockages
- Non-Vessel Lockages
- Non-Commercial Vessels, Flotillas, and Lockages
- Percent Vessels Delayed
- Recreational Vessels and Lockages
- Total Vessels and Lockages

### Post-TransMAP Hub Conditions

As exact times of unavailabilities are known, it is now possible to control for things such as weather. It was an achieved objective of this use case to provide lock usage data collected on a better-than-annual basis that can be linked with anything else measured in time. Even without weather data the ability to adjust Lock Performance to continuous rather than annual operation represents a marked change in navigation decision support provided by NDC.

### Advantages & New Capabilities

**Users now have access to integrated, time series datasets relevant to lock unavailability and the reasons for it**. In practice the decision support analyst or user can now generate time series datasets on any lock by entering its identifying information into the program (EROC code, river code, and lock number). Users receive resulting sheets of data for analysis in the following columns: downtime (the response of interest, unavailability), scheduled (binary variable to distinguish between scheduled and unscheduled unavailability), previous uptime (availability), previous downtime, and previous scheduled (to indicate whether the previous downtime was scheduled or unscheduled). There is also a reason code associated with each downtime, and where overlapping downtimes existed in the raw data, those unavailabilities have been collapsed and included all different reason codes in the cell.


### Challenges

TThere remain at least two significant challenges associated with analyzing lock usage data:

1. Lock usage data tend to be incomplete. In other words, analysts have the problem of missing data in the Public Lock Usage Report. This problem has not been made much less severe by systematically collecting data from the Lock Queue Report. However, many locks do have complete data for the years 2000 through 2019.
2. Lock usage data tend to include overlapping unavailabilities that would make the creation of relevant time series datasets impossible. Our code finds and collapses those overlapping unavailabilities.

### Frequency of Use

Since analysts are dealing with event level data that may be changing all the time, analysts will always be tempted to recreate updated post-event datasets before performing new analyses. This potential frequency of use exceeds our expectations about previously being limited to count unavailabilities in set windows of time. That still may be done if it is the analyst’s preference, but the option to operate on a time series of event level data represents an even greater improvement over previous capabilities.

### Contacts

**Justin Chimka**

Associate Professor, Department of Industrial Engineering, University of Arkansas, Fayetteville

**Center for Advanced Spatial Technologies (CAST)**



