# 202 - Monte Carlo: Death Star and Borg Cube Accident

Here we ask a simple question: what if the Death Star (from Star Wars) and the Borg Cube (from Star Trek) 
had a traffic accident? 

Exercise 1: Suppose the Borg Cube accidentally backed into the Death Star (partway!) and crushed in part of the 
volume following the shape of the Borg Cube. This means fewer sleeping spaces and offices(?) for 
Stormtroopers. Using a Monte Carlo method calculate the remaining volume after the accident.
Optionally include in the calculation the concave disk for the "Composite Beam Superlaser".
Try to visualize the output of the Monte Carlo.

![Death Star Borg Dent](../assets/death-star-borg-dent.png)

For the purposes of the exercise you can assume that the geometry of the collision was simple:

  * the Borg Cube sides $L_{BorgCube}$ are half the radius of the Death Star ($R_{DeathStar}$)
  * the collision axis is parallel to the equatorial plane of the Death Star
  * the bottom of the Borg Cube was 0.04 $R_{DeathStar}$ above the equatorial plane during the collision
  * the Borg Cube was centered on a plane that is (1) perpendicular to the equatorial plane of the Death Star and (2) runs through the center of the Death Star
  * the back side of the Borg Cube reached a distance 0.6 $R_{DeathStar}$ from the plane perpendicular to the equatorial plane and perpendicular to the collision axis

![Accident Diagram](../assets/Death-Star-Borg-Cube-Collision-Diagram.png)

Exercise 2: Some of you may be saying "Wait, you fool! The Borg Cube is larger than the Death Star!" I don't
actually know which is larger in the respective science fiction literature, but let's pretend... So let's now 
suppose that it was the Death Star that backed into the Borg Cube and left a spherical (Death Star) shaped 
crushed in dent. What is volume left within the cube for the Borg Collective to use?

![Borg Death Star Dent](../assets/borg-death-star-dent-0.png)
