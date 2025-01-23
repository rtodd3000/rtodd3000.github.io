---
layout: project
type: project
image: img/png-clipart-king-of-spade-playing-card-king-of-spades-playing-card-suit-jack-queen-miscellaneous-game-thumbnail.png
title: "Cards"
date: 2023
published: true
labels:
  - Java
summary: "My group designed an interactive, turn-based spoons card game for my Java college course."
---

For a project in my Java programming class, me and two of my friends made a console game in VScode based on the card game called Spoons. This game would run until all of the spoons were taken and someone loses. It was a project that was a big part of my grade and took many sleepless nights to complete due to the unqiue algorithm of the game.

For this project, I worked a lot on the deck and card classes while me and my two other group members worked on the game class together. My main prority was to just get the algorithm of the game to work, specifically this part of the loop running the game:

//if a spoon has already been taken, the players who don't have one will be given a 33% chance to get one
            else if (nSpoons < (players.length - 1)){
                for (Player curPlayer : this.players){
                    if (curPlayer.hasSpoon() != true){
                        int randChance = randy.nextInt(3);
                        if (randChance == 0){
                            curPlayer.stealSpoon();
                        }
                    }
                }
                //checks if a loser has been found
                if (loser != 0) {
                    break;
It took many attempts and a lot of use of ChatGPT, but eventually I was able to solve the issue and get this part of the code running.

Before making this project, I had no idea what the spoons game was. Unfortunately, this made the process of making the game a bit harder since me and my teammates had to research and learn how to play spoons, but once we got it down, everything else came into play. Initializing all the classes for the deck, dealer, cards, etc. was simple and did not take that long for us to do, however the implementation for the game class was very tricky and it took us a lot of trial and error until we were able to get it running. Basically, this project taught me a lot about trial and error until your code likes you and starts running. 
