# Root Motion NavMeshAgents

In this tutorial repository and [associated video](https://youtu.be/uAGjKxH4sDQ) you will learn how to combine a Root Motion animated model with a NavMeshAgent. 
This gives you all the pathing benefits and local avoidance of the Navigation System with the precise animation you expect from Root Motion.

There are multiple ways to approach this solution. In this repository I have chosen what makes the most sense to me - correcting the position of the Root Motion to pathable areas by moving the position of the model back towards the NavMeshAgent when they are out of sync. 
An alternative that I did not have much success with was to move the Agent faster towards the model's root motion position.

[![Youtube Tutorial](./Video%20Screenshot.jpg)](https://youtu.be/uAGjKxH4sDQ)

## Patreon Supporters
Have you been getting value out of these tutorials? Do you believe in LlamAcademy's mission of helping everyone make their game dev dream become a reality? Consider becoming a Patreon supporter and get your name added to this list, as well as other cool perks.
Head over to https://patreon.com/llamacademy to show your support.

### Phenomenal Supporter Tier
* Andrew Bowen
* YOUR NAME HERE!

### Tremendous Supporter Tier
* YOUR NAME HERE!

### Awesome Supporter Tier
* Gerald Anderson
* AudemKay
* Matt Parkin
* Ivan
* Paul Berry
* Reulan
* YOUR NAME HERE!

### Supporters
* Bastian
* Trey Briggs
* Matt Sponholz
* Dr Bash
* Tarik
* YOUR NAME HERE!

## Other Projects
Interested in other AI Topics in Unity, or other tutorials on Unity in general? 

* [Check out the LlamAcademy YouTube Channel](https://youtube.com/c/LlamAcademy)!
* [Check out the LlamAcademy GitHub for more projects](https://github.com/llamacademy)

## Socials
* [YouTube](https://youtube.com/c/LlamAcademy)
* [Facebook](https://facebook.com/LlamAcademyOfficial)
* [TikTok](https://www.tiktok.com/@llamacademy)
* [Twitter](https://twitter.com/TheLlamAcademy)
* [Instagram](https://www.instagram.com/llamacademy/)
* [Reddit](https://www.reddit.com/user/LlamAcademyOfficial)

## Requirements
* Requires Unity 2020.3 LTS or higher.
* [Navigation Components](https://docs.unity3d.com/Manual/NavMesh-BuildingComponents.html)
* I'm using [Infinity PBR's Gargoyle](https://assetstore.unity.com/packages/3d/characters/creatures/gargoyles-fantasy-rpg-37416?aid=1101l9QvC) but this can be replaced with any root motion animated model (such as "The Dude", which is included in this repository as the "enemy"). 
	* If you're using "The Dude" model for the player, be sure to update the Animator paramters to set `"velx"` `"vely"` to the `Velocity.x` & `Velocity.y` respectively as is done in `EnemyMovement.cs`
