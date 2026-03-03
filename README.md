# Fan Account – Select Tickets to Sell (Prototype)

Static prototype for the 2.0 Fan Account “Select Tickets to Sell” flow.

---

## Host on GitHub

### 1. Create a new repo on GitHub

- Go to [github.com/new](https://github.com/new).
- Name the repo (e.g. `fan-account-prototype`).
- Choose **Public**, leave “Add a README” **unchecked** (you already have one).
- Click **Create repository**.

### 2. Push this folder to the repo

In your terminal, from the **prototypes** folder:

```bash
cd /Users/bwang/Documents/GitHub/prototypes

# One-time: init and first commit
git init
git add .
git commit -m "Initial commit: Fan Account Select Tickets prototype"

# Add your GitHub repo as remote (replace YOUR_USERNAME and REPO_NAME with yours)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push (use main or master to match your default branch)
git branch -M main
git push -u origin main
```

After this, the code lives on GitHub and you can share the repo link or clone it.

### 3. (Optional) Host the app with GitHub Pages

To get a **shareable URL** (e.g. `https://YOUR_USERNAME.github.io/REPO_NAME/`):

1. In the repo on GitHub: **Settings** → **Pages** (left sidebar).
2. Under **Source**, choose **Deploy from a branch**.
3. Branch: **main** (or **master**). Folder: **/ (root)**. Save.
4. After a minute or two, the site will be at:
   - `https://YOUR_USERNAME.github.io/REPO_NAME/`  
   (GitHub Pages serves `index.html` from the root, so the prototype will load there.)

---

## Deploy to Vercel (shareable link)

1. **Install Vercel CLI** (if needed):
   ```bash
   npm i -g vercel
   ```

2. **From this folder, deploy**:
   ```bash
   cd /Users/bwang/Documents/GitHub/prototypes
   vercel
   ```

3. Follow the prompts:
   - Log in or link your Vercel account if asked.
   - Confirm the project (or create a new one).
   - Vercel will print a URL like `https://your-project-xxx.vercel.app`.

4. **Production deploy** (optional):
   ```bash
   vercel --prod
   ```

The app is served from **index.html** at the root, so the shareable URL is the project URL (no path).

## Assets

Ensure these files exist in this folder so images load:

- `billie-eilish-event.png` – event card image  
- `info-icon.png` – blue info banner icon  
- `error-icon.png` – error banner icon  

If any are missing, copy them from your assets (e.g. `.cursor/projects/.../assets/`) into this folder before deploying.

## Run locally

```bash
open index.html
# or
npx serve .
# then open http://localhost:3000
```
