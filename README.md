Referral Rush
The directory said yes. The office said no. Now the member is calling back, and they are not calm.

☎️ Take the calls
About 2 minutes. Sound on if you can.

Your shift starts now
You're on the specialist referral line at Caliche Creek Medical Group. The phone is ringing. Gloria needs a heart doctor. Three providers come up in the directory and they all look perfect.

At least one of them moved. Or left the network. Or stopped taking new patients. The directory won't tell you which.

Pick wrong and a week later Gloria calls back, frustrated, and you start the whole referral over.

Two rounds, one big difference
Round 1: Today. Every record looks equally trustworthy. Good luck.

Round 2: With confidence flags. An AI check scores every record before you send. Same job, completely different shift.

In between, there's a bonus round of hold music. Yes, you can score points on hold.

What's on the line
Speed bonus. Callers have patience, and it runs out. They go from Calm to Antsy to Fuming.
Streaks. Clean referrals in a row stack extra points.
Catches. Call the office to verify a record. It costs you 4 minutes, but a caught bad record pays.
Callbacks. Send a bad one and it costs you 15 minutes and a very annoyed caller.
A rank and badges at the end. Some of them are harder to unlock than they look.
Most people bounce at least one referral in Round 1. See if you can get through clean.

Behind the scenes
A few crumbs from the code. The rest stays on hold.

Every record gets a confidence score, and the score decides the flag you see:

const level = p => p.score >= 80 ? 'high' : p.score >= 50 ? 'check' : 'low';
const LEVEL = { high: 'Looks good', check: 'Verify first', low: 'Likely wrong' };
The game is rigged on purpose. It's a short demo, so two of the three providers on a heavy call are bad records. The problem shows up fast.

const chosen = heavy && trap.length > 1
  ? [ok[0], trap[0], trap[1]]
  : [ok[0], trap[0], /* one more, random */];
The math behind a bad send. Every action costs time, and a callback costs the most:

const BASE = 3, VERIFY = 4, CALLBACK = 15; // minutes
Callers lose patience in real time.

function mood(r){ return r>18 ? 'Calm' : r>8 ? 'Antsy' : r>0 ? 'Fuming' : 'Hello??'; }
The hold music, the ambient soundtrack and the ringing phone are all generated live in the browser with the Web Audio API. No audio files.

What's actually behind each flag, and how the badges unlock... you'll have to play.

The idea
Referral Rush is a playable demo of Provider Data Confidence, a concept for flagging bad provider directory records before a referral ever goes out. Round 1 shows the problem. Round 2 shows the fix.

Caliche Creek Medical Group and every member, provider, address and phone number in the game are fictional.

Built with
One HTML file. Vanilla JavaScript, CSS and the Web Audio API. No frameworks, no audio files, no build step.

Made by
Olu Ladipo Portfolio · LinkedIn

☎️ Line one is ringing
