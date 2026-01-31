# Deploying to Netlify

This is a single-file static app—no build step required.

## Option 1: Drag and Drop (Fastest)

1. Go to [netlify.com](https://netlify.com) and sign in
2. From your dashboard, look for the deploy dropzone
3. Drag the entire `todo` folder onto it
4. Done! Netlify gives you a live URL instantly

## Option 2: Connect Git Repository

1. Push this repo to GitHub/GitLab/Bitbucket
2. Go to [app.netlify.com](https://app.netlify.com)
3. Click **"Add new site"** → **"Import an existing project"**
4. Select your Git provider and authorize
5. Choose this repository
6. Configure build settings:
   - **Build command:** *(leave empty)*
   - **Publish directory:** `.` or `/`
7. Click **Deploy site**

Netlify will auto-deploy on every push to your main branch.

## Custom Domain (Optional)

1. From your site dashboard, go to **Domain settings**
2. Click **Add custom domain**
3. Follow the DNS configuration instructions

## That's It

No `netlify.toml` or build configuration needed. The app is a single `index.html` file that runs entirely in the browser with IndexedDB for storage.
