# Multi-Source Log Analysis Using Splunk

## Project Overview

This project demonstrates the ingestion, analysis, and investigation of multiple log sources using Splunk. The objective was to analyze authentication events, database activity, and web server access logs to identify patterns, monitor activity, and investigate potentially suspicious behavior.

The following log sources were analyzed:

* linux_secure
* database
* access_combined_wcookie

All log sources were indexed into Splunk under the `test` index and investigated using SPL (Search Processing Language) queries, statistical analysis, and dashboards.

---

## Objectives

* Ingest multiple log sources into Splunk
* Analyze Linux authentication logs
* Investigate web server access activity
* Monitor database events
* Develop SPL queries for log investigation
* Create dashboards for monitoring and visualization
* Identify authentication failures and suspicious activity

---

## Log Sources

### linux_secure

Linux authentication and security logs containing login attempts, authentication failures, and system security events.

### database

Database activity logs used to monitor database operations and event activity.

### access_combined_wcookie

Web server access logs containing client requests, HTTP status codes, and web traffic information.

---

## Analysis Performed

### Authentication Analysis

* Investigated failed password attempts
* Identified source IP addresses responsible for authentication failures
* Analyzed targeted user accounts
* Reviewed authentication event patterns

### Web Traffic Analysis

* Analyzed top client IP addresses
* Reviewed HTTP status code distribution
* Investigated web access activity
* Monitored request patterns

### Database Activity Analysis

* Reviewed database event activity
* Analyzed event distribution
* Compared activity across multiple log sources

---

## Dashboard Components

The Splunk dashboard includes:

* Total Event Count
* Events by Source
* Event Timeline
* Failed Authentication Attempts
* Top Client IP Addresses
* HTTP Status Code Analysis

---

## Key Findings

* Successfully ingested and analyzed three different log sources.
* Identified repeated failed authentication attempts from a small number of source IP addresses.
* One source IP generated significantly more failed password attempts than other observed IP addresses.
* Analyzed web traffic patterns through access log investigation.
* Compared event activity across Linux, database, and web application logs.

---

## Skills Demonstrated

* Splunk Administration
* Log Analysis
* Security Monitoring
* SPL Query Development
* Dashboard Creation
* Event Investigation
* Data Visualization
* Security Analytics

---

## Tools Used

* Splunk Enterprise
* SPL (Search Processing Language)

---

## Conclusion

This project demonstrates the use of Splunk for multi-source log analysis, event investigation, and dashboard development. By analyzing Linux security logs, database activity logs, and web server access logs, valuable insights were obtained regarding authentication activity, web traffic behavior, and overall event distribution across multiple systems.
