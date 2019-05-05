# Intro to System Design

## Analysis process in system design problems

- Scenario <br>
What features needs to be designed?<br>
Ask/ Features/ QPS/ DAU/ Interfaces

- Service <br>
Divide the large service into small parts<br>
Split/ Application/ Module

- Storage <br>
How the data be stored and visited?<br>
Schema/ Data/ SQL/ NoSQL/ File System

- Scale <br>
Upgrade the system. Handle possible problems.<br>
Sharding/ Optimize/ Special Cases

## Scenario

### Ask the interviewer: <br>
**What features need to be implement?** (Or you can figure out some extra feature yourself.)<br>

1. Enumerate the features one by one<br>
e.g. Register/Login, User Profile Display / Edit, Upload Image / Video, Search, Post / Share a tweet, Timeline / News Feed, Follow / Unfollow a user,etc.

2. Sort the core features (You don't have time to design then all!)<br>
e.g. Post a Tweet, Timeline, News Feed, Follow / Unfollow a user, Register/Login.<br>

**Ask about visitors** 

- DAU: daily active users
- MAU: monthly active users
- Read QPS
- Write QPS<br>

e.g.Twitter: MAU 330M, DAU ~170M+ <br>

### QPS conditions
- QPS = 100 <br>
Just use your laptop as the web server

- QPS = 1k <br>
Use a single web server and take single point failure into consideration.

- QPS = 1m <br>

Builder a cluster of 1k web servers and take maintainance into consideration(What if one of the web servers fails).

- Approximately relation between QPS and Webserver/Database <br>

One webserver for 1k QPS/ One SQL database for 1k QPS/One NoSQL Database (Cassandra) for 10k QPS/One NoSQL Database (Memcached) for 1m QPS



## Services




















