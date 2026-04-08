# Fleet Broadcast — OBS Stream Overlay

## File Structure
```
fleet-broadcast/
  index.html        ← OBS Browser Source (1920×1080)
  control.html      ← Config/control panel
  assets/
    lory-uplink.mp4 ← Your video file
```

## Setup
1. Add video to `assets/lory-uplink.mp4`
2. Push to GitHub → Settings → Pages → main/root
3. Open `control.html` → set timings → Generate URL → copy
4. OBS: Add Source → Browser → paste URL → 1920×1080
5. **Right-click Browser Source → Properties → tick "Control audio via OBS"**
6. Your source now appears in the OBS Audio Mixer

## Changing timing
Open `control.html` → adjust → Generate URL → paste into OBS source → right-click → Refresh

## URL Parameters
| Param | Default | Description |
|-------|---------|-------------|
| `msg` | 320 | Message duration seconds (master) |
| `vid` | 159 | Video duration seconds (fixed) |
| `interval` | 56 | CRT interval % of message |
| `crt` | 1 | CRT flash duration seconds |
