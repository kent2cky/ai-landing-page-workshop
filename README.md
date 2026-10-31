# Build Your Business Website with AI

**A free, step-by-step guide to creating and publishing a landing page for your business, with no coding.**

You'll use **Google AI Studio** to build the page by describing it in plain English, **GitHub** to store it, and **Vercel** to put it live on the internet. By the end you'll have a real link (like `your-shop.vercel.app`) you can share on WhatsApp, Instagram and Google.

> **Time needed:** 45–90 minutes the first time
> **Cost:** Free (a custom domain like `yourshop.com` is optional and paid)
> **Skill needed:** If you can fill a form and copy-paste, you can do this.

---

## Contents

0. [How it works](#how-it-works)
1. [Before you start (prerequisites)](#1-before-you-start-prerequisites)
2. [Step 1: Generate your page in Google AI Studio](#step-1-generate-your-page-in-google-ai-studio)
3. [Step 2: Refine it until you love it](#step-2-refine-it-until-you-love-it)
4. [Step 3: Run the pre-publish check](#step-3-run-the-pre-publish-check)
5. [Step 4: Save it to GitHub](#step-4-save-it-to-github)
6. [Step 5: Publish it on Vercel](#step-5-publish-it-on-vercel)
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
 │  Google AI Studio  │ ───► │    GitHub    │ ───► │    Vercel    │ ───► 🌍 Your live website
 │  (builds the page) │      │ (stores it)  │      │ (publishes)  │
 └────────────────────┘      └──────────────┘      └──────────────┘
```

- **Google AI Studio** is where you describe your website and Gemini (Google's AI) writes it for you.
- **GitHub** is like Google Drive for website code. Vercel reads your website from there.
- **Vercel** takes the code from GitHub and puts it on the internet for free. It works out the technical settings by itself, so publishing is mostly one click.

Once these three are connected, every change you make in AI Studio can go live in a couple of minutes.

> **About Vercel's free plan:** The free **Hobby** plan is meant for personal, non-commercial projects. It suits a simple personal page for a small shop. If your site later grows into a bigger commercial operation (online payments, a team, client work), look at [Vercel's plans](https://vercel.com/pricing) or another host.

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
- [ ] **A Vercel account**: go to [vercel.com/signup](https://vercel.com/signup), choose the **Hobby** (free, personal) plan, and click **Continue with GitHub**.
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

AI Studio can build big apps with servers and AI features. You only need a simple page, so this one prompt cleans the project up before you publish it.

1. Copy the prompt from [`prompts/03-pre-deploy-check.md`](prompts/03-pre-deploy-check.md).
2. Paste it into the AI Studio chat and send.
3. Read the reply. It should confirm the project builds with Vite into a folder called `dist`.
4. Check the preview still looks right.

> ✅ **Checkpoint:** AI Studio has confirmed the clean-up and your preview still works.

---

## Step 4: Save it to GitHub

1. In AI Studio, open **Settings** (the gear icon) and go to the **GitHub** tab.
   You may also see a GitHub icon or a **Save to GitHub** option near the top right of the Build screen.
2. Click to **connect your GitHub account**. A GitHub window opens: sign in and click **Authorize**.
3. Choose **Create a new repository**.
   - **Name:** use your business name with dashes, e.g. `glow-and-grace-salon`.
   - **Visibility:** **Public** or **Private** both work with Vercel. Private keeps your code hidden.
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

## Step 5: Publish it on Vercel

1. Go to **[vercel.com/new](https://vercel.com/new)** and sign in (use **Continue with GitHub**).
2. Under **Import Git Repository**, find your repository and click **Import**.
   - **Don't see it?** Click **Adjust GitHub App Permissions** (or **Configure GitHub App**), give Vercel access to that repository, then come back to this page.
3. On the next screen, check that **Framework Preset** says **Vite**. You don't need to change anything else.
   - The **Project Name** becomes your web address, so make it your shop's name, e.g. `glow-and-grace-salon`.
4. Click **Deploy**.
5. Wait 1–2 minutes. When you see **Congratulations!** and a picture of your site, it's live.
6. Click the picture (or **Continue to Dashboard** → **Visit**). Your link looks like `https://glow-and-grace-salon.vercel.app`. If that name was taken, Vercel adds a few extra characters.

> ✅ **Checkpoint:** Your website opens on your phone using the `vercel.app` link. Test the WhatsApp button from your phone too.

🎉 **You're live!** Share the link on your WhatsApp status, Instagram bio and Google Business Profile.

**Framework Preset doesn't say Vite?** Set **Framework Preset** to **Vite**. If you see build settings, they should be: Build Command `npm run build`, Output Directory `dist`.

---

## Step 6: Make changes later

Your site updates itself whenever GitHub changes:

1. Open your app in AI Studio: **Build** → find your project in your apps list.
2. Ask for changes in the chat as before.
3. Open **Settings → GitHub** and **push / sync** your changes. AI Studio writes the description of the change for you.
4. Vercel notices the change and republishes automatically. Refresh your site in 1–2 minutes.

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
| **My repository doesn't show up in Vercel** | Click **Adjust GitHub App Permissions** on the import page and give Vercel access to that repository. |
| **Vercel deployment failed** (red **Error**) | Open the deployment, click **Build Logs**, copy the red lines, and paste them into AI Studio using the prompt in [`03-pre-deploy-check.md`](prompts/03-pre-deploy-check.md#if-vercels-deployment-fails-later). Push to GitHub again. |
| **Site is live but the page is blank** | Run the [pre-publish check](prompts/03-pre-deploy-check.md) again and push to GitHub. In Vercel, check **Settings → Build and Deployment**: Framework Preset should be **Vite** and Output Directory `dist`. |
| **WhatsApp button opens the wrong number / error** | The number must be international format, no `+`, no spaces, no leading `0`: `https://wa.me/2348012345678`. |
| **My changes aren't showing on the live site** | Check you pushed to GitHub (Step 6), then look at the **Deployments** tab in Vercel for a new deployment. Hard-refresh your browser (Ctrl+Shift+R / Cmd+Shift+R). |

**Still stuck?** In AI Studio you can describe the problem in plain English, or paste a screenshot, and ask Gemini to explain what's wrong.

### Plan B: publish straight from AI Studio

If Vercel isn't working for you, AI Studio has its own **Publish** button (top right of Build mode). Eligible personal Google accounts can publish up to **two apps for free** without adding a card, and you can pick a link like `your-name.ai.studio`. Some accounts aren't eligible and will be asked to set up billing; if that happens, stick with Vercel. [Read Google's deployment guide](https://ai.google.dev/gemini-api/docs/aistudio-deploying).

---

## Optional next steps

- **Get your own domain** (e.g. `glowandgrace.com.ng`): buy one from a domain registrar, then follow [Vercel's custom domain guide](https://vercel.com/docs/domains/set-up-custom-domain). HTTPS is set up for you.
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
- [Deploying on Vercel](https://vercel.com/docs/getting-started-with-vercel): Vercel's getting-started guide
- [Vercel can't find my GitHub repository](https://vercel.com/kb/guide/unable-to-find-github-repository): fix for repositories missing on the import page
- [Vercel custom domains](https://vercel.com/docs/domains/set-up-custom-domain): connect your own domain name

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
- [ ] I know how to make changes (AI Studio → push to GitHub → Vercel republishes)

---

*Workshop: Build Your Business Website with AI. Guide current as of October 2026. Google, GitHub and Vercel update their screens often; if a button has moved, look for one with similar wording.*
