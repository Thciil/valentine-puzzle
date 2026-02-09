# Setup Instructions for Valentina's Valentine Puzzle

## What's Been Done

✅ Changed "Gaby" to "Valentina"  
✅ Added captcha stage before the envelope  
✅ Styled captcha to look like a real CAPTCHA  
✅ Added logic: must select all 9 images before proceeding

## What You Need to Do

### 1. Add Captcha Images (9 photos of you two)

In the `images/` folder, add 9 images named:
- `captcha-1.png`
- `captcha-2.png`
- `captcha-3.png`
- `captcha-4.png`
- `captcha-5.png`
- `captcha-6.png`
- `captcha-7.png`
- `captcha-8.png`
- `captcha-9.png`

**Recommendations:**
- Use different photos of you and Valentina together
- Square aspect ratio works best (1:1)
- Size: ~300-500px is perfect
- Mix of different moments/places makes it more romantic

### 2. Add Puzzle Images (from original README)

Cut one photo into a 3×3 grid:
- `tile-1.png` through `tile-9.png` (numbered left-to-right, top-to-bottom)
- `full-image.png` (the complete photo)

### 3. Customize Messages (Optional)

In `index.html`, you can change:
- Line 628: `"Dear Valentina..."` 
- Line 638: `"...you complete me."`
- Line 639: `"Will you be my Valentine?"`

### 4. Test Locally

Open `index.html` in a browser:
1. Should see "I'm not a robot" checkbox
2. Click it → captcha appears
3. Click all 9 images
4. Click "Verify" → envelope appears
5. Click envelope → puzzle opens
6. Solve puzzle → valentine question appears
7. Click "Yes" → celebration! 🎉

### 5. Deploy to GitHub Pages

Once everything looks good:
1. Commit and push to GitHub
2. Go to repo Settings → Pages
3. Source: Deploy from branch → `main`
4. Your site will be at: `https://Thciil.github.io/valentine-puzzle/`

---

## Flow Summary

**Stage 0:** "I'm not a robot" checkbox  
↓  
**Stage 1:** Captcha - select all images with "your valentine"  
↓  
**Stage 2:** Envelope appears and opens  
↓  
**Stage 3:** Solve 3×3 sliding puzzle  
↓  
**Stage 4:** Valentine question appears  
↓  
**Stage 5:** Click "Yes" → Celebration with confetti! 🎊

---

Made with 🌌 by Lyra
