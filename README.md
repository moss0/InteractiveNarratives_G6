# Interactive Narratives

FGCT4007

Richard Mann

2317919

Group 6

<br>

GitHub repository link: https://github.com/moss0/InteractiveNarratives_G6

Itch.io link: https://moss-0.itch.io/interactive-narratives-project

## Development

### GitHub

Throughout the course of this project I encountered many problems including out of date branches and merge conflicts. 
I asked everyone to create their own branches where they can work, and once finished, create a pull request to merge into the main branch. However, I was unaware on how to update branches at the time and people's branches were becoming increasingly out of date. I solved this problem by researching branches and understood merging properly, all I had to do was press 'update from main' every once in a while on everyone's branches and push. I am still not sure if updating from main while someone is working could cause them to lose work but I am choosing to play it safe and asking beforehand.
Merge conficts were common, as we did not communicate much, so I had to regularly try my best to ensure someone was not losing their work. I think I did an good enough job in this area.

### Third person shooting

I started off with the third person aim and shoot mechanics, deciding to make an aiming mode upon holding down Secondary fire (right mouse button.)

I learned that doing this in Event tick was not the proper way to implement this feature as it will cause performance problems when the project scales up in size. I decided to use a looping timer connected to an event that gets unpaused and paused upon pressing and releasing the mouse, respectively.

### AI NPCs

I decided to migrate my previous AI from the Client brief project in order to improve old code and add new features to save time.

#### Patrolling
Initially the increment code was kept inside of BP_PatrolRoute until I realised it does not support multiple NPC's using the same patrol route. I decided to move the code to within BP_NPC_Base so that way every NPC using the route has its own count of what spline index it is at, what direction along the spline to move, etc.

#### Senses

The AI NPC can sense the player through its AI controller. It loops through each actor percieved by the NPC and checks to see if it is the player and if the player has been misbehaving, in a restricted area determined by the disguise checker.

### Collectable system

This was the first time I used inheritance for a Blueprint. I watched a helpful [video](https://www.youtube.com/watch?v=k92eaGP4pss) which helped me to understand it properly. I made a base collectable that has child Blueprints for the disguise kit and money collectables. The 

### UI

I created a base button and base text box in order to have reusable widgets that can be changed universally across all instances. I tried to use inheritance with the button and text but it was behaving strangely, however, this was before I properly understood inheritance so it can be attributed to a lack of knowledge.


## Bibliography

Blueprint Interfaces | Unreal Engine 5 Tutorial (2023) At: https://www.youtube.com/watch?v=wGmlKbllPcw (Accessed  23/05/2025).
Components In Unreal Engine | UE5 Tutorial (2025) At: https://www.youtube.com/watch?v=h-kNZdshNSU (Accessed  23/05/2025).
How to create Modular and Scalable UI systems in Unreal Engine (2023a) At: https://www.youtube.com/watch?v=v9k-J2GeEKI (Accessed  16/05/2025).
How to create Modular and Scalable UI systems in Unreal Engine (2023b) At: https://www.youtube.com/watch?v=v9k-J2GeEKI (Accessed  23/05/2025).
Inheritance Tutorial (Parent Child) | Unreal Engine 5 (2023) At: https://www.youtube.com/watch?v=k92eaGP4pss (Accessed  23/05/2025).
Interaction System in 15 minutes | Unreal Engine 5 tutorial (2023) At: https://www.youtube.com/watch?v=xH2Wlr2RNhw (Accessed  23/05/2025).
Smart Enemy AI |  (Part 3: Perception) | Tutorial in Unreal Engine 5 (UE5) (2023) At: https://www.youtube.com/watch?v=gsyZdKYAT_4 (Accessed  23/05/2025).
Smart Enemy AI | (Part 1: Behavior Trees) | Tutorial in Unreal Engine 5 (UE5) (2023) At: https://www.youtube.com/watch?v=-t3PbGRazKg (Accessed  23/05/2025).
Smart Enemy AI | (Part 2: Patrolling & States) | Tutorial in Unreal Engine 5 (UE5) (2023) At: https://www.youtube.com/watch?v=WFV5IewGks8 (Accessed  23/05/2025).

## Declared Assets

Assetville pack At: https://assetsville.com/assetsville-town/ (Accessed  23/05/2025)

## Outcome and future prospects

I definitely could have done more this project, especially regarding the dialogue system and my overall communication skills. I tend to find myself repelled from speaking with the others and prefer to work in the background by myself, however, I know that this must change in order for me to be a successful group member. On the other hand, communication was overall amiss amongst all of the group members which caused me to be stressed.
The goals we had set were unrealistic, I feel, and I felt as though I was working alone even though I was a part of the group.

In the future, I would structure my branches differently, instead of making a branch for each individual person, I would make less branches that would each have specific purposes in mind.

If I was given more time to work on this project, I would add more to the dialogue system and have labels above the disguise boxes so you can tell that they are interactable. More interactive elements would also be added, like a code to the vault and some idle NPC's at the reception, for example.
