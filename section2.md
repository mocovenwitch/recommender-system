
# Section2 - Simple Recommendation Systems

Content Table
- [Non-ML techniques](#Non-ML-techniques)
- [Hacker News Formula](#hacker-news-formula)
- [Raddit Formula](#Raddit-Formula)
- [Reading](#reading)

## Non-ML techniques
These are `non-ml techniques`, can be achived by SQL, while they are still powelful.

`Popularity` - lots of prople willing to pay money for these products.

- `Issue`: just popularity, doesn't mean you want it. Especially when you travel to a new city, you don't want McDoald's even it's the most popular restaurant. News, no one want to see an outdated popular news.

`Context` - product associations. If a person wants to buy an iPhone, he/she might also want to buy an iPhone case. 

- `count(A,B)/count(B)`, if it's close to 1.

- `P(A|B)` - Conditional probability statesthat given an event (event A), it will only occur if an event (event B) has already occurred. 

- `Issue` people who bought baby bedsheet also bought normal bedsheet; but does people buy bedsheet also buy baby bedsheet, no.

- lift

![lift](arts/2-lift.png)

## Hacker News Formula

Since news is related very much to `age` (time), that's how Hacker News handle the recommendation

![Hacknews](arts/2-popularity-age.png)

We can see as the age grows, score grows sublinear.

![sublieaner growth](arts/2-p-a-diagram.png)

`Penalty` formula isn't known.
- if the link is too popular e.g. github.com
- too many comments - how controversial it is


"The unknown penalty is the powerful weapon of controlling media. isn't it?"


## Raddit Formula

![fomula](arts/2-reddit.png)

`Controversy`

![controversy](arts/2-reddit-controversy.png)


>I think the main takeaway is that we have all this cool math and there interesting algorithms. But at the end of the day it's politics and money that get the final decision on what you see. Perhaps the only true way to remain neutral is to be governed by robots.


## Ratings
News feed items typically hae upvotes and downvotes, likes...

Amazon, Walmart has 5 star ratings.

At high level, you can think of
- binary outcomes as classification
- 5 star ratings as regression

Problem of Avarage rating
- confidence: one 5 starts is better than 2 thousands rating as 4.8 star? No.

>the more samples I collect (N) the skinnier it's distribution 


## Reading
- http://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html
