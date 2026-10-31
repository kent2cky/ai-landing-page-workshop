# Prompt 3: Pre-Publish Check

Send this **once**, right before you connect GitHub. It makes sure your project will publish cleanly on Vercel.

```text
I'm about to publish this website on Vercel as a simple static site. Please check and fix the project so that:

1. It is frontend only, with no backend server code, no server.ts/server.js files, and no API keys or Gemini API calls. If any exist, remove them and remove anything in package.json that is only needed for them.
2. It is a standard Vite project: package.json has a "build" script that runs "vite build", and the finished site is created in the "dist" folder.
3. All images and files the page uses are included in the project (no links to files that only exist inside AI Studio).
4. All WhatsApp, phone, email and social media links are correct.
5. There are no build or TypeScript errors.

When you're done, tell me in one short list what you changed.
```

## What you should hear back

A short list of changes, and a confirmation that the project builds with Vite into the `dist` folder. That's what Vercel looks for, so you won't need to type any settings when you deploy.

## If Vercel's deployment fails later

Open the failed deployment in Vercel, click **Build Logs**, copy the red error lines, then send:

```text
My Vercel deployment failed with this error. Please fix the project so it builds with "npm run build" into the "dist" folder:

[PASTE THE ERROR HERE]
```

Then push to GitHub again. Vercel will try again automatically.
