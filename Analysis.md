# YOUTUBE TOP 200 TRENDING VIDEOS IN VIETNAM

## INTRODUCTION
### BACKGROUND
Youtube has increased its popularity a lot over the last few years. Many Vietnamese people of different ages are joining this community. It is easy to catch some kids, adolescents, adults or even elders using Youtube. Since trending videos can demonstrate quite clearly tastes of the majority of Youtube users. An exploratory analysis on top 200 most popular videos may be helpful to find out those tastes as well as some patterns shared among those videos. 
### OBJECTIVE
I decided to do an analysis and some basic visualizations for several reasons. 
- To discover Vietnamese people's tastes in Youtube videos.
- To find out some similar patterns and offer some basic information to anyone with the intention of taking part in youtube content creator.
- To gain some experiences in working with data and to practice what I have learned so far.
### ABOUT DATASET
The dataset was collected on  07/May/2022 (the date executing these codes) in Vietnam region using Youtube API V3.
## EXPLORATORY ANALYSIS
### POPULAR WORDS
With the help of Youtube API V3, I could collect top 200 most popular videos in Vietnam and write the data to file **data.json**.
After that, the first thing I did is finding top 10 channels with the largest number of videos currently on trending.
<p align="center">
<img width="560" alt="image" src="https://user-images.githubusercontent.com/105037210/167250510-be14a3ef-413e-4cb9-a0bf-202b19a8255f.png">
</p>
As can be seen from the above image, the largest number of trending videos which one channel could achieve is 3. The most popular channels include:
Anh Ba Phai TV, On Sports Plus, Ung Hoang Phuc, Tran Thanh Chuong, Lien Quan Mobile...,  MrBB Vlogs.

Then I generated some word cloud charts to see what keywords are used the most in Video titles, Video tags, Video 
description and Channel title.

<p align="center">
  <img width="381" height=190 alt="image" src="https://user-images.githubusercontent.com/105037210/167250731-7601f37f-3a34-495b-b250-3f96f8b102ef.png">
  <img width="381" height=190 alt="image" src="https://user-images.githubusercontent.com/105037210/167250697-29754c1e-dcd8-48ff-95d8-b913661667b2.png">
  <img width="381" height=190 alt="image" src="https://user-images.githubusercontent.com/105037210/167250755-67687cdc-1934-47af-8e17-6cca3813ee36.png">
  <img width="381" height=190 alt="image" src="https://user-images.githubusercontent.com/105037210/167250762-e72b1dba-6457-4b87-a4b6-50155b19d98a.png">
</p>

I also counted the number of times some popular words appearing in video titles and video tags.

Counted popular words in Video Titles 

> {'phim': 15, 'phim lẻ': 4, 'tiktok': 10, 'shorts': 34, 'việt nam': 18, 'official': 18, 'highlights': 6, 'thử thách': 9, 'học': 10}

Counted popular words in Video Tags 
 
> {'tiktok': 201, 'phim': 247, 'garena': 22, 'official': 28, 'game': 102, 'tv': 113, 'bóng đá': 61, 'bão ngầm': 14, 'liên quân': 28, 'free fire': 36}

It is easy to understand why 'Viet Nam' and 'Indonesia' words appear a lot of times on trending. It is mainly because the data was collected one day after the SEAGAME 31 football match between Vietnam Team and Indonesia Team. The other popular words should be noticed include 'tiktok', 'phim', 'shorts', 'games', 'tv', 'thử thách', etc.

### CATEGORIES

After adding a new column named 'Category_name' into the dataframe based on the 'CategoryId', I grouped all videos into categories. Then I summed each category based on the number of view, like and comment.
These under images will explain more clearly.
<p align="center">
<img width="420" height=250 alt="image" src="https://user-images.githubusercontent.com/105037210/167285927-fecb36c8-a10e-4a19-9ddc-026e606263b5.png">
<img width="420" height=250 alt="image" src="https://user-images.githubusercontent.com/105037210/167285945-776ba219-6344-4e09-92cd-0ad7e461dad6.png">
<img width="420" height=250 alt="image" src="https://user-images.githubusercontent.com/105037210/167285999-44b56212-2f9a-4763-954e-9ad93be9e549.png">
</p>
Top-watched categories are Entertainment, Music, Sports, People & Blog. Among those, Entertainment and Music can be considered the most cared categories with the majority of users watching. It is understandable since many people using Youtube for relaxing and entertaining purposes. 
However, Education and News & Politics categories stand at the least trending ones although they bring more useful knowledge. (Opinion)

### PUBLISH HOURS
The column "PublishedAt" is written in UTC, so I converted it into a new column named "Published Hour" which is written in UTC+7 (I only took the publishing hour for analysing). After grouping all the videos into published hours, I generated a Bar Graph.
<p align="center">
<img width="404" alt="image" src="https://user-images.githubusercontent.com/105037210/167286787-0fc4bbaa-baa6-487d-88d0-cc1b5979de29.png">
</p>

As the bar graph demonstrates, the hours which the majority of trending Youtubers choose to upload their videos are between 18:00 and 20:00. In general, many trending content creators prefer to publish their videos during the evening than other periods.

## CONCLUSION
After conducting an exploratory analysis on the dataset of top 200 most popular videos in Vietnam, I can give some answers to the questions mentioned in the introduction.
- Vietnamese tastes when using Youtube include
  - Videos with the short time duration (inferred from 'tiktok', 'short' words in video title and tags)
  - Videos with contents of challenging, gaming, film, short film and sports.
  - Videos in 'Entertainment', 'Music', 'People & Blog', 'Sports' categories.
  - ...
- Some patterns which are shared betweent those videos include
  - Video content which can satisfies the popular tastes of users
  - Published hours are mainly between 18:00 and 21:00
  - ...
 - For anyone with the intention of being a youtube content creator, I hope you can find some useful basic information to consider when putting your very first step in that field.

To view my code [Click here](https://github.com/hoongdoong/youtube-popular-vids-vn/blob/main/data_processing.ipynb)
