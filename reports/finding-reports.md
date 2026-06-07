# Findings Report

## Project Overview

The purpose of this project was to analyze multiple log sources using Splunk and gain hands-on experience with log investigation, SPL queries, and dashboard creation.

The following log sources were analyzed:

* linux_secure
* database
* access_combined_wcookie

All data was indexed under the `test` index.

---

## Authentication Analysis

Linux security logs were reviewed to investigate authentication-related events.

During the analysis, failed password attempts were identified and grouped by source IP address. Three source IP addresses were observed generating failed authentication events.

One IP address was responsible for 99 failed password attempts, while the remaining IP addresses generated significantly fewer events. This activity indicates a concentrated pattern of failed authentication attempts and was selected for further investigation.

User-based analysis was also performed to determine which accounts were targeted during the failed login attempts.

---

## Web Traffic Analysis

Web application access logs were analyzed to understand client activity and request behavior.

The investigation included:

* Identifying the most active client IP addresses
* Reviewing HTTP status code distribution
* Examining request activity patterns
* Comparing web traffic volume over time

The analysis provided visibility into how users interacted with the web application and highlighted common request patterns.

---

## Database Log Analysis

Database logs were reviewed to understand event activity within the environment.

The analysis focused on:

* Event volume
* Host activity
* Log distribution

Database events were successfully ingested and correlated with other log sources to provide a broader view of system activity.

---

## Dashboard Development

A Splunk dashboard was created to visualize key metrics from all three log sources.

Dashboard panels included:

* Total Events
* Events by Source
* Event Timeline
* Failed Authentication Attempts
* Top Client IP Addresses
* HTTP Status Analysis

The dashboard improved visibility into overall log activity and allowed for easier investigation of events.

---

## Skills Demonstrated

Through this project, the following skills were developed and demonstrated:

* Splunk Search Processing Language (SPL)
* Log Analysis
* Security Monitoring
* Dashboard Creation
* Event Investigation
* Data Visualization
* Multi-Source Log Correlation

---

## Conclusion

This project provided hands-on experience working with multiple log sources in Splunk. By analyzing Linux security logs, database logs, and web application access logs, valuable insights were obtained regarding authentication failures, web traffic activity, and overall event distribution.

The project also strengthened practical experience with SPL queries, dashboard creation, and log investigation workflows commonly used in Security Operations Center (SOC) environments.
