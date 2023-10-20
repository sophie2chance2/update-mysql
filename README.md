# Updating MySQL Database

## Overview

This folder contains scripts for updating the MySQL database. Currently, these tables are hosted in GoogleSheets. This script will work to replace those processes with a MySQL database.

## Safety

PLEASE use caution when running these scripts. They are designed to update the database, and if run incorrectly, could cause data loss. Please make sure you have a backup of the database before running these scripts.

Each script should only be run once. Running the script multiple times will cause duplicate entries in the database in many cases.

## Setup

1. Must be connected to the CourseKey VPN
2. Create a .env file in the same directory as the script. See below for details.
3. Install the required packages with `pip install -r requirements.txt`
4. Run only the necessary scripts. See safety section above.

## Running the Script

Each table has its own script. The creation of tables is left in and commented out in case the tables need to be recreated. Each table should have a corresponding action in the script to update the table.

## Environment Variables

**GOOGLE_CRED:** The Google Cloud credentials json. This is used to authenticate with the Google Cloud SQL API. This is required for the script to run.  
**MYDB_PASS:** The password for the MySQL leadershipDashboard user. This is required for the script to run.  
**HUBSPOT_KEY:** The HubSpot API key for pulling all company and deal data. This is required for the script to run.

.env file should look like this:

```
GOOGLE_CRED={json Google Credentials}
MYDB_PASS='password'
HUBSPOT_KEY='key'
```
