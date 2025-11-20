# ***42 Badge Generator***

Generate a customizable dynamic badge for your 42 intra profile.
Live website:

***https://badge-umber.vercel.app/***


This site allows you to create a personalized SVG badge showing your

- Name
- Login
- Campus
- Grade
- Level progress bar
- Avatar
- Optional animated GIF background Fully customizable colors, border, and shadow

The generated badge can be embedded anywhere (README, website, GitHub profile, etc).

## 🚀 Features

Fetches live data from the 42 API (user info & avatar)

Supports static themes + GIF backgrounds

Fully customizable colors:

- Accent
- Name color
- Title/secondary color
- Level bar text
- Border & shadow color

Auto-generates:

- Direct badge URL
- Markdown embed
- HTML embed

## 🖥️ How to Use the Website

### 1. Enter Your 42 Login

On the left side, enter your 42 intra username (ex: dda-fons).
This fetches your:

- Name
- Campus
- Email (if public)
- Grade
- Level
- Avatar
  
Your badge preview updates instantly.


### 2. Optional: Insert Your GitHub Username

This allows the generated Markdown to link to your GitHub profile.

3. Choose a Theme

Available base themes include:

Dark Blue
- Light
- Green
- Slate
- Red
- Purple
- Orange
- GIF Mode (explained next)

Selecting a theme updates the default colors automatically.

### 4. Choose a GIF Background (Optional)

Switch to the GIF theme and pick from the available GIFs or add your own:

Built-in GIFs (One Punch, Akira, Cutie, etc.)

Add custom GIF by pasting any https://...gif URL

When using GIF mode, additional color controls appear to help match the badge text to the GIF.

### 5. Customize Colors (GIF mode)

You can adjust:

- Text Color
- Title Color
- Level Color
- Accent Color
- Border Color
- Shadow Color

This ensures the badge stays readable even over complex GIF backgrounds.

The preview updates live.

### 6. Generate Your Badge

Click the Generate button.

You will receive:

- Direct Image URL
- Markdown (for GitHub README)
- HTML

## 📌 Notes

The server always uses theme darkblue when generating GIF badges — color overrides handle the rest.

Caching is disabled on the backend to ensure the badge always displays the latest version.

All GIFs are embedded as Base64 inside the final SVG to avoid CORS issues.

## 🛠️ Tech Stack
### Frontend
- React (Vite)
- Custom SVG generator
- URL builder for shared links

### Backend
- Node.jS + Express
- 42 Intra API integration
- Dynamic SVG generation
- GIF embedding & Base64 conversion

## 🌟 Example Badge
[![42 Badge](https://badge42-backend.onrender.com/api/badge/darkblue/dda-fons?gifUrl=https%3A%2F%2Fbadge42-f.vercel.app%2Fakira.gif&accent=%23FFFF00&fg=%23FFFF00&titleCol=%23FFFF00&bodyTextColor=%23FFFF00&borderColor=%23FFFF00&shadowColor=%23FFFF00&borderWidth=3)](https://github.com/dda-fons)
