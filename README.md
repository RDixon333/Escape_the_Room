# Escape_the_Room

To keep myself from overcommitting to something I don't yet have the full grasp of, I've decided to make my project a little "Escape the Room" game. It would utilize my own internal database of virtual items.

The idea is that you are stuck in a room and need to escape. This will utilize HTML tables as the front end, and Javascript working in the backend, managing the state of interactive objects. There will be 4 interactive objects in the "room": a refrigerator, drawer, cabinet, and the locked door. You can click on objects, and they will change state, and/or return a message.

Javascript will do most of the heavy lifting, while HTML and a small bit of CSS will make it somewhat appealing to look at.

[UPDATE 6/12/18]

As of yet, a portion of game's most basic functionality is there, albeit with some caveats.

You're able to click on objects and a "collision detection system" will spit out an alert for the object you clicked on. Multiple tables of these colliders are placed above a background image which is centered on the page. A click event listener determines this by the ID of the given element (i.e. cabinet, fridge, etc.).  All works as intended... mostly.

Now for the caveats. The colliders only position themselves correctly on the page if you're running a maximized window on Chrome at a resolution of 1920x1080. A bit of research indicates that HTML tables are not inline objects, so they do not behave correctly even when "tamed" with CSS. Even Flash games from 2005 don't have this level of janky implementation, so this simply will not do.

The table placement issue still occurs even when spliting the background into its separate objects, and distributing them within the table. What to do?

Well, the simple solution to this is to just use a javascript-based game engine to do everything, including displaying the objects. Fortunately, I've found some promising ones that I'll be playing around with this week.
