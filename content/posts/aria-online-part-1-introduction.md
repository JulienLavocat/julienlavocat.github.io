---
title: "Aria Online Devblog: Part 1 - Introduction"
date: 2020-01-01
draft: false
ShowShareButtons: true
---

[THIS IS A DRAFT, I ADVISE YOU TO COME BACK LATER, FOLLOW ME ON LIKEDIN TO KNOW WHEN IT'S READY]

# Introduction

During my research I've noticed that it's hard to come accors resources explaining how an actual MMORPG works. When you find an article or a devblog often the content is quite shallow and doesn't go beyond a single server and sparse details about it's deployment or most of the logic is client-sided. I believe that if people often says "making and MMO is the hardest thing in gamedev" it's partially due to the lack of in-depth documentation around this topic.  
With this devblog, I'd like to be able to go deeper into the rabbithole and provide some strong bases for the next person that will want to develop such games.

## Disclaimer

I'm not a game developer, I'm a fullstack software developer mainly working with Angular and NestJS but I will bring what I know about software engineering and try to apply as much as I can to the game, mainly around CI/CD and deployment.  
Don't expect to see some crazy graphics or artworks, also you shouldn't expect me to nail the game design on my first try.

# The Game

Before going any futher, let's talk a bit about the game and set some expectations about it's scope.  
When I think about the game I imagine something PvP-focused with a very-short / no leveling at all (mostly improving your equipment) and relatively easy to pickup but harder to master and only one server per continent.  
Here is list of some games that inspired me :

- **PvP / Realm vs Realm**: Guild Wars 2 and PlanetSide 2
- **Equipment / No classes**: New World and Albion Online

And here is a little pitch about the game :

Aria Online is a PvP MMORPG in which you won't be a hero but a mere soldier fighting the war between 3 factions, you will be able to jump into the action as soon as you're online. There will be no sharding nor multiple servers (except maybe one per continent as I'm not sure if I would be able to tackle such extreme latency issues), every character will exists in the same world.

As I said before, I'm neither a game developer not an artist so you won't see some crazy beatiful arts here but I will try to do my best :D Worst, I'm working on this alone.

# What I will cover

In future chapters, I will try to cover as much as I can everything I did, from the game design to how I choose to deploy my fleet of servers. Here are some examples of such topics :

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

I hope to have picked your curiosity, feel free to follow me to see the next chapter of this adventure :)
