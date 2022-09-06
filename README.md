# Simulation for Disaster System

###### Motivation

The Rescue Simulation is based on concepts of the RoboCup, anannual international robotics competition proposed and founded in 1996 by a group of university professors. The German University in Cairo has been taking part in this competition for few years and won various titles including the best team. The aim of rescue simulations is to derive strategies and behaviors for maximizing the number of saved lives and minimizing the number of casualties. The hope is that one day these strategies can be applied by actual policemen, firefighters and medics in real life disasters and accidents.

###### Simulation Game Rules

The game consists of a main simulation 10x10 grid where the whole map is taking place.
The game is a single player one, where the player is responsible for managing the rescue units to handle buildings and citizens suffering from the disasters that ensue during gameplay throughout the whole map. The main goal of the game is for the player to efficiently employ the rescue units to rescue as many citizens and minimize the number of deaths. All the available rescue units are assigned to the player at the start of the simulation. As the game proceeds certain disasters start appearing throughout the map affecting different buildings and citizens.

###### Winning Conditions

The game ends when all the planned disasters are either handled by rescuing the targeted citizens or failing to do so, thus the death of these citizens. When all citizens are either rescued or deceased the simulation game ends and the score of saves and losses is presented to the player.

###### Time Representation 
The game is cycle based meaning that time is represented as cycles passing within the simulation. Each rescue task takes a specific number of cycles and each disaster reaches its full effect in a specific number of cycles. The player controls the progression of the cycles.

