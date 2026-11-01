# Rare Crystal Salon AI Review Writer

A mobile-first, QR-friendly Vercel website. Customers describe their genuine salon experience; Gemini drafts a review for them to check, copy, and voluntarily submit to Google.

## Deploy to Vercel

1. Import this GitHub repository into Vercel, or use the Vercel project linked to this repository.
2. In Project Settings → Environment Variables, add:
   - `GEMINI_API_KEY`: a Google AI Studio API key. Store it only as an encrypted/sensitive environment variable in Vercel.
   - Optional: `GEMINI_MODEL`: defaults to `gemini-2.5-flash`.
3. Apply the variable to Production and Preview as required, then redeploy.
4. Test the customer flow on a phone.

## Important

- Never commit API keys, paste them into frontend code, or share them in chat.
- If a key has been exposed, revoke it and create a replacement before use.
- Google review link uses the confirmed salon Place ID configured in `index.html`.
- Customers must read/edit, choose their Google star rating and submit themselves. This app does not submit reviews.
- The draft must accurately reflect the customer's own experience. Do not filter by sentiment or offer incentives for positive reviews.
- The project does not store customer feedback or include tracking analytics.
- After the production deployment is ready, create a QR code pointing to that site's public URL, not directly to the Google review form.
