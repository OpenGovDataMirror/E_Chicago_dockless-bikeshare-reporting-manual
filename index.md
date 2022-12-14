---
title: Overview
---

As part of its licensing process for Dockless Bikeshare companies, Chicago requires the companies to report on their activities each month and to provide publicly accessible information on bike and system availability.

## Monthly Data Submissions

Companies are required to submit details on trip, maintenance, and customer reported issues on a monthly basis. Companies must follow the specified schemas when reporting the data and pass validation checks before it is accepted by the City of Chicago.

### Submission Deadlines

Data meeting the requirements of this manual must be submitted on or before these dates through the duration of the pilot:

|      Due Date       |   Beginning Date   |      End Date      |
|---------------------|--------------------|--------------------|
| June 11, 2018       | May 1, 2018        | May 31, 2018       |
| July 10, 2018       | June 1, 2018       | June 30, 2018      |
| August 10, 2018     | July 1, 2018       | July 31, 2018      |
| September 10, 2018  | August 1, 2018     | August 31, 2018    |
| October 10, 2018    | September 1, 2018  | September 30, 2018 |
| November 12, 2018   | October 1, 2018    | November 1, 2018   |


### Submission Format

Submit three separate CSV files with the following naming convention, where [company] denotes the submitting company; [topic] represents one of the three areas being requested: trips, reports, and maintenance; and date corresponds to the period covered by the file (not the period when the file is submitted). For instance, ACME service submitting the trips file for data pertaining to May 2018 would submit "acme-trips-201805.csv".

```
[company]-[topic]-[date].csv
```

Three files should be submitted for [trips](trips), [reports](reports), and [maintenance](maintenance).

## Bike and System Availability

Companies must make data on bicycle and system availability to the public using the General Bikeshare Feed Specification (GBFS). The current requirement is to post feeds that comply with the draft specification of [GBFS v1.1](https://github.com/dsgermain/gbfs/blob/f76251ad4c754b62defc42562887724f287b73ea/gbfs.md). 

Companies must publish the GBFS feed where it can be accessed without a username or password. Companies may request a token or authentication be used to access the GBFS feed; however, the process to receive a token needs to be available to the public.

See the [bike and system availability](gbfs) section for specific details.
