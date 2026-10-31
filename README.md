# Build Your Business Website with AI

**A free, step-by-step guide to creating and publishing a landing page for your business, with no coding.**

You'll use **Google AI Studio** to build the page by describing it in plain English, **GitHub** to store it, and **Render** to put it live on the internet. By the end you'll have a real link (like `your-business.onrender.com`) you can share on WhatsApp, Instagram and Google.

> **Time needed:** 45–90 minutes the first time
> **Cost:** Free (a custom domain like `yourbusiness.com` is optional and paid)
> **Skill needed:** If you can fill a form and copy-paste, you can do this.

---

## Contents

0. [How it works](#how-it-works)
1. [Before you start (prerequisites)](#1-before-you-start-prerequisites)
2. [Step 1: Generate your page in Google AI Studio](#step-1-generate-your-page-in-google-ai-studio)
3. [Step 2: Refine it until you love it](#step-2-refine-it-until-you-love-it)
4. [Step 3: Run the pre-publish check](#step-3-run-the-pre-publish-check)
5. [Step 4: Save it to GitHub](#step-4-save-it-to-github)
6. [Step 5: Publish it on Render](#step-5-publish-it-on-render)
7. [Step 6: Make changes later](#step-6-make-changes-later)
8. [Troubleshooting](#troubleshooting)
9. [Optional next steps](#optional-next-steps)
10. [Helpful resources](#helpful-resources)
11. [Final checklist](#final-checklist)

**Files in this repo:**

| File | What it's for |
|---|---|
| [`templates/business-info-sheet.md`](templates/business-info-sheet.md) | Fill this in first: your business details |
| [`prompts/01-starter-prompt.md`](prompts/01-starter-prompt.md) | The main prompt that builds your page |
| [`prompts/02-refine-prompts.md`](prompts/02-refine-prompts.md) | Follow-up prompts to polish it |
| [`prompts/03-pre-deploy-check.md`](prompts/03-pre-deploy-check.md) | The check to run before publishing |
| [`example/salon-example.md`](example/salon-example.md) | The salon used in the live demo, fully filled in |

---

## How it works

```
 ┌────────────────────┐      ┌──────────────┐      ┌──────────────┐
 │  Google AI Studio  │ ───► │    GitHub    │ ───► │    Render    │ ───► 🌍 Your live website
 │  (builds the page) │      │ (stores it)  │      │ (publishes)  │
 └────────────────────┘      └──────────────┘      └──────────────┘
```

- **Google AI Studio** is where you describe your website and Gemini (Google's AI) writes it for you.
- **GitHub** is like Google Drive for website code. Render reads your website from there.
- **Render** takes the code from GitHub and puts it on the internet for free.

Once these three are connected, every change you make in AI Studio can go live in a couple of minutes.

> **Why Render and not Vercel?** Vercel's free plan is for personal, non-commercial projects only. A business website is commercial. Render's free static site hosting doesn't have that restriction.

---

## 1. Before you start (prerequisites)

### ✅ Equipment

- [ ] A **laptop or desktop computer**. This doesn't work well on a phone.
- [ ] **Google Chrome** browser (other browsers work, but Chrome is what this guide uses).
- [ ] A stable internet connection.

### ✅ Accounts (all free)

Create these **before** you start building. Email verification can take a few minutes.

- [ ] **A personal Google account** (a regular `@gmail.com` works best).
  Work or school Google accounts sometimes have AI Studio switched off by the administrator.
- [ ] **A GitHub account**: sign up at [github.com/signup](https://github.com/signup).
  You can choose **Continue with Google** to make it faster. **Verify your email**: GitHub won't let you create projects until you do.
- [ ] **A Render account**: go to [render.com](https://render.com), click **Get Started**, and choose **Sign up with GitHub**.
  Signing up with GitHub saves a step later.

### ✅ Your business content

- [ ] Fill in the [**Business Info Sheet**](templates/business-info-sheet.md).
- [ ] Put your **logo** and **3–6 photos** in one folder on your computer (optional but strongly recommended).
- [ ] Know your **WhatsApp number in international format**: country code + number, **no** `+`, spaces or leading `0`.
  Example: `0801 234 5678` in Nigeria becomes `2348012345678`.

---

## Step 1: Generate your page in Google AI Studio

1. Go to **[aistudio.google.com](https://aistudio.google.com)** and sign in with your Google account.
   If it's your first time, accept the terms.
2. Click **Build** in the left menu (or go straight to [aistudio.google.com/apps](https://aistudio.google.com/apps)).
3. Open [`prompts/01-starter-prompt.md`](prompts/01-starter-prompt.md) and copy the prompt.
4. Paste it into a notes app first and **replace every `[SQUARE BRACKET]`** with your business details.
5. Paste your finished prompt into the big prompt box in AI Studio and press **Run** (or **Build**).
6. Wait 1–3 minutes. You'll see files being written, then your website appears in the **preview** on the right.

> ✅ **Checkpoint:** You can see a website with your business name, your services and a WhatsApp button in the preview panel.

**Tips**

- Don't worry if the first version isn't perfect. That's what Step 2 is for.
- AI results vary every time. Two people with the same prompt will get different designs, and that's normal.
- Google updates AI Studio often, so buttons may look slightly different from this guide. Look for similar words.

---

## Step 2: Refine it until you love it

Use the **chat box on the left** to ask for changes in plain English. Ready-made prompts are in [`prompts/02-refine-prompts.md`](prompts/02-refine-prompts.md).

### Things to check

- [ ] Business name, phone, email and address are spelled **exactly right**
- [ ] Prices are correct
- [ ] Every WhatsApp button opens a chat with **your** number (click it in the preview to test)
- [ ] It looks good on mobile. Use the device toggle in the preview, if available, or make your browser window narrow.
- [ ] No made-up reviews, awards or numbers

### Adding your own photos

1. Click the **+** (Add files) button in the chat box.
2. Upload your logo and photos.
3. Send the "Add your own photos" prompt from [`02-refine-prompts.md`](prompts/02-refine-prompts.md#add-your-own-photos).

### Point-and-change (annotation mode)

Can't describe what you want? Turn on **annotation mode** in the preview, highlight the part of the page you want changed, and type what you want, like "make this button bigger".

### Golden rules

1. **One or two changes per message.** Then check the preview.
2. **Be specific.** "Make the services section cards bigger with gold borders" beats "make it nicer".
3. **If it breaks, ask it to undo:** "Undo your last change."

> ✅ **Checkpoint:** You're happy with how the page looks on both mobile and laptop.

---

## Step 3: Run the pre-publish check

AI Studio can build big apps with servers and AI features. You only need a simple static page, so this one prompt cleans the project up before you publish it.

1. Copy the prompt from [`prompts/03-pre-deploy-check.md`](prompts/03-pre-deploy-check.md).
2. Paste it into the AI Studio chat and send.
3. Read the reply. Note down the **Build Command** and **Publish Directory** it confirms. They should be:

| Setting | Value |
|---|---|
| Build Command | `npm install && npm run build` |
| Publish Directory | `dist` |

4. Check the preview still looks right.

> ✅ **Checkpoint:** AI Studio has confirmed the build settings and your preview still works.

---

## Step 4: Save it to GitHub

1. In AI Studio, open **Settings** (the gear icon) and go to the **GitHub** tab.
   You may also see a GitHub icon or a **Save to GitHub** option near the top right of the Build screen.
2. Click to **connect your GitHub account**. A GitHub window opens: sign in and click **Authorize**.
3. Choose **Create a new repository**.
   - **Name:** use your business name with dashes, e.g. `glow-and-grace-salon`.
   - **Visibility:** **Public** or **Private** both work with Render. Private keeps your code hidden.
4. Confirm. AI Studio pushes (uploads) your project to GitHub.
5. Open [github.com](https://github.com), click your profile picture → **Your repositories**, and click your new repository.

> ✅ **Checkpoint:** On GitHub you can see a list of files including `package.json`, `index.html` and a `src` folder.

**Backup route (if the GitHub connection won't work):**

1. In AI Studio, use the **Download** option to get your project as a **ZIP file**.
2. Unzip it on your computer.
3. On GitHub, click **+** (top right) → **New repository** → name it → **Create repository**.
4. On the new repository page, click **uploading an existing file**.
5. Drag **everything inside** the unzipped folder (not the folder itself) into the upload box. Skip any `node_modules` folder if there is one.
6. Click **Commit changes**.

---

## Step 5: Publish it on Render

1. Go to **[dashboard.render.com](https://dashboard.render.com)** and sign in (use **GitHub**).
   If asked to create a workspace or pick a plan, choose the **free / Hobby** option.
2. Click **+ New** (top right) → **Static Site**.
3. Under **Connect a repository**, find your repository and click **Connect**.
   - **Don't see it?** Click **Configure GitHub** / **Configure account**, choose **All repositories** (or select yours), and click **Save**. Then return to Render.
4. Fill in the settings:

| Field | What to type |
|---|---|
| **Name** | Your business name, e.g. `glow-and-grace-salon`. This becomes part of your link. |
| **Branch** | `main` (leave as is) |
| **Root Directory** | Leave **empty** |
| **Build Command** | `npm install && npm run build` |
| **Publish Directory** | `dist` |

5. Click **Create Static Site** (or **Deploy Static Site**).
6. Watch the logs. After 1–3 minutes you'll see **Your site is live** / a green **Live** label.
7. Click the link at the top of the page. It looks like `https://glow-and-grace-salon.onrender.com`. If that name was taken, Render adds a few extra characters.

> ✅ **Checkpoint:** Your website opens on your phone using the `onrender.com` link. Test the WhatsApp button from your phone too.

🎉 **You're live!** Share the link on your WhatsApp status, Instagram bio and Google Business Profile.

---

## Step 6: Make changes later

Your site updates itself whenever GitHub changes:

1. Open your app in AI Studio: **Build** → find your project in your apps list.
2. Ask for changes in the chat as before.
3. Open **Settings → GitHub** and **push / sync** your changes. AI Studio writes the description of the change for you.
4. Render notices the change and rebuilds automatically. Refresh your site in 2–3 minutes.

> **Tip:** Change prices, add a new service, or swap photos any time you like. No developer needed.

---

## Troubleshooting

| Problem | What to do |
|---|---|
| **AI Studio says I can't access it** | Use a personal `@gmail.com` account, not a work or school one. |
| **AI Studio says I've hit a limit / quota** | Free usage has limits. Wait a while (or until tomorrow) and continue. Your app is saved. |
| **The preview is blank or shows an error** | Type in the chat: `The preview is showing an error. Please fix any build issues with the current code.` |
| **The AI changed things I didn't ask for** | Type: `Undo your last change.` Then ask again, more specifically. |
| **GitHub verification email hasn't arrived** | Check spam/promotions. Resend from GitHub's settings. |
| **My repository doesn't show up in Render** | In Render, click **Configure GitHub**/**Configure account** and give Render access to that repository. |
| **Render build failed** (red **Failed** label) | Open **Logs**, copy the red error lines, and paste them into AI Studio using the "If Render's build fails" prompt in [`03-pre-deploy-check.md`](prompts/03-pre-deploy-check.md#if-renders-build-fails-later). Push to GitHub again. |
| **Site is live but the page is blank** | Run the [pre-publish check](prompts/03-pre-deploy-check.md) again, push to GitHub, and wait for Render to rebuild. Double-check the **Publish Directory** in Render (Settings) is `dist`. |
| **WhatsApp button opens the wrong number / error** | The number must be international format, no `+`, no spaces, no leading `0`: `https://wa.me/2348012345678`. |
| **My changes aren't showing on the live site** | Check you pushed to GitHub (Step 6), then look in Render's **Events** tab for a new deploy. Hard-refresh your browser (Ctrl+Shift+R / Cmd+Shift+R). |

**Still stuck?** In AI Studio you can describe the problem in plain English, or paste a screenshot, and ask Gemini to explain what's wrong.

### Plan B: publish straight from AI Studio

If Render isn't working for you, AI Studio has its own **Publish** button (top right of Build mode). Eligible personal Google accounts can publish up to **two apps for free** without adding a card, and you can pick a link like `your-name.ai.studio`. Some accounts aren't eligible and will be asked to set up billing; if that happens, stick with Render. [Read Google's deployment guide](https://ai.google.dev/gemini-api/docs/aistudio-deploying).

---

## Optional next steps

- **Get your own domain** (e.g. `glowandgrace.com.ng`): buy one from a domain registrar, then follow [Render's custom domain guide](https://render.com/docs/custom-domains). Render's free Hobby workspace includes 2 custom domains with free HTTPS.
- **Get found on Google Maps:** create a free [Google Business Profile](https://www.google.com/business/) and add your new website link.
- **Add your link everywhere:** WhatsApp Business profile, Instagram bio, Facebook page, email signature, flyers (make a QR code for it).
- **Check your speed:** paste your link into [PageSpeed Insights](https://pagespeed.web.dev) to see how fast it loads on mobile.
- **Ask customers for reviews,** then add the real ones to your page with a refine prompt.

---

## Helpful resources

### The tools

- [Google AI Studio](https://aistudio.google.com): where you build
- [AI Studio Build mode docs](https://ai.google.dev/gemini-api/docs/aistudio-build-mode): Google's official guide to Build mode, GitHub sync and annotation mode
- [AI Studio troubleshooting](https://ai.google.dev/gemini-api/docs/troubleshoot-ai-studio): fixes for common AI Studio problems
- [Publishing from AI Studio](https://ai.google.dev/gemini-api/docs/aistudio-deploying): the Plan B route
- [Creating a GitHub account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github): GitHub's official sign-up guide
- [Render static sites](https://render.com/docs/static-sites): Render's official static site guide
- [Render custom domains](https://render.com/docs/custom-domains): connect your own domain name

### Better prompts

- [Google's prompting guide](https://ai.google.dev/gemini-api/docs/prompting-strategies): how to write clearer instructions for Gemini

### Content and design

- [Unsplash](https://unsplash.com) and [Pexels](https://www.pexels.com): free stock photos (check each photo's license)
- [Canva](https://www.canva.com): design a simple logo or edit photos
- [Coolors](https://coolors.co): pick a color palette and get the color codes
- [Favicon.io](https://favicon.io): turn your logo into a browser tab icon

### WhatsApp

- [How to create a WhatsApp click-to-chat link (Techpoint Africa)](https://techpoint.africa/guide/how-to-create-whatsapp-link/): includes a Nigerian number example and pre-filled messages

---

## Final checklist

- [ ] My site opens on my phone using the live link
- [ ] Business name, phone, email, address and prices are correct
- [ ] Every WhatsApp/call button reaches me
- [ ] Social media links open the right pages
- [ ] No fake reviews or made-up numbers
- [ ] I've shared the link on WhatsApp, Instagram and my Google Business Profile
- [ ] I know how to make changes (AI Studio → push to GitHub → Render rebuilds)

---

*Workshop: Build Your Business Website with AI. Guide current as of October 2026. Google, GitHub and Render update their screens often; if a button has moved, look for one with similar wording.*
