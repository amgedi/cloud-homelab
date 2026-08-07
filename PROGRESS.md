# Progress Log

Just a running log of what I did, what broke, and what I learned. Newest entry will always be ontop!

### 2026-08-07
**What I did:** Spent real time on Bandit Level 13 & just decided to give up on it as i finally just closed on the idea its an error (the one with the SSH key login), tried multiple valid approaches (localhost, full hostname, verbose debugging), confirmed via -v output that my key loaded correctly. Also watched my first 3 A+ Core 1 videos on laptop hardware and mobile connectivity!
**What clicked:** Actually understand SSH key auth now, how -i works, why chmod matters (but only know what 600 does at the moment, i'll probably learn the rest of the numnbers as i go!), and how to read verbose SSH debug output to diagnose a connection issue instead of guessing blindly (somewhat..)
**What annoyed me:** The level itself seems to have a platform-side issue blocking the connection, independent of anything I did. Confirmed it via other people hitting the identical error online, not just a random guess.
**Random thought:** Learned when to stop pushing on something that's not me, and move forward anyway with the concept intact! That's arguably more useful than the actual password would've been if i'm being quite honest.

### 2026-08-06
**What I did:** Cracked Level 12! It was multi layer decompression  (xxd, gzip, bzip2 loop) and pushed into Level 13 (SSH private key login). Learned about file ownership, chmod abit more extensively, /tmp as scratch space, and copying files across permission boundaries!
**What clicked:** Compressed files always look like gibberish with cat... at least it's normal & not broken though! Also finally got why /tmp exists as a universal writable scratch space when your own home folder can be locked down.
**What annoyed me:** Level 13 kept failing with a "connecting from localhost is blocked" error even after doing everything right i believe? HOPEFULLY it's a serverside quirk & not something I did wrong but i'm saying this as cope to validate a frustrating 30+ min session.
**Random thought:** Realized today that troubleshooting something that ISN'T my fault is its own skill! knowing when to say "this might just be a server issue" instead of endlessly blaming my own command is new for me though, thought it was only movie talk up until now😭

### 2026-08-05
**What I did:** Explored whether Boot.dev or an aio app could replace this whole process (turns out no single platform does 0-to-DevOps (confirmed via research, it's normal to stitch multiple free resources together). Pushed Bandit up to Level 10. Had a real conversation about what Bandit is actually testing.
**What clicked:** The big one today. Bandit isn't about memorizing exact command syntax, it's about recognizing the *category* of problem (searching inside a file? finding files by property? removing duplicates?) and then knowing what tool fits, even if I have to look up the exact flags. That reframes basically everything I've been stressing about lol, overthinking is really a killer!
**What annoyed me:** Almost went down a rabbit hole trying to find "the one app that does everything", turns out that doesn't exist so we're back to what I've already been doing (mixing Bandit + lessons + real practice) is basically what every roadmap recommends anyway.
**Random thought:** Feeling less like I'm "behind" and more like I'm starting to think the way this field actually wants me to think, pattern recognition over memorization! Level 10 by day 4, not bad. 3-4 hours today, calling it quits here.

### 2026-08-04
**What I did:** Finished Linux Survival Module 2 (permissions concept via the zoo analogy), worked through a LinuxJourney challenge on cp/mv/rm. learned to back up files with `cp` and use `-r` for copying whole directories recursively..? (whatever that means, i only understand 50% of it at the moment aswell😅)
**What clicked:** Permissions finally made sense from two angles now (zoo metaphor + my own lesson plan) & rwx isn't just random letters anymore. Also understood why `-r` is needed for folders but not single files (recursion = digging into everything inside).
**What annoyed me:** Hit a tired/confused wall after ~3 hours across two platforms. felt like I was going pretty slow even though looking back, I actually covered a lot (Bandit to Level 5, WSL2 installed, 3 learning platforms touched, and I can now reason through commands instead of just copying them), so i guess progress really does make perfect!
**Random thought:** Got clarity today on what "the goal" actually is. Bandit + A+ Core 1 are the real targets now, everything else (LabEx, Linux Survival, TryHackMe) is just supplementary from here on out. Feels good to have less noise. Tomorrow: back to Bandit Level 5 with fresh eyes, a newly installed WSL 2, and prayers that this doesn't actually sound like jargon in the near future..

### 2026-08-03
**What I did:** Worked through Bandit up to Level 6, hit a wall on the find command's flags (-size, -not -executable). Also downloaded WSL2 + Ubuntu to have my own sandbox.
**What clicked:** find is basically a filtered search - once broken into pieces (where to look, filter by size, filter by permission) it stopped looking like gibberish, now i gotta memorize it!
**What bothered me:** Trying to learn new syntax under puzzle pressure is rough. kept blanking even after the command was explained piece by piece, overthinking is a killer but we're gonna push through it! its how we grow as people!
**Random thought:** Having my own Ubuntu now feels like getting a practice field instead of just taking exams. No pressure to "get it right" first try! i think..?

### 2026-08-02
**What I did:** Started TryHackMe's Pre Security path, got through most of Computer Fundamentals thankfully! 
**What clicked:** Terminal stuff is way less scary than I thought, whoami and id are basically just "who am I and what am I allowed to touch", praying to get over my overthinking & ego!
**What annoyed me:** Hit a paywall mid-path (of course) so pivoting to Bandit + free A+ videos going forward until we gain credible skils.. i hope..?
**Random thought:** 3 hours in on day one, not bad for someone who's never touched a terminal before but most of it was like staring at an airplane construction manual.. geez..
