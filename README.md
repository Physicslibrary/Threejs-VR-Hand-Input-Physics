# Threejs-VR-Hand-Input-Physics
Explore physics simulations with Threejs VR hand input

## System Requirements

Oculus Quest.<br>

Oculus Browser >10.2 (Quest update >19.0 and threejs r119).<br>

"chrome://flags/#webxr-hands" in Oculus Browser.<br>
"WebXR experiences with joints tracking" enabled.<br>
"WebXR experiences with hands tracking" disabled.<br>

## 1. Minimal Threejs VR Hand Input

<img src="images/1-threejs-vr-hand-input-physics.gif" width="320">

With an Oculus Quest, open Oculus Browser to link (and "Enter VR" with controller):<br>

[https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/threejs_vr_hand_input_physics.html](https://physicslibrary.github.io/Threejs-VR-Hand-Input-Physics/examples/threejs_vr_hand_input_physics.html)

To exit simulation, use Oculus Quest right hand gesture of facing palm with index finger and thumb touching (or press left Touch controller menu button).


Files (except .html) in /build and /examples are from threejs r119. These are minimal files to start VR with joints tracking. Since it is experimental in Oculus Browser, it may break in future update of browser or threejs. Currently, a controller is needed to "Enter VR". Nevertheless, it is fantastic that Oculus has WebXR joints tracking in its browser and three.js in its library.<br>

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

