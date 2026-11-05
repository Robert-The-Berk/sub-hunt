# Sub Hunt

A turn-based submarine hunt on a 40×26 sonar plotting table. An enemy sub is stalking a friendly convoy on its way west to the escape line; find it with active pings and passive sonobuoys, sink it with depth charges, and keep the convoy afloat.

Open `index.html` in a browser to play. No build step.

## Sensors
- **Active buoys** (6): drop one and it pings every turn for 4 turns. A ping returns a range ring only if the sub is within 10 nmi, and only as often as the sub's size allows.
- **Counter-detection**: the sub hears pings out to 24 nmi, much further than you can hear its echo. When it does, it sprints and steers to stay out of that buoy's range, so lay active buoys where it has to go.
- **Passive buoys** (8): silent, report a bearing up to 16 nmi. Fast subs are loud; slow subs are quiet.

## Sonar waterfall
The waterfall shows what one passive buoy hears: bearing across, time going down, newest at the top. Pick the buoy from the tabs. Convoy ships, torpedoes and whales all leave traces, and white ticks mark the friendly bearings. The sub's trace appears even when it is too faint for a logged contact, so a weak line holding a steady bearing is worth acting on. Hover to read a bearing, and click to plot it on the map.

## Plot pencil
Press **4** or pick **Plot** to mark up the table yourself. It's free and doesn't use a turn. Click a square to drop a guess mark labelled with the current turn, and click it again to erase it. Drag to draw a course line with an arrowhead. **Undo** and **Clear plot** tidy up. Bearings plotted from the waterfall use the same pencil colour, and the replay shows your plot alongside the sub's real track.

## Replay
When a hunt ends, **Watch replay** plays it back turn by turn: the sub's course, every buoy drop, ping return, bearing, torpedo and depth charge, with that turn's events underneath. Scrub with the slider or pause.

## The convoy
Four friendly merchant ships sail east along a marked route. The sub closes to within 8 nmi and fires torpedoes. Each launch is loud: the targeted ship reports a bearing, buoys hear it more easily, and the torpedo's run is shown, so you get one turn to answer. A sub that was just pinged or charged fires less often. You can't drop a depth charge on top of a friendly ship.

You have 6 active buoys, 8 passive buoys and 6 depth charges. You lose if every ship is sunk, if you run out of charges, or if the sub crosses the escape line. The Red October mission has no convoy.

## Subs
| Sub | Size | Speed | Active | Passive | Torpedoes |
| --- | --- | --- | --- | --- | --- |
| Leviathan | Huge | Medium | Easy | Fair | 2 |
| Whisper | Medium | Slow | Fair | Hard | 4 |
| Barracuda | Small | Fast | Hard | Easy | 4 |
| Minnow | Tiny | Very slow | Very hard | Very hard | 2 |
| Red October (secret) | Huge | Medium | Easy | Very hard | 0 |
