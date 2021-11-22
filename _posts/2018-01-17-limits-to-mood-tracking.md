---
title: "An Exploration of Mood Tracking: Can We Measure How We Feel?"
layout: post
categories:
  - Tracking
  - Quantified Self
  - Track Everything
  - Mood
  - Mood Tracking
comments: true
published: true
date: 2018-01-17
---

{% picture center /images/2018-resources/mood-tracking-cover.jpg %}

**What is a mood? Can we track it? Can we improve it?**

After a few previous failed attempts, I decided to try another exploration into mood tracking.

CONFESSION: I’m not depressed and not particularly prone to the “blues” either. I do have waxing and waning motivation and drive though. In fact, I tend to be a good mood most of the time and quite productive too.

Instead, I’m curious self-tracker, and for this mood tracking experiment, I wanted to see if I could better understand what affects my mood by tracking it. Hopefully, eventually, I can avoid factors that create negative moods and optimize my life to be in a better mood more often.

Unlike other tracking metrics like productivity, money or even the somewhat ambiguous idea of measuring good heath, mood isn’t easy to quantify. It’s difficult to be objective about our moods or even “score” our current mood. Scientists also struggle with measuring our moods for both practical and even philosophical reasons.

In this post, we will explore what is mood tracking and some of the problems in measuring it. We will take a look at the psychological understanding of moods and different ways scientists measure it. In the conclusion, I’ll share some of the problems I see in mood tracking.

NOTE: In future posts, I’ll share my review of a few mood tracking apps as well as how I tracked my mood and what I learned.

<!--more-->

## What is Mood Tracking?

Mood tracking is the act of quantifying your current mood.

Mood tracking or mood monitoring has existing in therapeutic psychology since the 1960s. It’s typically used as a form of self-help, self-awareness and self-tracking for people suffering from mood disorders like anxiety, clinical depression, and bipolar disorder.

{% picture right /images/2018-resources/mood-tracking-scale.png %}

I’ve included a table of the Mood Scale used with Bipolar disorder. This is a fairly typical method of measuring moods in psychology.

The simplest method for mood tracking is through a diary or chart where you record your mood on a scale and optionally provide additional notes. You can then use this log to understand your mood changes over time, search for patterns, and implement changes to improve your mood. This log can help you help yourself but also help your doctor understand and treat more serious mood disorders.

With rise of the software and smart phones, it’s increasingly easy to track your mood on your computer or phone. In fact, there are dozens of apps that can help you track your mood.

These apps reveal just how little we still understand about moods and, not surprisingly, present a lot of different approaches in how we can measure our moods. It seems that apps like professional scientists and psychologists are still struggling with how best to track our moods too.

Let’s look briefly at what are moods.

## What is a Mood? Binary and Linear Scale Moods

Moods are an expression of our emotional state.

According to Wikipedia, "In psychology, a mood is an emotional state. In contrast to emotions, feelings, or affects, moods are less specific, less intense and less likely to be provoked or instantiated by a particular stimulus or event. Moods are typically described as having either a positive or negative valence. In other words, people usually talk about being in a good mood or a bad mood.”

This is a decent working definition. In this definition, moods are more of a “state" and less prone to stimulus response you get in emotions and affects. Moods stand in for a more long-lasting state of how we feel or consider our situation. In the simplest sense, we often say our mood is positive or negative and sometimes just so, so or neutral.

When it come to tracking moods, we could stop here in a quest to understand moods and just measure our mood as either positive or negative. It is an abstraction in view how complex the nexus of emotions and language for emotions are, but this positive/negative mood remains a simplistic and practical approach.

For example, for tracking purposes, all you need to do is measure your mood as positive, negative or some variance to collect a mood data point.

The binary scale of a “good mood" vs. "bad mood" remains the most common approach to mood tracking. Many apps and surveys still use it.

A variation would be put this on a linear scale from extremely good mood to extremely bad mood with states in between like good, so, so, neutral, etc.

Whether it’s a 3-point scale, 10-point scale or some variation, these mood measurements present a simplistic framework for our moods:

{% picture center /images/2018-resources/moods-on-a-scale.jpg %}

From a tracking perspective, this subjective scoring on a scale is the simplest way to track your mood. You log a mood as one thing and not another. For therapeutic psychology, mood tracking this way is a nice heuristic tool.

From a computational and data scientist’s standpoint, binary or linear states make for clean data and easier modeling. As such, if you want to track your mood, positive, negative or neutral can be a pretty good approach.

