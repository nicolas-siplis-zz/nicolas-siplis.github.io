---
layout: post
title: "'Inventing' treesort"
subtitle: "Or how I learned to keep trying and avoid Google"
date: 2015-11-12
author: "Nicolás Siplis"
---

Here’s some context for those of you who don’t know me, and since I’m a 19 year old argentine student that probably includes pretty much every single person reading this post. I’m in my first year of computer engineering, loving it so far and can’t wait for the next one.

We started looking at recursion and tree-like structures this semester, and as you probably know one of the most simple structures to study is the binary tree. Not gonna get into specifics, just remember that a balanced binary tree allows us to insert and search for a node in *O(log n)* time.

We had seen sorting algorithms previously, and the complexity of the ones we studied (insertion and bubble sort) was *O(n²)* in both cases. So, now you have a first year student who thinks he’s on to something. If inserting and retrieving nodes from a balanced binary tree is *O(log n)*, I realized I could construct a binary tree from an array and then sort it in *O(n log n)* by reinserting the elements from the tree.

At this point, I actually got excited! Up until then, most of the things we had done were pretty much direct applications of what we had been taught, creativity not being the most useful quality. However, I had come up with a sorting algorithm from scratch! Well, not really from scratch since I was just combining two highly related concepts. But still, not bad for my second semester!

Naturally I wanted to brag about my discovery to someone, so I created a basic implementation of the algorithm and compared it with the insertion and bubble sorts. It took a bit longer than expected since I had to actually learn how to create a self balancing binary tree (which I suspect will come in handy next year). However, after some time and effort I got everything to work.

As expected, the “new” sorting method was significantly faster than both bubble and insertion sort. I walked up to the professor after class and talked to him about it. He let me ramble on and on about how I came up with it, how it worked and the speed comparisons. Once I was done, the conversation went something like this.

> So, you implemented treesort.
>
> What?
>
> Yeah, it’s a pretty well known sorting algorithm. Not the fastest but it does have some pretty cool properties.
>
> So someone already thought of all this?
>
> Yep.
>
> … I need to learn how to Google before getting excited.

I’m going to take a wild guess and say that 100% of the ideas I’ll think of in the years to come have already been implemented, discussed and improved dozens of times long before I was born. Googling them might be faster, but luckily I’m not a computer so I don’t care about speed. I care about having fun, and coming up with an algorithm on my own (and learning a whole lot in the process) was really, really fun.

Besides, if people call Columbus the discoverer of America then I sure as hell can call myself the discoverer of Treesort.
