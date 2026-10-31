# Prompt 1: The Starter Prompt

Paste this into the prompt box in **Google AI Studio → Build**.

**Before you paste:** replace everything in `[SQUARE BRACKETS]` with details from your [Business Info Sheet](../templates/business-info-sheet.md). Delete any line that doesn't apply to you.

Keep the **IMPORTANT TECHNICAL RULES** section exactly as it is. It's what makes your site free and easy to publish.

> Want to see it filled in? Look at the [salon example](../example/salon-example.md#filled-in-starter-prompt).

---

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
- Business name: [YOUR BUSINESS NAME]
- What we do: [ONE SENTENCE]
- Our customers: [WHO YOUR CUSTOMERS ARE]
- What makes us different: [YOUR SELLING POINTS]
- Area we serve: [CITY / AREAS]

SERVICES AND PRICES:
- [SERVICE 1]: [SHORT DESCRIPTION]. [PRICE]
- [SERVICE 2]: [SHORT DESCRIPTION]. [PRICE]
- [SERVICE 3]: [SHORT DESCRIPTION]. [PRICE]

CONTACT DETAILS:
- WhatsApp: [NUMBER IN INTERNATIONAL FORMAT, e.g. 2348012345678]
- Phone: [PHONE]
- Email: [EMAIL]
- Address: [ADDRESS, or delete this line]
- Opening hours: [HOURS]
- Instagram: [FULL LINK]
- Facebook: [FULL LINK]

LOOK AND FEEL:
- Colors: [YOUR BRAND COLORS]
- Mood: [e.g. elegant, playful, bold, calm]

MAIN ACTION:
The main button everywhere should be "[BUTTON TEXT, e.g. Chat on WhatsApp]".
It must open https://wa.me/[YOUR WHATSAPP NUMBER]

PAGE SECTIONS (in this order):
1. Top bar with business name and the main button
2. Hero section: a strong headline, a one-line description, and the main button
3. About us
4. Services or products with prices, shown as cards
5. Photo gallery (use tasteful placeholder images for now; I'll add my own photos later)
6. Why choose us (3–4 short points)
7. Opening hours and location
8. Contact section
9. Footer with copyright and social links

Do not invent customer reviews, awards, or statistics.
Also add a floating WhatsApp button at the bottom-right corner on every screen size.
```

---

## Tips

- **Have real reviews?** Add a section to the list: `Customer reviews, using exactly these: "..." – Name`.
- **Don't use WhatsApp?** Change the MAIN ACTION to a phone link (`tel:+234...`), an email link (`mailto:you@email.com`) or your Instagram link, and delete the floating WhatsApp line.
- **Sell products?** Rename "Services" to "Products" and describe each item.
- **Prefer not to show prices?** Delete them and add: `Show "Contact us for pricing" instead of prices.`
