# Unauthorized AWS API Calls (AccessDenied)

## Data Ingestion

During ingestion, most events were indexed into the default Splunk index (`main`).
Although a custom index (`cloud_logs`) exists, it contains only a minimal number of events (12),
while the `main` index contains over 2.4 million events.

For this reason, all detections and analysis in this project are based on the `main` index.
