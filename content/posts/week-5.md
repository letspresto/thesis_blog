---
title: "Week 5 | Imagined Currency"
date: 2018-03-19T12:51:51-04:00
draft: true
---

Recently on [Fresh Air](https://www.npr.org/2018/03/15/593863645/robots-are-now-creating-new-robots-tech-reporter-says), Cade Metz, a technology reporter, from the New York Times talked about how machines are learning on their own. My girlfriend forwarded me this episode because she found the discussion fitting considering I was utilizing machine learning techniques recently to help me find patterns in currency as part of my thesis. Here's Metz describing neural networks:

>
GROSS: So let's back up. These are systems that can - what did you say? They can learn on their own.
>
>
METZ: Exactly. They're called neural networks. And that's a metaphor. They're meant to mimic the web of neurons in the brain. But really, they're just math. They're mathematical algorithms that analyze data. A group of millions of photos is just data, and these systems look for patterns in that data - the way a nose curves on a person's face, the way the lines of an eye come together. They can identify those patterns, the math of those visual patterns, for instance, and then learn to recognize what is in an image. In the same way, it can recognize patterns in voice data and learn to recognize what people say.
>

Since my last post where I was looking for patterns in currency, I wondered if neural networks could hallucinate new forms of currency. For arguments sake, I thought about this solely in an aesthetic sense. This is particularly relevant because when I started my thesis, I was intrigued by the cryptocurrency craze and how to make sense of it. I thought of questions like 'How will my parents function in a world where they are familiar with holding physical currency?' Many people are touting cryptocurrencies as the future. And as of today [Coin Market Cap](https://coinmarketcap.com/all/views/all/) lists over ~1500 cryptocurrencies in existence. Often I look to history to try and see if there are instances which mimic how the present-day is unfolding. There's a rich field of financial historians or anthropologists who have studied how various empires, cultures, and societies evolved with the focal point being money. Experts like [Rebecca Sprang](http://www.hup.harvard.edu/catalog.php?isbn=9780674047037), [Niall Ferguson](https://en.wikipedia.org/wiki/Niall_Ferguson), and [Bill Maurer](https://www.dukeupress.edu/how-would-you-like-to-pay) have all been helpful in my research. 

Here's one factoid that was interesting by Bill Maurer in 'How Would You Like to Pay?'

>
Prior to the invention of state-­ issued currency, a variety of private moneys circulated— as recently as the 1860s in the United States, there were around eight thousand currencies, issued by banks, railroad companies, retail stores, and other entities. The National Bank Act of 1863 began a decades-­long process of consolidating the national currency in the United States, completed by the Federal Reserve system in the early twentieth century.
>

So is living in 2018 with thousands of various cryptocurrencies any different than living in the mid-1860s in the U.S. with thousand of currencies? Regardless of what you or I think, it's an interesting thought exercise and something that we're living in. 

My dataset of currencies suprisingly had plenty of old currencies from that time-period. Using this I embarked on using neural networks to 'create' new currencies. I ended up using this Tensorflow implmentation of a [Deep Convolutional Generative Adversarial Networks (DCGAN)](https://github.com/carpedm20/DCGAN-tensorflow). I leave you with how this neural network generated new currencies. 

![500epoch](/images/500e.gif)
