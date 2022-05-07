# YOUTUBE TOP 200 TRENDING VIDEOS IN VIETNAM

## INTRODUCTION
### BACKGROUND
Youtube has increased its popularity a lot over the last few years. Many Vietnamese people of different ages are joining this community. It is easy to catch
some kids, adolescents, adults or even elders using Youtube. Since trending videos can demonstrate quite clearly tastes of the majority of Youtube users, 
An exploratory analysis on top 200 most popular videos may be helpful to find out those tastes as well as some patterns shared among those videos.
### OBJECTIVE
I decided to do an analysis and some basic visualizations for several reasons. 
- The first one to mention is that I want to discover Vietnamese people's tastes in Youtube videos.
- The second one is to find out some similar patterns and to help anyone with the intention of taking part in youtube content creator field.
- The last reason is to gain some experiences in working with data and to practice what I have learned so far.
## ANALYSIS
With the help of Youtube API V3, I could collect top 200 most popular videos in Vietnam and write the data to file **data.json**.

After that, the first thing I did is finding top 10 channels with the largest number of videos currently on trending.

<img width="560" alt="image" src="https://user-images.githubusercontent.com/105037210/167250510-be14a3ef-413e-4cb9-a0bf-202b19a8255f.png">

As can be seen from the above image, the largest number of trending videos which one channel could achieve is 3. The most popular channels include:
Anh Ba Phai TV, On Sports Plus, Ung Hoang Phuc, Tran Thanh Chuong, Lien Quan Mobile...,  MrBB Vlogs.

Then I generated some word cloud charts to see what keywords are used the most in Video titles, Video tags, Video 
description and Channel title.

<img width="381" alt="image" src="https://user-images.githubusercontent.com/105037210/167250731-7601f37f-3a34-495b-b250-3f96f8b102ef.png">
<img width="381" alt="image" src="https://user-images.githubusercontent.com/105037210/167250697-29754c1e-dcd8-48ff-95d8-b913661667b2.png">
<img width="381" alt="image" src="https://user-images.githubusercontent.com/105037210/167250755-67687cdc-1934-47af-8e17-6cca3813ee36.png">
<img width="381" alt="image" src="https://user-images.githubusercontent.com/105037210/167250762-e72b1dba-6457-4b87-a4b6-50155b19d98a.png">

I also counted the number of times some popular words appearing in video titles and video tags (you can see it in my code [here](https://github.com/hoongdoong/youtube-popular-vids-vn/blob/main/data_processing.ipynb)).
It is easy to understand why 'Viet Nam' word appears a lot of times on trending. It is mainly because the data is collected one day after the SEAGAME 31
football match between Vietnam Team and Indonesia Team. Therefore it is able to temporarily ignore the 'Viet Nam' word.
