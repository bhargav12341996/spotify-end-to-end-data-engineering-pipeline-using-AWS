# spotify-end-to-end-data-engineering-pipeline-using-AWS

In this project, I built end-to-end data engineering pipeline using Spotify API on AWS. In this project, I have worked on "BILLBOARD HOT 100 SONGS" playlist and extracted the data related to all the artists, songs & albums. This extracted data is in .json format and using Python pandas library we have transformed the document type data into structured dataframe format which is then crawled using AWS crawlers. These tables are further used for data analysis using AWS Athena analytical service.

## Architecture used in building this project:

<img width="1895" height="1045" alt="image" src="https://github.com/user-attachments/assets/6c63c991-cc04-4912-bf3e-cabfce0f639c" />

## Steps involved in implementing this project:
- Connected with Spotify API and extracted data using Spotipy package. Imported spotify and pandas package as custom layers to properly integrate with AWS lambda function.
- Deployed Lambda functions to extract the data and transform the data.
- Worked with Amazon S3 buckets to store both raw data and transformed data.
- Used AWS EventBridge (Cloud Watch Events) to set trigger and to schedule the data extraction in regular time intervals.
- Worked with AWS glue crawlers to infer schema for the transformed tables.
- Used boto3 python SDK at both resource and client level to communicate with different AWS services.
- Performed data analytics using AWS Athena analytical services.
- Performed data masking using environment variables to hide the sensitive data.
