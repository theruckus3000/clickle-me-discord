# 📄 Clickable Image → Discord Invite (GitHub Pages)

This repository hosts a **single‑page website** that displays an image which acts as a **full‑image clickable button**.  
Clicking anywhere on the image redirects the user to a Discord invite link.

This method is ideal when you want something that *looks like an image* in chat previews but behaves like a link when clicked.

---

## 🚀 Live Page

```
https://theruckus3000.github.io/clickle-me-discord/
```

Opening this URL displays the meme image.  
Clicking anywhere on the image opens the Discord invite.

---

## 📦 Project Structure

```
/
├── index.html        # Webpage containing the clickable image
└── click-on-me.jpg   # The meme image displayed on the page
```

---

## 🛠️ Setup Instructions

### 1. Create a GitHub Repository

1. Go to GitHub → **New repository**
2. Name it (example): `clickle-me-discord`
3. Set visibility to **Public**
4. Click **Create repository**

---

### 2. Upload Your Image

1. In the repo, click **Add file → Upload files**
2. Upload your meme image (e.g., `click-on-me.jpg`)
3. Commit the changes

---

### 3. Create `index.html`

1. Click **Add file → Create new file**
2. Name it: `index.html`
3. Paste the following code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Click Me</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      background: #000;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
    }
    img {
      max-width: 100%;
      height: auto;
      cursor: pointer;
      display: block;
    }
  </style>
</head>
<body>
  <a href="https://discord.gg/grkAwQ9W">
    <img src="click-on-me.jpg" alt="Click on me, I dare you">
  </a>
</body>
</html>
```

4. Commit the file.

---

### 4. Enable GitHub Pages

1. Go to **Settings** in the repo
2. Scroll to **Pages**
3. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/root`
4. Click **Save**

GitHub will generate your live site URL.

---

### 5. Test the Page

Open your GitHub Pages URL in a browser.

You should see:

- The meme image centered on the page  
- Clicking anywhere opens your Discord invite  

When you paste the link into Discord, iMessage, etc., the preview will show the image — making it feel like a clickable image even though it’s actually a webpage.

---

## 🧠 Why This Works

Most platforms **do not allow clickable images** directly.  
PDFs download.  
Images cannot contain active hyperlinks.  
Discord strips metadata.

GitHub Pages solves this by:

- Displaying your image as a preview card  
- Allowing the entire image to be wrapped in a link  
- Loading instantly on desktop and mobile  
- Requiring no backend or scripts  

This is the cleanest, most seamless way to achieve “click the image → join my Discord.”

---

## ✔️ Done

Your setup is complete and working.  
If you want enhancements — auto‑redirect, analytics, custom styling, or a disguised URL — they can be added easily.
