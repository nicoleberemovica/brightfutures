# Bright Futures
**A refugee-led initiative bringing solar energy, clean water, and digital access to Northern Uganda.**

---

## About This Project

Bright Futures was founded by community members from Northern Uganda to solve real problems from the inside out. Every project starts with the people closest to the challenge.

**Our two projects so far:**

- **Bright Minds, Bright Lights** *(Completed)* — Installed solar panels and WiFi at the Dongriin Foundation learning center. Raised $1,606 from 52 donors. Students can now study after dark and take online courses.
- **Bright Fields** *(Current)* — Bringing solar-powered water pumps to support irrigation and food security for farming families in Northern Uganda.

**Co-Founders:** Anyieth Philip Ayuen (Project Lead) and Nicole Beremovica

---

## How to Navigate the Website

When you open the website, here is what you will find as you scroll down:

| Section | What It Contains |
|---|---|
| **Top Navigation Bar** | Logo and links to jump to any section. On mobile, tap the menu icon (☰) in the top-right corner. |
| **Hero (top of page)** | A headline introducing Bright Fields and a "Support Bright Fields" button. |
| **Bright Fields** | Details about the current solar water pump project with photo placeholders. |
| **Our Story** | The founders' background and the mission behind Bright Futures. |
| **Impact** | Key numbers — money raised, projects completed, and communities reached. |
| **Bright Minds, Bright Lights** | The completed first project with a campaign video. |
| **Testimonials** | A quote from a student who benefited from the learning center. |
| **Donate** | A call to action to support Bright Fields financially or by sharing the page. |

A floating **Donate** button also appears in the bottom-right corner as you scroll past the top of the page.

---

## How to Edit the Website

> You do not need any coding experience to make basic edits. Follow the steps below carefully.

### What file to edit

The entire website lives in **one file**: `index.html`

Open it with any text editor:
- **Windows:** Right-click the file → "Open with" → Notepad (or Notepad++)
- **Mac:** Right-click the file → "Open with" → TextEdit (switch to plain text mode) or VS Code
- **Recommended for everyone:** Download [Visual Studio Code](https://code.visualstudio.com/) (free) — it highlights the code in colors which makes it much easier to read.

---

### How to change text on the page

1. Open `index.html` in your text editor.
2. Press **Ctrl+F** (Windows) or **Cmd+F** (Mac) to open the search bar.
3. Type the words you want to change and press Enter to find them.
4. Click on the text in the file, delete it, and type your new words.
5. Save the file with **Ctrl+S** (Windows) or **Cmd+S** (Mac).

**Example:** To update the fundraising amount, search for `$1,606` and replace it with the new number.

> ⚠️ **Important:** Only change the words themselves. Do **not** delete the angle brackets `< >` or quotation marks `" "` around the text — those are part of the code structure and the page will break without them.

---

### How to change the video

The campaign video file is named `BRIGHT MINDS, NO LIGHTS CAMPAIGN.mp4` and must be in the same folder as `index.html`.

To swap it for a different video:
1. Add your new video file to the same folder as `index.html`.
2. In `index.html`, press **Ctrl+F** / **Cmd+F** and search for `<video`.
3. Find this line:
   ```
   <source src="BRIGHT MINDS, NO LIGHTS CAMPAIGN.mp4" type="video/mp4">
   ```
4. Replace `BRIGHT MINDS, NO LIGHTS CAMPAIGN.mp4` with your new video's filename.
5. Save the file.

> ⚠️ Make sure your video file name matches exactly, including any spaces or capital letters.

---

## How to Add Photos

The website currently shows dashed placeholder boxes where photos will go. Here is how to replace them with real images.

### Step 1 — Add your image to the project folder

Copy your photo file (`.jpg` or `.png`) into the same folder as `index.html`.

> Tip: Rename your photo to something simple with no spaces, for example: `bright-fields-1.jpg` instead of `IMG_4823 (2).jpg`

---

### Step 2 — Find a photo placeholder in the code

1. Open `index.html` in your text editor.
2. Press **Ctrl+F** / **Cmd+F** and search for:
   ```
   photo-placeholder
   ```
3. You will find sections that look like this:
   ```html
   <div class="photo-placeholder">
     <span>Photo coming soon</span>
   </div>
   ```

---

### Step 3 — Replace the placeholder with your image

Delete the entire placeholder block (from `<div class="photo-placeholder">` to its closing `</div>`) and paste this in its place:

```html
<img src="YOUR-PHOTO-NAME.jpg" alt="A short description of the photo" style="width:100%; height:100%; object-fit:cover; border-radius:12px;">
```

Replace `YOUR-PHOTO-NAME.jpg` with your actual file name, and replace the description in `alt="..."` with a few words describing the photo (for example: `alt="Solar panels at the learning center"`).

**Example — before:**
```html
<div class="photo-placeholder">
  <span>Photo coming soon</span>
</div>
```

**Example — after:**
```html
<img src="bright-fields-1.jpg" alt="Solar water pump in the field" style="width:100%; height:100%; object-fit:cover; border-radius:12px;">
```

> ⚠️ Do not leave any extra spaces or delete the quotation marks around the file name.

---

## How to Publish Changes to GitHub

After editing and saving `index.html`, you need to push the changes to GitHub so they appear online.

**Option A — GitHub Desktop (recommended for beginners):**
1. Download [GitHub Desktop](https://desktop.github.com/) (free).
2. Open the app and sign in to your GitHub account.
3. It will show your changed files. Add a short description (e.g. "Added photos to Bright Fields section").
4. Click **Commit to main**, then click **Push origin**.

**Option B — Terminal / Command Line:**
```bash
git add .
git commit -m "Your short description of what you changed"
git push
```

---

## Project File Structure

```
brightfutures/
├── index.html                              # The entire website (HTML + CSS + JS all in one file)
├── BRIGHT MINDS, NO LIGHTS CAMPAIGN.mp4   # Campaign fundraising video
└── README.md                              # This guide
```

---

*Built by the community, for the community.*
