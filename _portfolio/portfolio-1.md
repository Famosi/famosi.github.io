---
title: "Duckietown - AI Driving Olympics"
excerpt: "The AI Driving Olympics (AI-DO) is a competition with the objective of evaluating the state of the art in machine learning and artificial intelligence for mobile robotics. The goal of the competition is to build a machine learning (ML) model that allows a self-driving car, called Duckiebot, to drive on streets within Duckietown. <br/>

<img src='Duckietown-logo.png'>"

collection: portfolio
---

The [“AI Driving Olympics” (AI-DO)](http://aido.duckietown.org/) is a competition with the objective of 
evaluating the state of the art in machine learning and artificial intelligence for mobile robotics.
The goal of the competition is to build a machine learning (ML) model that allows a self-driving "car", called `Duckiebot`, to drive on streets within `Duckietown`.

The AI Driving Olympics competition is structured into the following separate challenges:
* Lane Following - `LF` 
* Lane Following with Vehicles - `LFV`
* Lane following with Vehicles and Intersections- `LFVI`
* Autonomous Mobility-on-Demand - `AMoD`

This project is a solution for the `aido-LF` challenge: 
* **Control of a Duckiebot to drive on the right lane on streets within Duckietown without other moving Duckiebots present.**

More info about the Duckietown Project and `aido-LF` challenge [here](http://aido.duckietown.org/).

## Description

The approach is to train a Reinforcement Learning (RL) agent to build an `expert` that drives 
perfectly within an environment, then use this `expert` to collect data. 
Data are pairs `<observation, actions>`collected in different maps/environments used to train an agent that imitates the expert's behaviour (Imitation Learning / Behavioural Cloning) .
Finally, you have a self-driving car that navigates within Duckietown using only one single sensor, the camera.

Trough this tutorial you will:
* Use the [Reinforcement Learning](duckietown_rl) approach (Decision Tree) to build an `expert`.
* Use the `expert` to [collect data](duckietown_il/collect_data.py).
* Use the [Imitation Learning](duckietown_il) approach to train the `Duckiebot`.
* [Submit](submission) the solution to the [“AI Driving Olympics” (AI-DO)](http://aido.duckietown.org/).

## Author
* **[Simone Faggi](https://github.com/FaMoSi)**
* Email: **simone.faggi@yahoo.it**




