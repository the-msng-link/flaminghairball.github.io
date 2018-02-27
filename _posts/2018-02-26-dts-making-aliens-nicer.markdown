---
layout: post
title:  "Making Alien Cruisers Nicer"
date:   2018-02-26 22:57:10 -0800
categories: dts game
---
Right now my Alien Cruisers look like this:
![game screenshot](https://www.dropbox.com/s/5nskwcsgyr3aqlj/2018-02-26%2022.32.08.gif?raw=1)

I don't like this because it looks unnatural the way they're all locked together in speed.
I've added a bit of variation in the speed which makes it look more like this:
![game screenshot](https://www.dropbox.com/s/4bjhj8kxgwy7nxo/2018-02-26%2022.34.33.gif?raw=1)

I like that a lot more. But I'm not satisfied with the way the aliens are spawned. They tend to come in waves across all 4 lanes at once -- I'd like a more noisy distribution.
The reason for this is that right now the obstacle spawner waits for x + rand(y, z) seconds before checking if it needs to spawn an obstacle -- where y and z are lower than x -- to remedy this I will lower x so that there is more noise than constant. The effect:
![game screenshot](https://www.dropbox.com/s/vwre02s7zi6uz6m/2018-02-26%2022.53.50.gif?raw=1)

That's better but still not 100% -- and it introduces a new problem -- because there's not as much buffer between obstacles, an alien cruiser that is faster than the one in front of it tends to collide. Whoops - these aliens will have to get a little smarter.

