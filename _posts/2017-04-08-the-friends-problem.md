---
id: 626
title: The Friends/Strangers Problem
date: 2017-04-08T07:00:00+00:00
author: CJeremy
layout: post
guid: https://blog-cjeremy.rhcloud.com/?p=626
permalink: /2017/04/08/the-friends-problem/
categories:
  - Uncategorized
tags:
  - Mathematics
  - puzzle
---
I recently came across a pretty interesting puzzle that used a different kind of mathematics &#8211; called Ramsey theory &#8211; in order to tackle the problem.

Here&#8217;s the problem:

_Suppose you have a group of six people. Show that you will necessarily have at least three mutual friends or three mutual strangers._

This is a sort of pigeonhole problem, which sort of means that we have to make a binary choice for each person. But what I love about this proof so much is that it&#8217;s entirely visual and fairly easy to grasp.

First, let&#8217;s imagine we have six people, who we can each represent as dots.

<img class="aligncenter wp-image-623 size-full" src="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-e1491573011500.png?fit=402%2C260" alt="" srcset="https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-e1491573011500.png?w=402 402w, https://i0.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-e1491573011500.png?resize=300%2C194 300w" sizes="(max-width: 402px) 100vw, 402px" data-recalc-dims="1" />

From there, we want to show the relationships between people. To do this, we will use lines to mark the type of relationship two people have. We will use orange to represent friends, and blue to represent strangers.

To begin, we need to start drawing lines. The first thing that you need to know is that there will _always_ be at least three lines of any one colour that goes out from one person. The reason that this is true is because if we look at one person, the five others have no choice but to be friends or strangers. As such, every person will have at least three orange _or_ blue lines connecting to other people, so we can simply choose one scenario of having three friends, which means three orange lines. We&#8217;ll connect them to other people at random, and so we get the following scenario.

<img class="aligncenter wp-image-624 size-full" src="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-1-e1491573056850.png?fit=400%2C269" alt="" srcset="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-1-e1491573056850.png?w=400 400w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-09-PM-1-e1491573056850.png?resize=300%2C202 300w" sizes="(max-width: 400px) 100vw, 400px" data-recalc-dims="1" />

Now that we&#8217;ve got three lines down, we know that each line represents a friendship between the people. But notice that, to show what we&#8217;ve set out to do, we only need to have one of _those_ three friends also be friends. Put differently, if we can find a friendship such that we get a triangle of a single colour, we will prove our statement. However, it&#8217;s trivial to simply draw a triangle of one colour and say that we&#8217;re done. Instead, we need to show that we&#8217;ll be _forced_ to make a triangle of one colour, no matter how much we don&#8217;t want to.

Suppose we consider one of those friends who were touched by our original rays. If we look at Person 4, they are friends with Person 1. Additionally, we see that Person 1 is friends with Person 3 and Person 5. Therefore, if we draw a friendship line between _either_ Person 4 and Person 3, or Person 4 and Person 5, we will create a triangle of one colour, which means three people are friends. Since we&#8217;re trying to avoid that at all costs, we will draw two blue lines between these people, making sure that no orange triangles are created. This give us the following:

<img class="aligncenter wp-image-625 size-full" src="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-10-PM-e1491573088771.png?fit=372%2C261" alt="" srcset="https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-10-PM-e1491573088771.png?w=372 372w, https://i2.wp.com/blog-cjeremy.rhcloud.com/wp-content/uploads/2017/04/Image-2017-04-06-8-10-PM-e1491573088771.png?resize=300%2C210 300w" sizes="(max-width: 372px) 100vw, 372px" data-recalc-dims="1" />

But what, we now have a problem. Look at the line we will need to eventually draw between Person 3 and Person 5. If we draw an orange line between them, then we will create an orange triangle between Person 1, Person 3, and Person 5. But on the other hand, if we draw a blue line between Person 3 and Person 5, we&#8217;ll be creating a _blue_ triangle between Person 3, Person 4, and Person 5. Therefore, we&#8217;re stuck!

This means that no matter what, a group of six people will have at least three mutual friends _or_ three mutual strangers. Using this technique, we&#8217;ve _pigeonholed_, or forced, ourselves into this situation.

What I like the most about this proof is that it&#8217;s visual and easy to understand. It&#8217;s what happens when you apply logic at each step, until you arrive at an undeniable conclusion. Furthermore, it&#8217;s a glimpse into a type of mathematics that wasn&#8217;t shown to me in school, so I thought it would be interesting to share. As I mentioned, I first saw this from a [video by Raj Hansen](https://www.youtube.com/watch?v=7p76yYMth5A&list=PL3dVWQq5Sx9cEjb5W_4WVxSMPy9PnsP4d) who explains this problem in the introductory video to his Ramsey theory series. You should definitely check it out if you find this proof interesting. Personally, I&#8217;m excited to see what other kinds of applications we can find for Ramsey theory.