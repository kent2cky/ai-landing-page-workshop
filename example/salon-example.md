# Worked Example: Glow & Grace Salon

This is the sample business used in the live demo. It's a made-up salon, so the phone number and address are placeholders.

Use it to see what a completed [Business Info Sheet](../templates/business-info-sheet.md) and a filled-in [Starter Prompt](../prompts/01-starter-prompt.md) look like.

---

## Completed Business Info Sheet

**Business name:** Glow & Grace Salon

**What we do:** Hair styling, braids, nails and bridal makeup in Lekki, Lagos.

**Customers:** Busy professional women aged 25–45 and brides-to-be.

**What makes us different:** Home service available across Lekki and Ajah, 10 years' experience, and we only use products that are gentle on natural hair.

**Area served:** Lekki, Ajah, Victoria Island (Lagos)

**Services:**

| Service | Description | Price |
|---|---|---|
| Knotless braids | Medium length, neat and lightweight | ₦35,000 |
| Silk press | Wash, treatment and silk press for natural hair | ₦20,000 |
| Gel manicure | Long-lasting gel polish with nail care | ₦12,000 |
| Bridal makeup | Trial session plus wedding-day glam | ₦150,000 |
| Home service | We come to you (Lekki to Ajah) | From ₦10,000 extra |

**WhatsApp:** 2348000000000 *(placeholder)*

**Phone:** 0800 000 0000 *(placeholder)*

**Email:** hello@glowandgrace.example

**Address:** 12 Example Street, Lekki Phase 1, Lagos *(placeholder)*

**Opening hours:** Tue–Sat 9am–7pm, Sun 1pm–6pm, closed Mondays

**Instagram:** instagram.com/glowandgrace.example *(placeholder)*

**Brand colors:** Soft blush pink, warm gold and off-white

**Mood:** Elegant, warm, luxurious

**Main action:** Chat on WhatsApp to book

**Reviews:** None yet (section skipped)

**Photos:** Using free stock photos for the demo.

---

## Filled-in Starter Prompt

This is exactly what gets pasted into Google AI Studio during the demo:

```text
Build me a one-page landing page website for my business.

IMPORTANT TECHNICAL RULES (follow these exactly):
- This must be a simple static website: frontend only.
- Do NOT use the Gemini API or any AI features inside the website.
- Do NOT add a backend server, database, login, or API keys.
- Use React with Vite and Tailwind CSS.
- Running "npm run build" must create the finished website in a folder called "dist".
- The page must look great on mobile phones first, then on laptops.

ABOUT MY BUSINESS:
- Business name: Glow & Grace Salon
- What we do: Hair styling, braids, nails and bridal makeup in Lekki, Lagos.
- Our customers: Busy professional women aged 25–45 and brides-to-be.
- What makes us different: Home service across Lekki and Ajah, 10 years' experience, products that are gentle on natural hair.
- Area we serve: Lekki, Ajah, Victoria Island (Lagos)

SERVICES AND PRICES:
- Knotless braids: medium length, neat and lightweight. ₦35,000
- Silk press: wash, treatment and silk press for natural hair. ₦20,000
- Gel manicure: long-lasting gel polish with nail care. ₦12,000
- Bridal makeup: trial session plus wedding-day glam. ₦150,000
- Home service: we come to you (Lekki to Ajah). From ₦10,000 extra

CONTACT DETAILS:
- WhatsApp: 2348000000000
- Phone: 0800 000 0000
- Email: hello@glowandgrace.example
- Address: 12 Example Street, Lekki Phase 1, Lagos
- Opening hours: Tue–Sat 9am–7pm, Sun 1pm–6pm, closed Mondays
- Instagram: https://instagram.com/glowandgrace.example

LOOK AND FEEL:
- Colors: soft blush pink, warm gold and off-white
- Mood: elegant, warm, luxurious

MAIN ACTION:
The main button everywhere should be "Book on WhatsApp". It must open
https://wa.me/2348000000000?text=Hi%20Glow%20%26%20Grace%2C%20I%27d%20like%20to%20book%20an%20appointment

PAGE SECTIONS (in this order):
1. Top bar with business name and a "Book on WhatsApp" button
2. Hero section: a strong headline, a one-line description, and the main button
3. About us
4. Services with prices, shown as cards
5. Photo gallery (use tasteful placeholder images for now; I'll add my own photos later)
6. Why choose us (3–4 short points)
7. Opening hours and location
8. Contact section with WhatsApp, phone, email and Instagram
9. Footer with copyright and social links

Do not invent customer reviews, awards, or statistics.
Also add a floating WhatsApp button at the bottom-right corner on every screen size.
```
