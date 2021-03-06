# Tank-Track-Simulator
 This Unity asset simulates the track movement of a tank.
 
 ![image](https://github.com/swordmaster003/Tank-Track-Simulator/blob/master/Screenshots/Cover.png)
 
 ## Download

You can download this asset from Unity Asset Store:

[Tank Track Simulator](https://assetstore.unity.com/packages/tools/physics/tank-track-simulator-99013)
 
## Online Documents:

[Tank Track Simulator Manual](https://www.swordmaster.info/unity-asset-documents__trashed/tank-track-simulator-manual-document/)

[Binding Bones To Tank Tracks Guide](https://www.swordmaster.info/documents/unity-assets-documents/binding-tank-track-bones-in-3ds-max-instruction%e2%80%8b/)
 
 ## Features:

- Higly simulates the track movement of a tank.

- This package contains the M1A2 tank model which has been binded bones to track's skinmesh.

- The editor of this system is very friendly,and you will set up your tank easyly and quickly.

- There are two documentations In this package :

  (1) The documentation which name is Binding Bones To Tank Tracks Guide will teach you to bind bones to your own tank'tracks in 3ds max       software,in order to make your model could be used by the Final Tank Track Simulator;

  (2) The documentation which named Tank Track Simulator Manual will teach you how to set up your tank's tracks by using the Final       Tank Track Simulator .

## The technology behind this package :

Each wheel collider of tank generates the displacement relative to tank’s vertical direction, then we record each wheel collider’s current position, assigning this position information to its corresponding wheel model and wheel bone,that is to say, each wheel model’s position and wheel bone’s position are always the same as their corresponding wheel collider’s position.

![image](https://github.com/swordmaster003/Tank-Track-Simulator/blob/master/Screenshots/1.png)

Besides,the track's skinmesh is binded with wheel bones,when a wheel bone generates displacement relative to tank’s vertical direction, corresponding part of the skin which effected by this wheel bone will generate deformation .

![image](https://github.com/swordmaster003/Tank-Track-Simulator/blob/master/Screenshots/2.png)

As far as the rotation of wheel model, we calculate wheel colliders’ average rotation speed on one side of the tank,and applied this rotation speed to each wheel model’s rotation on this side of the tank.

![image](https://github.com/swordmaster003/Tank-Track-Simulator/blob/master/Screenshots/3.png)
