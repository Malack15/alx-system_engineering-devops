Summary
Date of Incident: June 15, 2024

Duration: 10:00 AM to 12:30 PM GMT

Impact:

75% of users affected
Severe slowdowns and intermittent downtime
Users experienced long load times and frequent timeout errors
Root Cause: Misconfigured database index leading to inefficient query execution and database overload.

Timeline Highlights
10:00 AM GMT: Monitoring alert triggered due to increased response times.
10:05 AM GMT: Engineers began investigation.
10:15 AM GMT: Database performance metrics checked—no immediate issues found.
10:30 AM GMT: Network and server logs reviewed—no network issues.
11:00 AM GMT: Application logs indicated long-running database queries.
11:15 AM GMT: Issue escalated to DBA team.
11:30 AM GMT: DBAs identified misconfigured index related to a new feature.
11:45 AM GMT: Root cause (misconfigured index) identified.
12:00 PM GMT: Database index reconfigured and queries optimized.
12:30 PM GMT: Normal operations restored.
Root Cause and Resolution
Root Cause
A new feature introduced complex queries that lacked appropriate indexing, causing full table scans and heavy database load.

Resolution
The DBA team reconfigured the database index to support the new queries and optimized the queries for better performance.

Corrective and Preventative Measures
Improvements/Fixes
Code Review: Enhance database change review processes.
Automated Testing: Improve testing to simulate high-load scenarios.
Monitoring Enhancements: Increase monitoring capabilities for better database performance insights.
TODO
Patch Database Indexes: Ensure proper indexing for all features.
Add Monitoring Alerts: Set up alerts for long-running queries and high database load.
Optimize Queries: Review and optimize existing queries.
Update Documentation: Document indexing strategy and best practices.
Training: Conduct developer training on efficient database usage and indexing.
