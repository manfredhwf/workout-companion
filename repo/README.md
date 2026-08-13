# Workout tracker

A installable web app that shows exactly which exercise to do next, with sets, reps,
weight, and an embedded demo video for each one. Works offline once installed.

## Deploy this repo to GitHub Pages

1. Create a new **public** repository on GitHub and push this folder to it:

   ```
   git init
   git add .
   git commit -m "Workout tracker PWA"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

2. In the repo on GitHub, go to **Settings → Pages**, and under **Build and
   deployment → Source**, choose **GitHub Actions**. The included workflow
   (`.github/workflows/deploy.yml`) will run automatically and publish the site.

3. After the workflow finishes (check the **Actions** tab), your app is live at:

   ```
   https://<your-username>.github.io/<your-repo>/
   ```

Every future push to `main` redeploys automatically — no manual steps.

## Install it on Android

1. Open the URL above in **Chrome** on your phone.
2. Tap the **⋮** menu → **Add to Home screen** (or use the install prompt if
   Chrome offers it automatically).
3. Launch it from your home screen — it opens full-screen, with no browser bar,
   and keeps working without signal once it's been opened at least once.

## Notes

- Workouts are stored in the browser's `localStorage`, on-device only — they
  won't sync between your phone and any other device. Say the word if you'd
  like this switched to a synced backend later.
- Video links: paste a YouTube or Vimeo link when building a workout and it
  embeds inline. Other video sites fall back to a "Watch ↗" link that opens in
  a new tab.
