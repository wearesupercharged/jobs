# Backend Engineering Challenge

Thank you for your interest in the Supercharged Software Engineer team! This project gives us a chance to see your Backend engineering programming skills.

Please complete this challenge and make your repository accessible to:

- [iamsupercharged](https://github.com/iamsupercharged) (rayan@supercharged.gg)


**Small Backend making use of the Twitter API**

Build a backend service that gathers data from two different endpoints of the Twitter API and writes it to a json file every 5 seconds. 

Twitter profiles we like (you can choose your own too) :
	@elonmusk
	@naval
	@reidhoffman
	@ninja
	@wendys

You should make use of the following endpoints: 

- [GET statuses/timeline](https://developer.twitter.com/en/docs/tweets/timelines/api-reference/get-statuses-user_timeline) in order to fetch the timelines of 5 different twitter accounts
- [POST statuses/filter](https://developer.twitter.com/en/docs/tweets/filter-realtime/api-reference/post-statuses-filter) in order to fetch @realDonaldTrump's profile updates

Each of these actions need to be performed in separate code chunks, gathered together and written to a different JSON files 5 times, every 5 seconds. 

The action should stop once it has finished fetching each profile and created 5 different JSON files. 

![](base-architecture.png)

**Implementation in AWS**
Think about how you would organize this project's architecture in AWS, if data was not written in JSON but rather sent through webhooks. A simple drawing of your different AWS components will work.


## Other Tips

- Think about how this could be done while many users would be fetching different twitter accounts. So better avoid global variables. 
- You do not need to write a front-end for this project, postman will work. 
- The goal of the exercise is to showcase not only your ability to 
