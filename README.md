# Sub Hunt

A turn-based submarine hunt on a sonar plotting table. A sub is running west for the escape line; find it with active pings and passive sonobuoys, then sink it with depth charges.

Open `index.html` in a browser to play. No build step.

## Sensors
- **Active ping**: returns a range ring only if the sub is within 10 nmi, and only as often as the sub's size allows. Pinging warns the sub.
- **Passive sonobuoys**: silent, report a bearing up to 16 nmi. Fast subs are loud; slow subs are quiet.

## Subs
| Sub | Size | Speed | Active | Passive |
| --- | --- | --- | --- | --- |
| Leviathan | Huge | Medium | Easy | Fair |
| Whisper | Medium | Slow | Fair | Hard |
| Barracuda | Small | Fast | Hard | Easy |
| Minnow | Tiny | Very slow | Very hard | Very hard |
| Red October (secret) | Huge | Medium | Easy | Very hard |