Unfortunately, like much of what goes on in our emotional and mental lives, the reality might not be so simple. Mood tracking as states (especially binary states!) isn't a real thing; it’s an abstraction.

Just ask yourself, is your mood simply positive, negative or neutral? Or is it more complicated?

If you are being honest (and not a robot), the most likely answer is no, our mood isn’t an either/or. Our emotions and moods are not simple states, and if pushed to the extreme, we cannot quite ever measure our moods.

## Complexity of Our Moods and Emotions

The problem with this binary or linear scale for mood tracking is not that it isn’t capturing something about our moods, but that is an abstraction.

Our moods and emotions are not so binary or clearcut in reality. Unlike computers, we rarely exist in "mood states" like we'd want to track. Our moods aren’t discrete states.

The same problems appears in the history of economics and behavioralism and its critique of rationality. While we have attempted to imagine and model human actions as rationally as possible, humans are not pure rational, economic, abstract agents. Our actions are a convergence of multiple forces include motive, environment, social and many others. We don’t act in a classical “economic” manner.

Like behavioral models that attempt to understand why we act in certain ways, emotional and mood models aren’t simply about on/off states. Our moods exist in a convergence of dimensions rather than as discrete states. This idea of framing emotions and moods in terms of dimensions instead of states significantly changes how we think about mood, define it or even track it.

One interesting takeaway from this new framework is that we can have multiple moods at the same time. For example, we could be both happy and sad at the same time. Everything falls on a scale and multiple factors are part of what encompass our mood.

Several psychologists and social scientists have proposed ways we can “measure" our moods on a dimensionally scale. Using this alternative framing of moods, they present mood as measured through a prism of multiple questions about specific aspects of feelings, energy levels and mental states. This can then be used to provide a portrait of our mood.

One example of moods in terms of dimensionality scale is Circumplex Model, which can visualize this way:

{% picture center /images/2018-resources/moods-circumplex.jpg %}

There is also the Brief Mood Introspection Scale (BMIS):

{% picture center /images/2018-resources/moods-BMIS.png %}

There is no neutral state when we measure our mood using the BMIS survey. Instead we have a range of factors that can interpreted into an overall score or definition of our mood.

Arguably this approach is a more robust way of capturing moods. By quantifying an array of emotions and states, we can then put our general mood into different buckets. We can also find relationships between a few aspects of our mood and our positive or negative mood too.

Personally I find this approach to an interesting one, but I find it adds a lot of dimensions that it can be harder to use. For example, you get a lot more data points and connecting it to effectively reflect on your mood becomes harder. As such, I think this multifactorial approach to mood tracking is probably best left to the experts. Even for data analysis multifactorial data points add a lot more complexity.

## Conclusion: Challenges to Mood Tracking

Amongst everything I track, I’ve yet to find a clear and easy method of quantifying my mood. Mood tracking is challenged on two sides.

Firstly, we lack a clear psychological framework for emotions, sentiments and moods. We don’t even have a simple definition of what is a mood, though there are various proposals that try to frame mood within a construct of related concepts. For example, the simplest way to define mood would be either positive or negative.

Secondly, we don’t have a simple and defined protocol to capture and measure moods. When you don’t know what is a mood, it’s difficult to measure it. This has resulted in several psychological approaches to measuring our mood or alternatively our emotions.

Mood tracking is a challenge for both science and for individual self-trackers. The science is unfinished on defining what is a mood and how best to measure it. Because we don’t know what is a mood and we struggle with a host of factors that relate to our emotional and mental state, it’s not easy to come up with a simple method that would capture our mood at a single point during the day and help us aggregate or score our mood on longer time scales.

These philosophical problems haven’t stopped us from trying to measure our moods, especially for certain diseases. Depression and bipolar disorder are two diseases in particular where mood monitoring matters for both the patient and for their doctors. Both of who want to understand their mental state and what triggers certain emotional highs and lows.

In spite of all the limitations and challenges to measuring I mood, I decided it was an area worth attempting to measure. There are also a number of apps which make capturing your mood pretty seamless on an app or even apple watch. Considering I have good data on my productivity (RescueTime, Todoist), on my health (HRV, Blood Testing, Resting Heart Rating) and on my fitness (Running and Training Logs) (and I am able to visualize all of this data too), it feels like time to track tracking my mood. More on this experiment to come.

_Have you ever tried to measure your moods? What do you use? And what have you learned?_
