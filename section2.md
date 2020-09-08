
## Section2 - Simple Recommendation Systems

These are non-ml techniques, can be achived by SQL, while they are still powelful.

`Popularity` - lots of prople willing to pay money for these products.

- `Issue`: just popularity, doesn't mean you want it. Especially when you travel to a new city, you don't want McDoald's even it's the most popular restaurant. News, no one want to see an outdated popular news.

`Context` - product associations. If a person wants to buy an iPhone, he/she might also want to buy an iPhone case. 

- `count(A,B)/count(B)`, if it's close to 1.

- `P(A|B)` - Conditional probability statesthat given an event (event A), it will only occur if an event (event B) has already occurred. 

- `Issue` people who bought baby bedsheet also bought normal bedsheet; but does people buy bedsheet also buy baby bedsheet, no.

- lift

![lift](arts/2-lift.png)

### Hacker News Formula

Since news is related very much to `age` (time), that's how Hacker News handle the recommendation

![Hacknews](arts/2-popularity-age.png)

We can see as the age grows, score grows sublinear.

![sublieaner growth](arts/2-p-a-diagram.png)

`Penalty` formula isn't known.
- if the link is too popular e.g. github.com
- too many comments - how controversial it is


"The known penalty is the powerful weapon of controlling media. isn't it?"


### Reading
- http://www.righto.com/2013/11/how-hacker-news-ranking-really-works.html
