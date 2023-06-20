# Python3 Networking Library Tests
A small script to test RPS of multiple different python librarys

`python3 main.py -tc X -tl Y -url Z`

My results: 

[requests results] 5.833

[urllib3 results] 8.5

[asyncio & httpx results] 11.5

[httpx results] 11.667

[sockets results] 46.0

## Conclusion:

requests is all around very stable and easy to use.

urllib3 is very fast but is a bit more complex.

httpx is a bit of a mixed bag , sometimes it is really fast other times urllib3 and requests will beat it, not sure i would recommend it.

sockets is phenomanly fast considering you do not need to deal with responses but if you would like to you can use .recv(), very good if you need something fast and also something more configurable .
