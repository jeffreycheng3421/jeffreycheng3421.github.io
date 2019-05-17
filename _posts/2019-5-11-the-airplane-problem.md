---
layout: post
tags: [Probability, Monte Carlo, Project]
title: The Airplane Problem
---
Problem: one hundred people line up to board an airplane. Each has a boarding pass with assigned seat. However, the first person to board has lost his boarding pass and takes a random seat. After that, each person takes the assigned seat if it is unoccupied, and one of unoccupied seats at random otherwise. What is the probability that the last person to board gets to sit in his assigned seat? Problem found [here](https://www.math.ucdavis.edu/~gravner/MAT135A/resources/chpr.pdf). Answer is 1/2.

Simple intuition would guide one to believe that the answer is very small. For example, one specific example of a success is if the first person sits in their assigned seat. Then, everyone else sits in their assigned seat and the last person will sit in their assigned seat. However, the probability of this occuring is only 0.01. My guess was that integrating the probabilities of all the possible success would end up with a very low total probability.

This is incorrect. The problem can be solved through Monte Carlo, but after further thought and discussion with others (Anna Zhang) we came to a much more elegant solution:

We are presented with two scenarios: the problem will immediately end if a displaced person (including the first person!) randomly chooses the first person's seat or a displaced person randomly chooses the last person's seat. Because these two possibilities are equally likely at any point in the problem, the answer is 1/2.

It is clear that the solution remains the same for any n number of passengers, but it can be more rigorously proved by induction. I will not attempt to prove that here.

Monte Carlo Simulation linked [here](https://nbviewer.jupyter.org/github/jeffreycheng3421/jeffreycheng3421.github.io/blob/master/rpdfs/Airplane_Problem.pdf).
