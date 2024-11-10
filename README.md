
<!--#echo json="package.json" key="name" underline="=" -->
shisen-sho-multiplayer
======================
<!--/#echo -->

<!--#echo json="package.json" key="description" -->
Placeholder project for a multiplayer variant of Shisen-sho aka Mahjong
Connect aka Four Rivers.
<!--/#echo -->


Today I discovered the [Shisen-sho game][wp-en-shisen-sho] and played
[the DKM games version](https://dkmgames.com/Shisen/shisenplay.htm) for a bit.
I had some ideas for a multiplayer version, so I made this repo to write
them up and share them. Maybe some day I might even find time to implement it,
maybe as a learning example for some new web UI framework.



Standard rules
--------------

* Your goal is to eliminate all mahjong tiles.
* Tiles can be eliminated if you find a pair that is either adjacent or
  can be connected by a line with at most 2 bends, i.e. max. 3 line segments.
* All line segments must align to the grid.
* Line segments along the borders are valid, i.e. there is a frame of empty
  tiles around the grid of mahjong tiles.



Multiplayer additions
----------------------

* Players take turns in eliminating tile pairs.
* Default scoring schema is one score point per pair found.
* When a player found a pair, they may continue, up to a configurable maximum
  streak length.
* Player turns can have a time limit.
  * Players can choose to take a penalty in exchange for extending their turn
    time limit, with limits on how often they can do so.







<!--#toc stop="scan" -->



Known issues
------------

* Vaporware: There is no implementation on the horizon.





&nbsp;


  [wp-en-shisen-sho]: https://en.wikipedia.org/wiki/Shisen-sho


License
-------
<!--#echo json="package.json" key=".license" -->
ISC
<!--/#echo -->
