# Tell HN: My fish died because of CoderPad

**Posted by RomanPushkin on 2025-07-02**

I'm not writing this to be dramatic—just wanted to share something that happened, and maybe it’ll be useful to someone.

I have a small apartment with a few fish tanks. When one of my fish gets sick, I move it to a separate "quarantine" tank where I can monitor it more closely—especially water temperature, which can spike due to direct sunlight.

To help with this, I built a small JavaScript script that runs in my browser via TamperMonkey. It reads from a temperature sensor through a local API and plays a loud alert sound if things get too hot. It’s not fancy, but it’s worked fine for months. I’m not a hardware or desktop developer—web is my platform, and this was my DIY solution.

Some time ago, I had a two-hour technical interview using CoderPad. I stayed focused in the browser tab the whole time. At some point, the alert I normally hear when things go wrong didn’t go off. When I finished the interview, I checked—the quarantine tank had overheated, and unfortunately, the fish didn’t survive.

After digging a bit, I suspect what happened is this: CoderPad (or something in its environment) intercepts and blocks fetch calls from browser scripts. Maybe to prevent AI helpers or tampering—I’m not sure. But my alert system relied on those fetch calls to read from the temperature sensor. During the interview, those calls silently failed, and I never got the warning.

Now I’m left wondering: who’s at fault here? Me, for building something fragile? CoderPad, for blocking browser functionality in the name of test integrity? Or is it just one of those weird, sad intersections of code and real life. :(

Anyway, just needed to tell someone.