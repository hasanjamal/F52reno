# House Renovation Tracker – Clifton, Karachi

A simple, elegant static website to track our home renovation project and share progress with the family.

## 🏠 What's This

This is a **single-page HTML site** listing all renovation items across every room of the house. It's designed to be:
- Shared with family to review priorities
- Updated as phases are confirmed
- Published instantly via GitHub Pages (no backend needed)

## 🚀 Publishing to GitHub Pages

1. **Create a new GitHub repo** (e.g. `house-renovation`)
2. Push this folder's contents to the `main` branch
3. Go to **Settings → Pages**
4. Under *Source*, select `main` branch and `/ (root)` folder
5. Click **Save** — your site will be live at:
   ```
   https://yourusername.github.io/house-renovation/
   ```

## ✏️ Updating Phases

When the family has reviewed priorities, edit `index.html` and update each item's badge:

```html
<!-- Change "tbd" to the right phase: -->
<span class="item-badge tbd">To Decide</span>      <!-- not yet decided -->
<span class="item-badge phase1">Phase 1 – Now</span>  <!-- do now -->
<span class="item-badge phase2">Phase 2 – Later</span> <!-- later -->
<span class="item-badge skip">Skip</span>              <!-- not doing -->
```

The stats in the hero bar (Phase 1 count, Phase 2 count, etc.) update automatically based on the badges.

## 📁 File Structure

```
/
└── index.html      ← entire site (single file, no dependencies)
└── README.md       ← this file
```

No build step, no framework, no dependencies. Just open `index.html` in a browser or push to GitHub Pages.
