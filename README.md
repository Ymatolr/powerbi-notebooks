# Power BI Artifacts Extractor

This notebook uses Microsoft Power BI and Fabric APIs to fetch all artifacts (datasets, reports, dashboards, dataflows, notebooks, and pipelines) from a specified workspace.  
The data is written to a Spark DataFrame and saved as a Delta table.

## How to Use

1. Fill in your `client_id`, `client_secret`, `tenant_id`, and `workspace_id`.
2. Run the notebook in an environment with Spark and `msal`, `requests`, `pandas` installed.
3. Outputs will be printed and stored in a Delta table named `power_bi_artifacts`.
