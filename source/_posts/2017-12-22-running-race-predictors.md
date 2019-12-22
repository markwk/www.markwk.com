---
title: "Running Your Best: A Comparison of Race Predictors, Calculators and Models"
layout: post
categories:
  - Tracking
  - Self-Tracking
  - Quantified Self
  - Personal Data
  - Track Everything
  - Running
  - Marathon
  - Predictions
comments: true
date:   2017-12-22
published: true
---

{% img center /images/2017-resources/race-predictors-for-runners-cover.png %}

Running your best race requires a number of good things to happen. You need to have done solid training and gotten yourself as ready as possible. You need to be healthy and well-rested. You need to know the conditions and have the necessary gear for the race. But arguably one of the most important factors in running your best is having a good prediction. 

There are a number of tools and methods online to to estimate and predict your next race time. These race predictor calculators looks at factors like weekly running distance and previous time at a short distance (like the half marathon or 5k) to guess your expected next race time. 

While there is a segment of runners who just want to finish and don’t care much about performance or improvement, I don’t really include myself in that group. Like the vast majority of runners I know, we are trying to run our best at races. We want hit a target and get a Personal Best (PBs). 

Later this week I’ll be running my second marathon in Chiang Mai, Thailand. I’m happy to say that my training has gone quite well. I’ve been using an [smart, adaptive training program from TrainAsOne](###) in order to push my different capacities, avoid injury and get myself ready. At the time of writing, my conditions are good. I’m not sick, and I’ve been getting good sleep and decent nutrition. 

In this post, I want to look at several of the predictors, calculators and models used to estimate run times. We will be using my recent half marathon score (1:45:00) and training log to see what these models predict from my next race. Unfortunately, there are a lot of models and predictors out there and there is some degree of variance. Several of the older models were purely mathematical and their predictions are dangerously optimistic. More recent models are based on statistical data and algorithms to make their predictions. 

<!--more-->

## Why Accurate Race Predictions Matters

Running at the correct target pace during a race is not an insignificant consideration, especially at long distances like the marathon. If you run too fast, you risk depleting your capacity, running out of energy reserves, or, proverbially, "hitting the wall.” 

Failure to run at close to your potential on a race can result in a number of problems. If you underestimate, then you risk not getting as good of a time as you could. If you overestimate, you’ll end up depleted and maybe be unable to finish. 

For runners trying to hit their peak, having both the right prediction and running at a proper pace can be huge advantage going into your next race. 

## Marathon: A Comparison of Race Predictors, Calculators and Models

Before looking at how these models predict my race time, let’s briefly compare some of the most popular race predictors and models: 

**Riegel’s Formula**: This is one of the oldest formulas and was first published in the August 1977 issue of Runner's World. The idea is simple and purely mathematical. You take a shorter race time and then using a coefficient (Coef), which describes how you slow down at longer distances, you predict your race time at a longer distance. For example, using an online [Riegel Calculator](https://www.runningahead.com/tools/calculators/race), if you ran a 2:00:00 half marathon, Riegel’s Formula predicts a full marathon time of 4:13:42. 

{% img center /images/2017-resources/aschwanden-marathon-1.png %}

**Vickers-Vertosick Model Based On One Race**: This originally started as a critique of Riegel’s formula. They hypothesized that the Riegel model didn’t work as well as you increased distances. Vickers surveyed over 2000 runners online to come with a predictive model based on two factors: a previous race time and your weekly training mileage. The piece was originally published in Slate before being tweaked and republished in FiveThirtyFive as [Tell Us Two Things And We’ll Tell You How Fast You’d Run A Marathon](https://fivethirtyeight.com/features/tell-us-two-things-and-well-tell-you-how-fast-youd-run-a-marathon/). For example, using the [FiveThirtyFive Marathon Calculator](https://projects.fivethirtyeight.com/marathon-calculator/), if you race a previous half marathon at 2:00:00 and run about 20 miles per week, the model predicts a full marathon time of 4:29:41. 

**Vickers-Vertosick Model Based On Two Races**: If you add an additional data point in the form of a second race result, the predictive values become stronger. If you race a previous half marathon at 2:00:00, run about 20 miles per week and also did 10k at 00:51:00, the model predicts a full marathon time of 4:26:19. 

**Method for Vickers-Vertosick Model**: This model is based on a dataset of 2000 runners that was solicited online through a survey. Using that data, a logistic regression was used to come up with the predicted results and underlying formula. I’ve included a chart that visualizes these two models. 

**Runner’s World Race Time Predictors**: A few years ago Runner’s World updated their race time predictors. According to [article on the revision](https://www.runnersworld.com/marathon-training/heres-a-better-marathon-time-predictor), they admit that their old calculator was just wrong and that the new one is based on the "data-driven research” from Vickers. In view of this, their new predictor can take a variety of factors to predict a race time, including a single race, two races and also training volume. As you add more data, the prediction should become more accurate. 

**Runner’s World Race Time Predictor Based On One Race**: Using the [Runner's World calculator](https://www.runnersworld.com/tools/race-time-predictor), if you ran a 2:00:00 half marathon, your predicted marathon time is 4:10:12 which is similar to Riegel’s formula. 

**Runner’s World Race Time Predictor Based On Two Races**: If you ran a 2:00:00 half marathon and 10k at 00:51:00, your predicted marathon time would be 3:54:37.  That’s a variance of nearly 15minutes when you add in a 10k score. 

**Runner’s World Race Time Predictor Based On Two Races and Training Volume**:  If you race a previous half marathon at 2:00:00, run about 20 miles per week and also did 10k at 00:51:00, the model predicts a full marathon time of 4:26:19. In fact, this is the same result as Vickers-Vertosick Model since it’s the same model! 

**Race Predictor (Kosakowski) Based on a Single Race**: Kosakowski is Polish runner and researcher. As he writes in [The Mathematical Model of Race Time Predictor](http://lkosakowski.com/rtp/model/en/), various existing models “share...a common feature. While working well for elite runners' results, they collapse when it comes to the marathon at amateur level, producing seemingly unachievable results.” His approach is a mix of statistical methods and additional considerations about the limits of racing performance. Using results from 6200 runners at several marathons and half marathons in Poland, he created a new predictive model that, he claims, more accurately predicts performance of non-elite, recreation runners. Using his app “Race Time Predictor,” which is available on Apple, Android and Windows Phone, if you ran a half marathon at 2:00:00, then your predicted full marathon time is 4:27:51. 

## Summary of Race Predictors, Calculators and Models

Let’s compare these predict results from our example case: 

{% img center /images/2017-resources/race-predictions-sample-numbers.PNG %}

These models show a considerable amount of variance. The slowest prediction is nearly 4h30 and the fastest is 3h54. That’s a difference of 36 minutes!

As you add or change factors, the predictions change significantly too. So if you increase your training volume or improve your race times, the expected results change too. 

## Summary of My Predicted Marathon Race Times According to Multiple Models

Based on my last half marathon (1:45:00), a previous 5k (00:21:17), and my current training volume (51.1 km or 32 miles per week), I checked my race prediction through these different models. 

Here is a summary of my predictions: 

{% img center /images/2017-resources/race-predictions-mark-numbers-2017-chiangmai.PNG %}

All of these models predict that I should be able to run my next marathon at under 4 hours with the average target time of 3:52:59. 

There is variance of 3.12 minutes between the most optimistic model from FiveThirtyFive (b) and Kosakowski’s Race Predictor. I was slightly surprised on similar the results were from these predictors, especially in view of much variance I saw in the test cases. 

In view of the differences in how these predictive models work, it show that there is a point of convergence too. For example, Kosakowski’s race time predictor is based on a single race score, and yet it is within a few minutes of the more sophisticated model. 

## Conclusion: What My Strategy for My Next Marathon? 

In this post we looked at several race time prediction models. After comparing for a sample case, I was surprised to see how convergent this models were for my predicted time. With a variance of about 6 minutes between the models, it’s a pretty same assumption that they agree on my possible next race time at under 4 hours and possibly closer to 3:55. 

**So what’s my strategy and race plan for my next marathon?**

My next race is about a week away, and I’m hoping to complete my first marathon under 4 hours. My training has been good, and my last half marathon about a month ago (1:45:00) all point towards this as being a realistic target. 

Beyond these predictions, I obviously need to consider the environment too. Will it be hot and humid? How might those factors change my ability to run at peak potential? This is a topic outside of this post, but worth pondering in a later one. 

For my next upcoming race, I’ve set a couple of different goals. My conservative or “safe” goal is running under 4 hours. I just need to stay with that pace group. My more aggressive goal is 3:52, which is inline with my predictions as well. Finally, my middle-ground strategy will be running around 3:55. I think it’s a good idea to have a couple different goals when you approach a marathon since things change and it’s good to be honest during the race. 

In terms of strategy and pacing, research and data studies indicate that the way to run a your best half or full marathon is to run at an even pace.  So you should avoid starting too fast and finishing too slow as well as starting to conservative and slow and trying to run fast at the end. While shorter distance races might see variance in your first and second half splits, marathon are best run with an even or slightly negative split. 

Why does having a good prediction matter for marathon running? First off, properly predicting and running at your best possible target pace will lead to your best race times. Second it will help you avoid going too fast and hitting the wall or the opposite of too slow and missing your next PB. 

Hopefully these race predictors and calculators can help you run your next personal best! 

