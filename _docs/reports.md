---
title: Customer Reports
category: Monthly Submission
order: 2
---

## Scope

All reports, violations, and complaints submitted to the company. Should include all reports by customers and other members of the public, even if the report cannot be verified or was an invalid complaint.

## File Format

Customer Report data must be reported using the following schema and reported with the following `[company]-reports-[date].csv`.

| Field | Element                  | Data Type           | Required | Description                                                          |
| R1    | Report ID             | String              | Yes      | A unique ID for the report. IDs should be permanently unique, not just unique within the reporting period.                                       |
| R2    | Date and time reported   | ISO 8601 (YYYY-MM-DDTHH:MM:SS+00:00) | Yes      | The date and time of when the report was reported to the company (e.g., 2018-06-30T20:06:06-05:00). |
| R3    | Description              | String              | Yes      | A text description of the alleged violation, complaint, comment, or other report.                                 |
| R4    | Resolution               | String              | Yes      | A text description of the action taken or other resolution by the company. To the extent possible, distinguish between reports determined to be unfounded and reports whose validity could not be determined (e.g., report of inappropriate bicycle return for a bicycle rented again before the company could investigate).                         |
| R5    | Latitude                 | Latitude (WGS84)    | No      | Latitude of the location of the alleged violation or other subject of the report.                           |
| R6    | Longitude                | Longitude (WGS84)   | No      | Longitude of the location of the alleged violation or other subject of the report.                          |
