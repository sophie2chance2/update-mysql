# Updating MySQL Database

## Environment Variables

GOOGLE_CRED: The path to the Google Cloud credentials file. This is used to authenticate with the Google Cloud SQL API. This is required for the script to run.
MYDB_PASS: The password for the MySQL leadershipDashboard user. This is required for the script to run.
HUBSPOT_KEY: The HubSpot API key for pulling all company and deal data. This is required for the script to run.

## Running the Script

Each table has its own script. The creation of tables is left in and commented out in case the tables need to be recreated. Each table should have a corresponding action in the script to update the table.
