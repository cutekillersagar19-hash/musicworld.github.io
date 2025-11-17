# MusicWorld — Static Music Website

This package contains a single-file static website `index.html` named **MusicWorld**.
Features:
- Play local audio files (drag & drop or Add Files).
- Library & playlist management.
- YouTube & SoundCloud embed support (embedded tracks).
- Import / Export playlist as JSON.
- Save/load using `localStorage`.

## Files
- `index.html` — the whole site (HTML, CSS, JS).

## How to use locally
1. Download and unzip.
2. Open `index.html` in your browser (double-click or right-click → Open with...).
3. Add audio files with **Add Files** or drag & drop. Use embed box for YouTube/SoundCloud.

## Deploy to GitHub Pages (recommended — free)
1. Create a GitHub account: https://github.com
2. Create a new repository named: `yourusername.github.io` (replace `yourusername` with your GitHub username).
3. Upload `index.html` to the repository root:
   - On GitHub website: Add file → Upload files → Commit changes.
   - Or use git:
     ```
     git init
     git add index.html
     git commit -m "Initial MusicWorld site"
     git branch -M main
     git remote add origin git@github.com:yourusername/yourusername.github.io.git
     git push -u origin main
     ```
   (If you prefer HTTPS remote, use `https://github.com/yourusername/yourusername.github.io.git`.)
4. Wait a minute, then visit: `https://yourusername.github.io`

## Using a custom domain (optional)
1. Register a free domain at https://www.freenom.com (e.g., `.tk`, `.ml`, `.ga`).
2. Point DNS `A` records (or ALIAS) to GitHub Pages IPs — see GitHub Pages docs.
3. Add `CNAME` file to the repository with your custom domain name on the first line.

## SSH key (for pushing via SSH)
Generate SSH key (on your machine):
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub
# Copy the output and add to GitHub > Settings > SSH and GPG keys > New SSH key
```

## Notes & Limitations
- Music files added locally use `URL.createObjectURL` and are stored only in the browser session; the site cannot upload files to a server.
- Embedded YouTube/SoundCloud rely on the third-party site's policies.
- I cannot create the GitHub repository on your behalf — you must sign in to your GitHub account to create the repo and push files.

If you'd like, I can:
- Create a `musicworld.zip` with these files (already prepared).
- Provide exact `git` commands tailored to your username.
- Walk you step-by-step while you do the deploy (I'll provide commands and copyable steps).