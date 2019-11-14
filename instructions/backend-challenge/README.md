# Backend Engineer Challenge

Thank you for your interest in the Supercharged Software Engineer team! This project gives us a chance to assess your programming skills.

Please complete this challenge and make your repository accessible to:

- [iamsupercharged](https://github.com/iamsupercharged) (rayan@supercharged.gg)


**Small Backend making use of the Twitter & Spotify API**

You should make use of the following endpoint to listen to the real-time tweets from 5 different profiles:
- [POST statuses/filter](https://developer.twitter.com/en/docs/tweets/filter-realtime/api-reference/post-statuses-filter)

Twitter profiles we like (you can choose your own too) :
	@elonmusk
	@naval
	@reidhoffman
	@ninja
	@wendys

You should also make use of the [Spotify Web API](https://developer.spotify.com/documentation/web-api/) in order to fetch your currently played song every second (with song name, artists and progress). 

Aggregate the twitter notifications together with the last fetched spotify song and write the new data to a new JSON file every 5 seconds. Stop the action once 7 files have been created.

![](base-architecture.png)

## Implementation in AWS ##

Think about how you would organize this project's architecture in AWS, if data was not written in JSON but rather sent through webhooks to a front-end listener. A simple drawing of your different AWS components will work. 

## Other Tips

- You have the freedom to use any third-party library 
- Think about how this could be done while many users would be fetching different twitter accounts. So better avoid global variables. 
- You do not need to write a front-end for this project, postman will work. 
- In designing your AWS solution, think security, efficiency, scalability (with many concurrent users in different locations of the world)
- The goal of the exercise is to showcase not only your ability to write code but also think of scalability. 
