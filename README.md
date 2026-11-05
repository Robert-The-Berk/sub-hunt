# Sub Hunt

A turn-based submarine hunt on a 40×26 sonar plotting table. An enemy sub is stalking a friendly convoy on its way west to the escape line; find it with active pings and passive sonobuoys, sink it with depth charges, and keep the convoy afloat.

Open `index.html` in a browser to play. No build step.

## Sensors
- **Active buoys** (6): drop one and it pings every turn for 4 turns. A ping returns a range ring only if the sub is within 10 nmi, and only as often as the sub's size allows.
- **Counter-detection**: the sub hears pings out to 24 nmi, much further than you can hear its echo. When it does, it sprints and steers to stay out of that buoy's range, so lay active buoys where it has to go.
- **Passive buoys** (8): silent, report a bearing up to 16 nmi. Fast subs are loud; slow subs are quiet.

## Decoys
When a ping catches it or a depth charge lands close, the sub may drop a noisemaker and creep away deep and slow for a few turns, holding its torpedoes. A decoy echoes like the sub on active buoys, but there are tells: passive buoys report broadband noise with **no clear blade rate**, its waterfall trace is broad and smeared, it barely moves, and a buoy may catch a **short mechanical transient** when one is launched. A charge on a decoy reports the noise cutting out with no breaking-up sounds. With Jonesy on watch, he calls them out.

## Sonar waterfall
The waterfall shows what one passive buoy hears: bearing across, time going down, newest at the top. Pick the buoy from the tabs. Convoy ships, torpedoes and whales all leave traces, and white ticks mark the friendly bearings. The sub's trace appears even when it is too faint for a logged contact, so a weak line holding a steady bearing is worth acting on. Hover to read a bearing, and click to plot it on the map.

## Plot pencil
Press **4** or pick **Plot** to mark up the table yourself. It's free and doesn't use a turn. Click a square to drop a guess mark labelled with the current turn, and click it again to erase it. Drag to draw a course line with an arrowhead. **Undo** and **Clear plot** tidy up. Bearings plotted from the waterfall use the same pencil colour, and the replay shows your plot alongside the sub's real track.

## Replay
When a hunt ends, **Watch replay** plays it back turn by turn: the sub's course, every buoy drop, ping return, bearing, torpedo and depth charge, with that turn's events underneath. Scrub with the slider or pause.

## The convoy
Four friendly merchant ships sail east along a marked route. The sub closes to within 8 nmi and fires torpedoes. Each launch is loud: the targeted ship reports a bearing, buoys hear it more easily, and the torpedo's run is shown, so you get one turn to answer. A sub that was just pinged or charged fires less often. You can't drop a depth charge on top of a friendly ship.

You have 6 active buoys, 8 passive buoys and 6 depth charges. You lose if every ship is sunk, if you run out of charges, or if the sub crosses the escape line. The Red October mission has no convoy.

## Debrief and scoring
Every hunt ends with a scored debrief:

| | Points |
| --- | --- |
| Sub sunk (or Red October found) | 1,000 |
| Each convoy ship saved | 300 |
| Speed, on a win | 5 × (90 − turns), never below 0 |
| Gear left, on a win | 60 per charge, 25 per active buoy, 15 per passive buoy |
| Silent hunter / One ping only | 200 / 150 |
| Not fooled by decoys (sub used decoys, you never charged one) | 150 |

A win earns 1 star, 2 stars from 2,000 points and 3 stars from 2,600 (1,250 and 1,500 on missions with no convoy). Your best quick-hunt score for each target is saved.

## Campaign
Five missions in a row (**Shakedown**, **Quiet Water**, **Fast Mover**, **Needle** and **Ghost**) drawing from one supply pool: 18 active buoys, 26 passive buoys and 18 depth charges. Each mission takes up to the normal loadout from the pool. Unused gear goes back afterwards, and each win adds +2 active, +3 passive and +2 charges. You can retry a failed mission, but what you spent is gone. If the pool runs out of charges, the campaign is over. Progress, the campaign score and your best campaign are saved in the browser. Starting a mission takes its gear from the pool straight away, so leaving mid-mission forfeits it.

## Subs
| Sub | Size | Speed | Active | Passive | Torpedoes | Decoys |
| --- | --- | --- | --- | --- | --- | --- |
| Leviathan | Huge | Medium | Easy | Fair | 2 | 2 |
| Whisper | Medium | Slow | Fair | Hard | 4 | 3 |
| Barracuda | Small | Fast | Hard | Easy | 4 | 3 |
| Minnow | Tiny | Very slow | Very hard | Very hard | 2 | 1 |
| Red October (secret) | Huge | Medium | Easy | Very hard | 0 | 1 |
