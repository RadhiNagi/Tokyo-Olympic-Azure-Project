Project Overview:
The Spotify Data Pipeline project automates the extraction, transformation, and loading of Spotify data for analysis using Microsoft Azure services.

Key Components:
Azure Functions:

Purpose: To extract raw data from Spotify and store it in Azure Blob Storage.
Steps:
Uses spotipy to interact with the Spotify API.
Extracts playlist data and stores it as a JSON file in Azure Blob Storage.
Triggers an Azure Data Factory pipeline to process the extracted data.
Azure Data Factory:

Purpose: To transform the raw Spotify data and store the transformed data back into Azure Blob Storage.
Steps:
Reads JSON data from Blob Storage.
Processes the data to extract relevant details about albums, artists, and songs.
Writes the transformed data back to Blob Storage in CSV format.
Azure Synapse Analytics:

Purpose: To load the transformed data into Synapse tables for querying and analysis.
Steps:
Creates tables for albums, artists, and songs.
Loads data into these tables using the transformed CSV files from Blob Storage.
Sets up Synapse pipelines to automate data loading.
