---
title: GBFS
category: Bike and System Availability
order: 1
---

## Scope

The City of Chicago requires that companies publish information about their system and bike availability using the [General Bikeshare Feed Specification (GBFS) v1.1 (draft spec)](https://github.com/dsgermain/gbfs/tree/f76251ad4c754b62defc42562887724f287b73ea). This data will be used by the city to ensure equity of bike availability and can be used by the transit community to integrate dockless bikeshare data into mobile applications that are used by Chicagoans.

## File Format

GBFS is a flexible format that consists of required and optional files. Below outlines the minimum requirements for operation within the City of Chicago.

Companies may also publish the optional files listed below. Likewise, companies may make additions to the GBFS format as long as it does not conflict with the minimum requirements.

#### Required Files

City of Chicago requires that companies publish six of the GBFS v1.1-draft files. Below are the required files that must be published:

File Name                           | Defines
------------------------------------| ----------
gbfs.json                           | Auto-discovery file that links to all of the other files published by the system. *This file is optional in the GBFS, but required by the City of Chicago*.
system_information.json             | Describes the system including System operator, System location, year implemented, URLs, contact info, time zone.
station_information.json            | Mostly static list of all stations, their capacities and locations. *(Note: This file may contain no information in a dockless system but is required by the City of Chicago in order to maintain compliance with the GBFS standard.)*
free_bike_status.json               | Describes bikes that are available in non station-based systems. *This file is optional in the GBFS, but required by the City of Chicago*.
geofencing_zone_information.json    | Mostly static list of all geofencing zones, their capacities, locations and areas. *This file is optional in the GBFS, but required by the City of Chicago*.
geofencing_zone_status.json         | Defines geofencing zones available in the system and their link to physical stations if any. *This file is optional in the GBFS, but required by the City of Chicago*. Elements within the `num_bikes_available_types` array are required by the City of Chicago and should be set to 0 if not applicable.
system_regions.json                 | Describes the regions the system is broken up into. *This file is optional in the GBFS, but required by the City of Chicago*.



#### Optional Files

These files are supported by GBFS, but are not mandatory:

File Name                           | Defines
------------------------------------|-----------
station_status.json                 | Number of available bikes and docks at each station and station availability. Optional as system can be free floating.
system_hours.json                   | Describes the hours of operation for the system.
system_calendar.json                | Describes the days of operation for the system.
system_pricing_plans.json           | Describes the system pricing.
system_alerts.json                  | Describes current system alerts.


## Reporting to Chicago

Companies will need to inform the City of Chicago of the location of the `gbfs.json` file on the internet. The `gbfs.json` file contains the necessary information to find other files related to the GBFS data.

If a token or authentication is required to view that file, the location to apply for the token must also be submitted to the City.
