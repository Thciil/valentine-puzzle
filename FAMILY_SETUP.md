# Family Setup Guide - Multiple Valentines 💕

This guide explains how to use one deployment for multiple people in your family.

## How It Works

The site uses URL parameters to customize the experience for different people. One deployment, multiple valentines!

**Examples:**
- `https://Thciil.github.io/valentine-puzzle/` → Valentina (default)
- `https://Thciil.github.io/valentine-puzzle/?name=Mathilde` → Mathilde (brother's wife)
- `https://Thciil.github.io/valentine-puzzle/?name=Jette` → Jette (mother)
- `https://Thciil.github.io/valentine-puzzle/?name=Natalie` → Natalie (sister)

## Folder Structure

Create separate image folders for each person:

```
images/
├── valentina/          (your default, or just use images/ root)
│   ├── captcha-1.png
│   ├── captcha-2.png
│   ├── ...
│   ├── captcha-9.png
│   ├── tile-1.png
│   ├── ...
│   ├── tile-9.png
│   └── full-image.png
├── mathilde/           (brother → Mathilde)
│   ├── captcha-1.png
│   ├── ...
│   └── full-image.png
├── jette/              (father → Jette)
│   ├── captcha-1.png
│   ├── ...
│   └── full-image.png
└── natalie/            (sister's boyfriend → Natalie)
    ├── captcha-1.png
    ├── ...
    └── full-image.png
```

**Important:** Folder names must be lowercase (mathilde, jette, natalie).

## Setup Steps

### 1. For Valentina (Your Version)

Keep images in root `images/` folder or create `images/valentina/`:
- 9 captcha images: `captcha-1.png` through `captcha-9.png`
- 9 puzzle tiles: `tile-1.png` through `tile-9.png`
- 1 full image: `full-image.png`

**URL to share:** `https://Thciil.github.io/valentine-puzzle/`

### 2. For Brother → Mathilde

Create `images/mathilde/` folder with:
- 9 captcha images of brother + Mathilde
- 9 puzzle tiles (one photo split into 3×3)
- 1 full image

**URL to share with brother:**
```
https://Thciil.github.io/valentine-puzzle/?name=Mathilde
```

### 3. For Father → Jette

Create `images/jette/` folder with:
- 9 captcha images of father + Jette
- 9 puzzle tiles
- 1 full image

**URL to share with father:**
```
https://Thciil.github.io/valentine-puzzle/?name=Jette
```

### 4. For Sister's Boyfriend → Natalie

Create `images/natalie/` folder with:
- 9 captcha images of boyfriend + Natalie
- 9 puzzle tiles
- 1 full image

**URL to share with sister's boyfriend:**
```
https://Thciil.github.io/valentine-puzzle/?name=Natalie
```

## What Happens Automatically

When someone opens a URL with `?name=Mathilde`:
1. Greeting changes to "Dear Mathilde..."
2. All images load from `images/mathilde/` folder
3. Everything else works the same

## Helping Family Members

### Option A: You Create All The Images
1. Collect photos from each person
2. Create all the folders and images
3. Deploy once
4. Share the custom URLs

### Option B: They Fork Your Repo
1. They fork your repository
2. You help them replace images
3. They deploy to their own GitHub Pages
4. More work but gives them ownership

**Recommendation:** Option A is simpler - you do the image prep, they just share the URL!

## Image Preparation Tips

**For captcha images:**
- Use different photos of the couple
- Square aspect ratio (1:1)
- ~300-500px is perfect
- Mix different moments/places

**For puzzle tiles:**
- Choose one romantic photo
- Split into 3×3 grid using Figma or online tool
- Each tile should be same size
- Tile-3 (top-right) is the empty space

**Tools for splitting images:**
- Figma (free, what original creator used)
- https://imagesplitter.net/
- Photoshop or any image editor

## Testing URLs Locally

Before deploying, test locally:
```
file:///path/to/valentine-puzzle/index.html?name=Mathilde
```

Make sure images load from correct folders.

## Deploy Once, Share Different URLs

After you've created all the image folders:
1. Commit and push to GitHub
2. Deploy to GitHub Pages (one time)
3. Share custom URLs with each person
4. They send it to their valentine 💕

---

**Family List:**
- ✅ You → Valentina (default URL)
- ✅ Brother → Mathilde (`?name=Mathilde`)
- ✅ Father → Jette (`?name=Jette`)
- ✅ Sister's boyfriend → Natalie (`?name=Natalie`)

---

Made with 🌌 by Lyra
