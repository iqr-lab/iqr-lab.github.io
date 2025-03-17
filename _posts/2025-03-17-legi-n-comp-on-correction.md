---
title: Effects of Robot Competency and Motion Legibility on Human Correction Feedback (HRI 2025)
tags:
  # - conference
  # - interactive robot learning
  # - learning from corrections
  # - kinesthetic teaching
authors:
  # - Shuangge Wang
  # - Anjiabei Wang
  # - Sofiya Goncharova
  # - Brian Scassellati
  # - Tesca Fitzgerald
---


Imagine a scenario where a robot is deployed in a household to pack up a box. Since there are unseen scenarios such as new shapes of the box or new items the robot has never seen before, the robot will inevitably fail at deployment. One way the robot can learn from their mistakes is through learning from corrections from humans as supervisors. This way the robot can learn directly from the mistakes without requiring large amounts of feedback while still maintaining its autonomy.
Prior work has studied how to learn from human feedback when humans act as teachers or supervisors, and how certain feedback such as demonstrations are given. However, there is a gap in understanding how correction feedback is given which is the focus of our work.
Why is it important to study how humans supervise robots? Being able to understand how corrections are given will help interaction designers design better ways to obtain good quality feedback, and for learning researchers it will help robots learn more efficiently with realistic human data, even if it is less ideal.
From prior work there are three assumptions on human feedback:
A1: people give corrections based on the divergence from success.
Here is an example - if a robot is carrying out a wrong trajectory, in the beginning the robot is likely to go to either goal so the divergence between success and failure is small and it is less likely for the human to give a correction; as the robot carries on it becomes more obvious that the robot is going to fail so it is more likely for the human to give a correction.
A2: Humans can (generally) predict if corrections are needed
In general humans are able to tell if the robot is going to succeed or fail and give corrections accordingly. However, humans are not perfect, so they might miss giving a correction or give a wrong correction.
A3: there is a tradeoff between task and effort. The task here could be task accuracy or other measurement, and the effort could be physical or mental. Here is an example of a human putting in more effort for a more stringent correction so the robot will end up precisely near the goal; while here the human puts in less effort for a more relaxed correction and it is less clear where the goal is for the robot.
Are these assumptions true? or…are there other factors that influence how people give corrections?
From prior work, we expect two robot behaviors competency and legibility to affect trust, which affects human feedback.
A robot with higher competency is more likely to succeed while one with lower competency is more likely to fail; legibility describes how clear the robot is able to express its intent - If the robot is going to goal A the trajectory above is more exaggerated so it is more legible than the one below. Here is a more legible trajectory that is more exaggerated; a more predictable trajectory that is more direct and short; and an illegible trajectory that is more misleading and confusing.
So considering the two factors, are the assumptions true?
To answer the question, we designed our study which is a long horizon pick-and-place task. Here is an example of the task where the human teacher gives corrections to the robot when needed. It is a between subject study. We have 6 conditions with 3 levels of legibility and 2 levels of competency. We had 60 participants divided into 10 participants for each condition, which led to in total almost 4000 trials and almost 2000 given corrections.
We want to study the effect of robot competency and legibility on human correction feedback and how they align with the three assumptions.
Here is our result
A1: prior trust based literature suggested that higher competence from the robot induces higher trust from humans so we expect that the human to give corrections closer to the mistakes) Is this true
Guess what, NO! 
People correct competent robots further from the mistakes than incompetent robots (except when the robot is being illegible)
Our intuition: humans’ expectation is high for competent robots, so they are less accepting.

A2: prior trust based literature suggested that higher competence from the robot induces higher trust from humans so we expect humans to overpredict success. When supervising incompetent robots, do people tend to over-correct?
Guess what, NO! 
People under-correct incompetent robots; people over-correct competent robots
Intuition: Lower competency leads to lower expectation, so humans don’t care as much, while higher comp leads to higher expectation, so humans are demanding. 

A3: There is a tradeoff between task and effort. 
Guess what? YES!
There IS a trade-off between task and effort, but its strength depends on competency and legibility conditions

Based on our findings, the prior assumptions on human feedback don’t necessarily hold when we are looking at various conditions for corrections. We also have cool implications for designers and learning researchers in our paper. Please check out our paper if you are interested!
