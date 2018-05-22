---
layout: post
title: Iterating to Success
category: posts
---

I recently launched [my first web app](https://www.flattestroute.com/), it was my final project at [Hackbright Academy](https://hackbrightacademy.com/). The idea for the project came about almost a year ago when, as a Bay Area newbie, it felt like I always took the steepest route possible while travelling around San Francisco. There had to be a better way.

When I joined Hackbright in March, I knew what I wanted to do for my project: help me (and other people too) find the flattest route while navigating San Francisco.

## First Iteration

My initial plan was to provide a simple directions finder like Google Maps but would auto-calculate a route that minimized slopes.

However, before writing a single line of code I decided to see if there were other apps that could do this already. There were a couple of options: [511.org](https://bicycling.511.org/) and [Mapquest](http://www.mapquest.com/). Both apps had options to avoid hills.

![Screenshot of iteration 1](https://i.imgur.com/vuy0Z8z.png)

By using the existing apps, I discovered three drawbacks:

1. They did't show the original route so I couldn't tell if the suggested route was the "best" route.

2. There was no elevation information displayed so I couldn't tell if there were still hills present.

3. I couldn't tell how much of a detour I had to take to flatten the route.

Based on my impressions of the apps available, I decided to improve upon what existed and go in a different direction than I originally intended.

## Second Iteration

I decided to show graphs of elevation and slope information along the suggested route so users could decide if the given route was too steep, letting the user find the flattest route themselves. I included sliders that the user could adjust based on their own slope preference (one for uphill, one for downhill). If the slope became steeper than what they had specified, that section of the route would be colored red.

![Screenshot of iteration 2](https://i.imgur.com/IUGhlbB.png)

To test for useability, I had my classmates and mentors try out this version of the app. I discovered that users found the sliders confusing since their purpose wasn't immediately obvious. Users didn't know yet what their slope thershold should be. This told me that my app needed to provide more guidance and remove the controls that users couldn't understand.

## Third and Final Iteration

Since the users didn't know what slopes they could handle, or even what the grades of a given slope meant (do you know how awful a 10% grade is?), I needed to determine the slopes the average pedestrian/cyclist would tolerate. Based on what I found on some [hiking](http://www.venturacountytrails.org/TrailMaps/TrailSymbols.htm) and [biking](https://www.bicyclenetwork.com.au/) sites, I determined the color scheme for the slopes, removed the slope slider, replaced it with a color legend, and redrew the path in the legend's colors to visually show the slope directly on to the map.

By providing the user with slope info, they are now empowered to find their own flattest route according to their own preferences.  As a nice side effect, it also allows them to find the steepest route if they're so _inclined_.

![Screenshoot of iteration 3](https://i.imgur.com/YbJkG8I.png)

This process must have worked because shortly after publishing my app it made it to [the top of Hacker News](https://news.ycombinator.com/item?id=5672515)!

In retrospect it looks like this should have been obvious but it only seems that way thanks to a bit of useability testing and research.

