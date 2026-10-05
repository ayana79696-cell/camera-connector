# Camera Connector

A lightweight prototype for connecting two Android phone cameras to a browser-based switcher using WebRTC.

## Prototype flow
1. Open **camera.html** on Camera 1 and Camera 2 phones.
2. Allow camera access and select the desired resolution.
3. Copy each phone's Connection ID.
4. Open **controller.html** on the control device.
5. Pair both cameras and switch the selected preview.

## Important next stage
The web switcher is the control/preview layer. Android Prism Live Studio does not automatically treat a browser video element as a camera source. The production version therefore needs a native Android output bridge (or another Prism-supported video input method) so the selected feed can actually appear inside Prism. This repository deliberately does not pretend that part is solved until it is tested on the target Android/Prism setup.
