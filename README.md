# Sub Hunt

A turn-based submarine hunt on a 40×26 sonar plotting table. An enemy sub is stalking a friendly convoy on its way west to the escape line; find it with active pings and passive sonobuoys, sink it with depth charges, and keep the convoy afloat.

Open `index.html` in a browser to play. No build step.

## Sensors
- **Active ping**: returns a range ring only if the sub is within 10 nmi, and only as often as the sub's size allows. Pinging warns the sub.
- **Passive sonobuoys**: silent, report a bearing up to 16 nmi. Fast subs are loud; slow subs are quiet.

## The convoy
Four friendly merchant ships sail east along a marked route. The sub closes to within 8 nmi and fires torpedoes. Each launch is loud: the targeted ship reports a bearing, buoys hear it more easily, and the torpedo's run is shown, so you get one turn to answer. A sub that was just pinged or charged fires less often. You can't drop a depth charge on top of a friendly ship.

You have 8 sonobuoys and 6 depth charges. You lose if every ship is sunk, if you run out of charges, or if the sub crosses the escape line. The Red October mission has no convoy.

## Subs
| Sub | Size | Speed | Active | Passive | Torpedoes |
| --- | --- | --- | --- | --- | --- |
| Leviathan | Huge | Medium | Easy | Fair | 2 |
| Whisper | Medium | Slow | Fair | Hard | 4 |
| Barracuda | Small | Fast | Hard | Easy | 4 |
| Minnow | Tiny | Very slow | Very hard | Very hard | 2 |
| Red October (secret) | Huge | Medium | Easy | Very hard | 0 |
