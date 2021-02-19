A basic, but complete, 2D multi-user spatialized sound demo.

Codepen, so developers can easily see how it is done. Target 500 lines of pure javascript, TOTAL, with no frameworks or server code.

Everything is drag and drop:
- Drag your dot to move.
- Drag on an mp3 to play it from that position, and anyone can drag it around afterwords. Gets deleted when you leave. (Opens a second connection to the mixer.)
- Drag an image to be the background (for everyone).
-  Drag an image onto yourself or any music to be the image. 
- ~~Twist/arrows to change your direction.~~

Start in anteroom/lobby, showing how many in each room. Join the one you want.

Because there is no server, there are no accounts. Get assigned a name for the duration ~~(and for several minutes after leaving). Expired names re-join the pool~~.

Because everyone is anonymous, you cannot speak for your first 5 seconds in a room. Beginning several seconds after you do speak in a room, you can kick out anyone in that room. You get kicked to the lobby (where there is no speaking), and you can rejoin the room, but beware that people can kick you before you have a chance to disrupt.

I don't want people to guess as to what is happening on the server, without being able to see the source, and I don't want the hassle of running a server. So I'm using Croquet to have replicated behavior without a server.

Ideas for further work, in addition to the ~~not-implemented~~ above:
- Bug: something wrong with initial audio positioning until drag.
- Bug: something wrong with behavior when tab is not closed, but goes to sleep
- Important Feature: Mute!
- Too easy to click instead of drag, bringing up file picker. Maybe instead have have a context menu by right-mouse/touch-hold?
- QR code to share the "full screen" view with someone. But who is face2face any more?
- Video: select a person to show their video. Select anyone who is sharing, but only one shown at a time to imit "Zoom fatigue".
- zoom or limit travels? (relates to mobile screen size issues)
- persist your color/name for several minutes, so that people will recognize you after you refresh.
- persist your avatar image (indefinitely?), but then how do you remove it?
- I'd like to highlight map and your own avatar as drop targets, depending on what is being dragged. But the dragleave fires on all subelements.
