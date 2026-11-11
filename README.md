# Sim Racing Coach (beta)

A free lap recorder, voice coach and lap analyser for **iRacing, Assetto Corsa
Competizione, Assetto Corsa, Assetto Corsa EVO and Automobilista 2** on Windows.

It runs on your own PC. There's no account, nothing is uploaded, and it works offline.

## What it does

- **Records every lap** at 60 times a second while you drive: speed, pedals,
  steering, g-forces, tyres, suspension and more. It also records the other
  cars in the session (AI or online) so you can compare yourself with them.
- **Voice coach (optional):** after each corner it tells you where you lost
  time against your own best lap, and why: braked early, coasted before the apex,
  slow mid-corner, late on the power. It gives a lap time at the line and stays quiet
  in the corners and the braking zones.
- **Brake beeps (optional):** a countdown beep before each braking point from
  your best lap (or from faster drivers in the same session).
- **Analyser page:** one click opens your session in your web browser. It shows a
  corner-by-corner comparison of any two laps, your ideal lap from your best
  sections, a map and traces, coasting, brakes and driver aids, steering force
  clipping, and setup suggestions fitted to what your car can actually adjust.
- **Corner names:** checked names for Spa, Silverstone, Suzuka, Okayama and Lime
  Rock. If you own original Assetto Corsa, it also uses the corner names from
  that game's track files. Everything else shows as "Turn 1", "Turn 2" and so on,
  and you can name corners yourself.

## Install

1. Download the zip from **Releases** (on the right of this page), unzip it, and put
   `SimLapRecorder.exe` anywhere (the Desktop is fine).
2. Double-click it. Windows may show **"Windows protected your PC"**. That's
   normal for a new app that isn't signed. Click **More info**, then **Run anyway**.
3. Leave the window open and drive. Recordings go to
   `Documents\SimLapRecorder`, one folder per session.
4. After driving, click **Analyse last session**.

Sim-specific setup:

- **Automobilista 2:** Options > System > Shared Memory = **"Project CARS 2"**.
- **Assetto Corsa (original):** other cars need the small in-game app that comes
  with the recorder (see `HOW TO INSTALL.txt` in the download). Your own laps work without it.
- iRacing, ACC and AC EVO need no setup.

## How well each sim is tested (honestly)

So far it's been tested on **one PC**, which is why this is a beta.

| Sim | Status |
|---|---|
| AC EVO | Checked against the game with real laps: lap times, valid/invalid laps, all channels. |
| iRacing | Checked live: lap times, invalid laps, setups, other cars. |
| ACC | Checked live in solo practice. Other cars on track not seen yet. |
| Assetto Corsa | Checked live, including AI races. A timed lap invalidated by track limits not seen yet. |
| Automobilista 2 | Checked live. Its lap-invalid flag only fires for cuts that gain time; not seen yet. |

## Known limits

- Windows only.
- When a sim updates its telemetry, the recorder may need an update too.
- Setup advice follows standard race-engineering rules, one change at a time.
  It's a starting point, not a guarantee.
- Balance in iRacing and AMS2 is estimated from steering, because those sims
  don't report slip angles. It's marked "indicative".

## Feedback

This is a beta. If something looks wrong, open an issue on this page (the
**Issues** tab) and say which sim, car and track. Attach `recorder.log` from
`Documents\SimLapRecorder`, and the session folder (zipped) if you can.
