# laliga-fixture-stats

## Overview
This project comprises of 3 pipelines which extracts the data of season and fixture of laliga from football-api, transforms the data and load them to the local SQL server database instance.

## Pipeline architecture
1. **pl_season**: Retreives season-level data, transform and store them in a table called season_data. It also extracts list of fixture_ids in the season and store it.
2. **pl_fixture_raw**: Uses the fixture_id list to make API calls for each fixture_id and store the raw data.
3. **pl_fixture**: Tranform the raw data of fixtures and stores the tranformed data in the table fixture_data.

## Technologies Used
1. Azure Data Factory
2. Azure Databricks
3. Azure Blob Storage (V2)
4. SQL Server

## Future Enhancements
 - Consolidate the three pipelines into a single orchestrated pipeline.
