---
title: "Week 4 | Currency Sick"
date: 2018-02-28T17:55:55-05:00
draft: false
---

Apologies for the late post, but I came down with the flu which knocked me out for a good week. Luckily, I was able to rapidly experiment a bit after my last post where I chronicled acting as a human foreign exchange collecting currencies. I quickly realized that I wasn't going to scale my learning of currencies by physically acquiring currencies in-person, so I decided to programatically write some scripts to help me collect currencies from some online sources. Using python, Beautifulsoup, and some digging around for sites, I eventually was able to cull ~6,200 images (half front of banknotes & other half back of banknotes) of currencies which go as far back as the 1750s when shillings were printed papers using leaf impressions. 

While taking Understanding Networks last semester, a class where we explored network topologies, my professor once quiped that currencies can also be thought of as a network during a discussion. Often technologies seldom stand alone as they exist in networks and they facilitate networked connections between people. For these experiments, I wanted to use tools to help me find elements and patterns that connect currencies together and what hold them together. [Gene Kogan](http://genekogan.com/) recently visited ITP to run workshops on [machine learning for artists](https://ml4a.github.io/), which was perfect timing for me to run these experiments. One technique I did was clustered the currencies using the t-sne algorithm, which attempts to extract feature vectors from the images then places them in 2d space based on similar features. Here's ~2000 currencies clustered together:

![tsne](/images/back.png)

What's fascinating about using this technique is how quickly t-sne is able to visualize high dimensional data and aid me in seeing patterns in image data. For instance, in my dataset which contained the back of banknotes, it clustered these two currencies for its large red typeface which stood out as the denominations ($10 and $25) of those particular bills. 

![zoom1](/images/zoom1.gif)

Another pattern you can see from the evolution of currencies are the prominence of individuals on bills. This made me pause for a second because I started to wonder when using cultural figures became a trend with issuing currencies. Was this a way to preserve significant cultural value for a soverign nation with their citizens using these bills? If so, how were these individuals chosen and was it by consensus or by a central authority? 

![faces](/images/faces_bills.png)

Let's look at the yellow bill in the lower-left quadron, which is a Ukrainian hryvnia displaying [Vladimir the Great](https://en.wikipedia.org/wiki/Vladimir_the_Great#Significance_and_legacy). When it comes to his legacy, Vladimir was reknowned for having consolidated the Kievan Realm in late 9th to the mid-13th century. The modern peoples of Belarus, Ukraine and Russia claim the Kievan Realm as the origin of their cultural ancestors who were from various East Slavic tribes. As wikipedia claims of Vladimir's legacy: 

>During his leadership, all branches of the economy prospered under him. He was able to mint coins and regulated foreign affairs with other countries such as trade. Through trade he brought in Greek wines, Baghdad spices, and Arab horses to trade at the markets of Kiev.
>

This is just one example, but it does lead me to think about how each currency ever created has a story with a mythical hero. In 2009, Satoshi Nakamoto is an unknown person who designed bitcoin. Would we see his bust on a cryptocurrency bill? 