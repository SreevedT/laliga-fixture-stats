# laliga-fixture-stats

## Overview
This project comprises 3 pipelines which extract the data of season and fixture of La Liga from football-api, transform the data and load it to the local SQL server database instance.

## Pipeline architecture
1. **pl_season**: Retreives season-level data, transform and store them in a table called season_data. It also extracts list of fixture_ids in the season and store it.
2. **pl_fixture_raw**: Uses the fixture_id list to make API calls for each fixture_id and store the raw data.
3. **pl_fixture**: Transform the raw data of fixtures and store the transformed data in the table fixture_data.

## Technologies Used
1. Azure Data Factory
2. Azure Databricks
3. Azure Blob Storage 
4. SQL Server

## Future Enhancements
 - Consolidate the three pipelines into a single, orchestrated pipeline.
