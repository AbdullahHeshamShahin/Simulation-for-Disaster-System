# Simulation for Disaster System

###### Motivation

The Rescue Simulation is based on concepts of the RoboCup, anannual international robotics competition proposed and founded in 1996 by a group of university professors. The German University in Cairo has been taking part in this competition for few years and won various titles including the best team. The aim of rescue simulations is to derive strategies and behaviors for maximizing the number of saved lives and minimizing the number of casualties. The hope is that one day these strategies can be applied by actual policemen, firefighters and medics in real life disasters and accidents.

###### Simulation Game Rules

The game consists of a main simulation 10x10 grid where the whole map is taking place.
The game is a single player one, where the player is responsible for managing the rescue units to handle buildings and citizens suffering from the disasters that ensue during gameplay throughout the whole map. The main goal of the game is for the player to efficiently employ the rescue units to rescue as many citizens and minimize the number of deaths. All the available rescue units are assigned to the player at the start of the simulation. As the game proceeds certain disasters start appearing throughout the map affecting different buildings and citizens.

<img width="1275" alt="Screen Shot 2022-09-06 at 10 41 57 AM" src="https://user-images.githubusercontent.com/64377604/188604856-2b9fe485-a329-4c64-a2a7-b18382a1d331.png">


###### Time Representation 
The game is cycle based meaning that time is represented as cycles passing within the simulation. Each rescue task takes a specific number of cycles and each disaster reaches its full effect in a specific number of cycles. The player controls the progression of the cycles.

<img width="1275" alt="Screen Shot 2022-09-06 at 12 39 10 PM" src="https://user-images.githubusercontent.com/64377604/188615385-62cea991-8197-4dc8-b0fd-81fadeccf064.png">

###### Simulation Components

There are different components in the game, each with special abilities, weaknesses, and goals. The game has a grid-based map representing the area covered in the rescue simulation. The map is occupied by buildings and citizens residing in said buildings. There are different disasters that can affect both buildings and citizens in different ways. Accordingly, there are different rescue units to be controlled by the player to handle said disasters.

###### Buildings
Buildings have citizen occupants. Each building has its own address i.e. locations on the map, that is different from the other buildings. At any given cycle in the simulation, a building can suffer from a disaster. This is why building disasters need rescue units to tend to the building itself and in some cases its citizens as well. Buildings have structural integrities representing the status of the building. The damage caused by fire disasters and the foundation damage caused by collapse, decreases the structural integrity of a building.

###### Citizens
Citizens are the people occupying the map. They can be located anywhere in the map including any of the residential buildings . Each citizen has health points (hp) indicating the current health. Citizens also have blood loss, toxicity indicators which are affected by being in a disaster. Citizens have different states that indicate the status of the current simulation scenario. At any given cycle in the game a citizen can either be safe i.e. not suffering from any disasters, in trouble which means a disaster is currently directly affecting this citizen, rescued from the disaster or deceased due to said disaster.

###### Disasters

There are different types of disasters that can occur throughout the game. Some of them affect buildings while others directly affect the citizens in the map. Buildings can 
1) catch fire.
2) collapse.
3) have a gas leak.
4) get infected.
5) injured.


###### Emergency Units

1) Gas Unit.
2) Medical Units.
3) Fire Units.
4) Disaster Units.
5) Evacuator.

<img width="1275" alt="Screen Shot 2022-09-06 at 12 40 42 PM" src="https://user-images.githubusercontent.com/64377604/188615445-9cd7668c-c1da-4699-a170-106e2f0257ac.png">



## Game Controllers 

You can select any Emergency Unit from the Right handside and put it on the targeted Disaster 
You can play next cycle by klicking over the controller button in the bottom left corner 


## Winning Conditions

The game ends when all the planned disasters are either handled by rescuing the targeted citizens or failing to do so, thus the death of these citizens. When all citizens are either rescued or deceased the simulation game ends and the score of saves and losses is presented to the player.

