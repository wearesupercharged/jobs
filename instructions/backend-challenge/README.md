# Backend Engineer Challenge

Thank you for your interest in the Supercharged Software Engineer team! This project gives us a chance to assess your programming skills.

Please complete this challenge and make your repository accessible to:

- [iamsupercharged](https://github.com/iamsupercharged) (rayan@supercharged.gg)


**Small Backend making use of the Twitter API**

Use the Twitter API to fetch sequentially (one by one) 5 different profile's statuses with the following endpoint:
-  [GET statuses/timeline](https://developer.twitter.com/en/docs/tweets/timelines/api-reference/get-statuses-user_timeline)

Twitter profiles we like (you can choose your own too) :
	@elonmusk
	@naval
	@reidhoffman
	@ninja
	@wendys

In a separate service, you should make use of the following endpoints to listen to the real-time tweets from @realDonaldTrump:
- [POST statuses/filter](https://developer.twitter.com/en/docs/tweets/filter-realtime/api-reference/post-statuses-filter)

Aggregate the twitter notifications with the fetched timeline and only write them in a JSON file every 5 seconds. Then move to the next twitter profile and aggregate it with donaldtrump realtime tweets in another JSON file. This action should only stop once it has finished fetching each profile and created 5 different JSON files. 

![](base-architecture.png)

## Implementation in AWS ##

Think about how you would organize this project's architecture in AWS, if data was not written in JSON but rather sent through webhooks to a front-end listener. A simple drawing of your different AWS components will work. 

## Other Tips

- You have the freedom to use any third-party library 
- Think about how this could be done while many users would be fetching different twitter accounts. So better avoid global variables. 
- You do not need to write a front-end for this project, postman will work. 
- In designing your AWS solution, think security, efficiency, scalability (with many concurrent users in different locations of the world)
- The goal of the exercise is to showcase not only your ability to write code but also think of scalability. 
