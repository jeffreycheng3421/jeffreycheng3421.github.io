---
layout: post
tags: [Probability]
title: The Monty Hall Problem
---
Problem: Suppose you're on a game show, and you're given the choice of three doors: Behind one door is a car; behind the others, goats. You pick a door, say No. 1, and the host, who knows what's behind the doors, opens another door, say No. 3, which has a goat. He then says to you, "Do you want to pick door No. 2?" Is it to your advantage to switch your choice?

Although it may seem like the answer to the question is no (you have two doors and therefore the car is behind either your initial door or the other door, making the probability of the car being behind either door 0.5), the answer is actually yes. It took me a while to understand it and I couldn't really find a (subjectively intuitive) way of explaining it online, so I will attempt to explain it in my own terms below:

The choice that Monty is giving you is actually a choice between your original door and the 2 remaining doors, as if he had not opened any door at all! Lets think about this: the two doors you did not initially choose either contain a) a goat and a car or b) two goats. Monty opens a door and shows you a goat—but you already knew this! It was already known that one of the other two doors contained a goat (regardless of which door you first chose) so Monty effectively has not given you any new information: he has not opened a door at all. What he has done, however, is created a situation in which you picking the last door is effectively the same as picking both doors you did not choose initially. This means that you are effectively making a choice between one random door and two random doors, which give probabilities of 1/3 and 2/3 respectively. So the right answer is that you should switch.
