# Threejs-VR-Hand-Input-Physics (broken, Oculus Quest Version 25 Update, some codes commented out, experimenting)

Explore physics simulations with Threejs VR hand input

[https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/](https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/)

## System Requirements

Oculus Quest.<br>

Oculus Browser >10.2 (Quest update >19.0 and threejs r119).<br>

"chrome://flags/#webxr" in Oculus Browser.<br>
"WebXR experiences with joints tracking" enabled.<br>
"WebXR experiences with hands tracking" disabled.<br>

## 1. Minimal Threejs VR Hand Input

<img src="images/1-threejs-vr-hand-input-physics.gif" width="320">

With an Oculus Quest, open Oculus Browser to link (and "Enter VR" with controller):<br>

[https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/threejs_vr_hand_input_physics.html](https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/threejs_vr_hand_input_physics.html)

(February 20, 2021.<br>
Oculus Quest (version>25) and WebXR (https://www.w3.org/TR/webxr-hand-input-1/) updates.<br>
"line trail[i].position.x = hand2.joints[XRHand.INDEX_PHALANX_TIP].position.x" not working and is commented out so no black screen and just display hands' joints.<br>
Experimenting with codes to see what is working.)<br>

Put controllers down, hold hands in front of headset until Quest recognizes them.

To exit simulation, use Oculus Quest left hand gesture of facing palm with index finger and thumb touching (or press left Touch controller menu button).<br>

The .html codes in Threejs-VR-Hand-Input-Physics use a subset of three.js r119 to start VR with joints tracking. Since it is experimental, it may break in future update of browser or threejs. ~~Also, a controller is needed to "Enter VR".~~ (Oculus Browser >12.0 update, now "Enter VR" with hands! No controllers required.) Nevertheless, it is fantastic that Oculus has WebXR joints tracking in its browser and three.js is making it accessible in its library.<br>

This example is not about physics except some kinematics. The right index finger plots 100 3D ticks. Assuming Oculus Quest 72Hz framerate (don't know sampling rate of joints tracking or time to determine joints' positions), time between each tick is ~13.9ms. The distance between two consecutive ticks is the distance the index finger moves in ~13.9ms. In the animated gif above, ticks are close together when finger accelerates (+/-) at peaks of sine wave and further apart between peaks.

The .html codes in Threejs-VR-Hand-Input-Physics are developed on a Raspberry Pi 3 Model B+ and tested with Oculus Quest. There is a short tutorial on writing three.js codes on a Raspberry Pi in "Making Threejs-WebXR-67P":

[https://github.com/Physicslibrary/Threejs-WebXR-67P](https://github.com/Physicslibrary/Threejs-WebXR-67P)

## 2. Threejs VR Hand Input Palm-Up Gesture

<img src="images/2-threejs-vr-hand-input-physics.gif" width="320">

An example of left palm-up to make a box visible (open a menus or change variables). The y-positions of two red cubes are used to compute a number when the palm is facing up.

[https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/2-threejs_vr_hand_input_physics.html](https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/2-threejs_vr_hand_input_physics.html)

## References

July 29, 2020 Threejs r119 added experimental Hand Input API support.<br>

https://github.com/mrdoob/three.js/releases/tag/r119

Oculus Browser >10.2 "chrome://flags" must be changed.<br>

https://github.com/marlon360/webxr-handtracking

Threejs VR hand input examples "vr / handinput" work in Oculus Browser:<br>

https://threejs.org/examples/

Threejs webxr_vr_handinput*.html codes to learn:

https://github.com/mrdoob/three.js/tree/dev/examples

July 23, 2020 Oculus added experimental WebXR Hand Input in Oculus Browser >10.2.<br>

https://twitter.com/fernandojsg/status/1286381837301022721

