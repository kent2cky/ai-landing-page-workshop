# Prompt 3: Pre-Publish Check

Send this **once**, right before you connect GitHub. It makes sure your project will build cleanly on Render.

```text
I'm about to publish this website as a static site on Render. Please check and fix the project so that:

1. It is frontend only, with no backend server code, no server.ts/server.js files, and no API keys or Gemini API calls. If any exist, remove them and remove anything in package.json that is only needed for them.
2. package.json has a "build" script that runs "vite build", and the finished site is created in the "dist" folder.
3. All images and files the page uses are included in the project (no links to files that only exist inside AI Studio).
4. All WhatsApp, phone, email and social media links are correct.
5. There are no build or TypeScript errors.

When you're done, tell me in one short list what you changed. Also confirm the Build Command and Publish Directory I should type into Render.
```

## What you should hear back

AI Studio should confirm something like:

- **Build Command:** `npm install && npm run build`
- **Publish Directory:** `dist`

If it gives you different values, use the ones it gives you in the Render step instead.

## If Render's build fails later

Copy the red error lines from Render's **Logs**, then send:

```text
My Render static site build failed with this error. Please fix the project so "npm install && npm run build" works and outputs to "dist":

[PASTE THE ERROR HERE]
```

Then sync to GitHub again. Render will rebuild automatically.
