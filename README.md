# YOUTUBE TOP 200 POPULAR VIDEOS IN VIETNAM
In this project, I did an exploratory analysis and some visualizations on top 200 most popular videos on Youtube Vietnam. The goal is to discover some similar patterns between these videos.
## DATASET
Dataset includes top 200 trending videos in Vietnam region on 07/May/2022.

Attributes include:
- Published Date
- Channel ID
- Channel Title
- Video Title
- Video Description
- Tags
- Category ID
- View, Like, Comment Count
- Others
## DATA SOURCE
The dataset is gathered using Youtube API V3 in Vietnam region.

If you need more information [Click here](https://developers.google.com/youtube/v3/getting-started)
## TO RUN
- Clone the project
- Open and run file **get_top_200_video.ipynb** (remember to replace **client_secrets_file** with yours)
- For more information on how to get **client_secrets_file** [Read here](https://stackoverflow.com/questions/40136699/using-google-api-for-python-where-do-i-get-the-client-secrets-json-file-from)
- Open and run file **get_category.ipynb** (remember to replace **client_secrets_file**)
- Open and run file **data_processing.ipynb**

Data gathered will belong to the date running these codes.