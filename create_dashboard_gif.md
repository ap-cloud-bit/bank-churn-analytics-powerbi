# Creating a Power BI Dashboard Demo GIF

## Step 1 — Record your screen  
Use any free tool:
- OBS Studio  
- Loom  
- Xbox Game Bar (Win + G)

Record a 10–12 second demo of your dashboard:
- Hover over visuals  
- Click slicers  
- Switch pages  

Save the recording as an MP4 video.

---

## Step 2 — Convert MP4 to GIF

### Online converter:
https://cloudconvert.com/mp4-to-gif

### FFmpeg (advanced users):
```bash
ffmpeg -i dashboard.mp4 -vf "fps=10,scale=1280:-1" dashboard.gif
