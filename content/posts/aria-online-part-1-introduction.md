---
title: "Aria Online Devblog: Part 1 - Introduction"
date: 2020-01-01
ShowShareButtons: true
---

# Introduction

Over the course of the past few months (the project's first commit was on september 29nth, 2023), I have been hard at work on a "little" side project that I hope to be able to publish one day, an MMORPG.
Although still in development and lacking a lot of features, I've gained a lot of knowledges that I would like to share.

In my research, I've observed a challenge: finding resources that explain how MMORPGs work in-depth is not easy. Articles and devblogs often stay surface-level, focusing on a single server with limited details on deployment or overly emphasizing client-side logic. The common belief that "making an MMO is the hardest thing in gamedev" is, in my opinion, partly due to the lack of comprehensive documentation on this topic. Through this devblog, my intention is to thoroughly explore this realm, encompassing topics such as CI/CD, network protocols, Kubernetes, and the creation of external tools like a spell editor. The objective is to establish a robust foundation for aspiring MMORPG developers.

# The Game

> Aria Online is a PvP MMORPG where you step into the shoes of a soldier engaged in the ongoing war between three factions. Action is at your fingertips the moment you log in, with no sharding or multiple servers (except maybe one per continent). Every character coexists in the same shared world.

Before delving deeper, let's discuss the game and establish some expectations regarding its scope.

When conceptualizing the game, I imagine a PvP-centric adventure that minimizes or completely discards traditional leveling mechanics, placing a significant emphasis on enhancing equipment. The goal is to create an easily approachable game while providing a more challenging learning curve for those aiming for mastery. The current plan is to maintain a single server for the entire world, though this approach may undergo adjustments based on the practicality of resolving severe latency issues—potentially leading to a compromise of one server per continent at the most extreme.

Here are some of my inspirations for the game:

- PvP / Realm vs Realm: Guild Wars 2, Foxhole, Dark Age Of Camelot, PlanetSide 2
- Equipment / No classes: New World and Albion Online

# What I will cover

In the upcoming articles, I plan to extensively cover all the topics I've touched upon, ranging from game design to the deployment of my server fleet. Here's a sneak peek into the topics I plan to delve into:

- Client architecture (Godot)
- Game server architecture (C#, ECS)
- API architecture (NestJS, PostgreSQL)
- How can a fleet of servers share the world simulation without conflicts
- Creating tools to make my life easier (The Inspector)
- Creating spells and abilities without writing a single line of code
- Continuous Integration (CI) / Continuous delivery (CD) (Github actions, automated versioning, automated Steam deployment)
- Deployment of every components (Gameserver, API, detabase, etc.) on a Kubernetes cluster
- Lag composentation
- Managing different enviroments (production, staging, etc.)

# Conclusion

Feel free to join me on this journey and stay tuned for the upcoming chapters, follow me on LinkedIn to be notified when the next article is published.
