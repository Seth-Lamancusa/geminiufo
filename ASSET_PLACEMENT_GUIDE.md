# Asset Placement Guide

This document outlines where to place assets and links in the site.

## Required Links (Update in HTML files)

### YouTube Video Link
**Location:** `index.html` (line ~67)
- Find the element with `id="youtube-link"`
- Replace `href="#"` with your YouTube video URL
- Example: `href="https://www.youtube.com/watch?v=YOUR_VIDEO_ID"`

### Google Drive Links
**Locations:**
1. `index.html` (line ~73) - element with `id="drive-link"`
2. `sources.html` (line ~18) - element with `id="drive-link-sources"`
3. `sources.html` (line ~95) - element with `id="drive-link-main"`

Replace all `href="#"` with your public Google Drive folder URL.

## Required Image Assets

### D-15 Frame Images
**Location:** `investigation.html` - D-15 Frames Section (around line 280)

Place D-15 frame images in a folder (suggested: `_site/assets/d15-frames/`) and update the placeholder divs:

**Frames needed:**
- Frame 364
- Frame 517
- Frame 876
- Frame 11560 (anomalous EM effects)
- Frame 14988 (anomalous EM effects)
- Frame 15076
- Frame 15108 (unique shape)
- Frame 15195 * (matches UFO)
- Frame 15355
- Frame 15406 * (matches UFO)
- Frame 15535 * (matches UFO)
- Frame 15552 * (matches UFO)

**To add:** Replace each `<div class="frame-placeholder">` section with:
```html
<img src="_site/assets/d15-frames/frame-XXXX.jpg" alt="D-15 Frame XXXX" class="frame-img">
```

### Featured D-15 Frame (Homepage)
**Location:** `index.html` - Featured Evidence section (around line 50)

Replace the placeholder div with an actual D-15 frame image. Suggested: use one of the frames that matches the UFO (15195, 15406, 15535, or 15552).

### Comparison Images
**Location:** `investigation.html` - Comparison Gallery section (around line 320)

1. **Hasselblad S66-54585**
   - Replace placeholder in "Hasselblad S66-54585" comparison item
   - Suggested path: `_site/assets/hasselblad-s66-54585.jpg`

2. **Mission Report Cover (NASA-S-66-9017)**
   - Replace placeholder in "Mission Report Cover" comparison item
   - Suggested path: `_site/assets/mission-report-cover.jpg`

**To add:** Replace each `<div class="frame-placeholder">` with:
```html
<img src="_site/assets/[filename].jpg" alt="[Description]" class="comparison-img">
```

## Suggested Folder Structure

```
_site/
  assets/
    ufo.jpg (already exists)
    d15-frames/
      frame-364.jpg
      frame-517.jpg
      frame-876.jpg
      frame-11560.jpg
      frame-14988.jpg
      frame-15076.jpg
      frame-15108.jpg
      frame-15195.jpg
      frame-15355.jpg
      frame-15406.jpg
      frame-15535.jpg
      frame-15552.jpg
    hasselblad-s66-54585.jpg
    mission-report-cover.jpg
```

## Notes

- All placeholder sections are clearly marked with `placeholder-text` and `placeholder-note` classes
- The site will function with placeholders, but images should be added for the full presentation
- Ensure all images are optimized for web (reasonable file sizes)
- Use descriptive alt text for accessibility

## Quick Checklist

- [ ] Add YouTube video URL to `index.html`
- [ ] Add Google Drive URL to all three locations
- [ ] Add D-15 frame images (12 frames)
- [ ] Add featured D-15 frame to homepage
- [ ] Add Hasselblad S66-54585 comparison image
- [ ] Add Mission Report Cover comparison image
