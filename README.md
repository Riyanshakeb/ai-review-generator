# Rare Crystal Salon AI Review Writer

A mobile-first, QR-friendly Vercel website. Customers describe their genuine salon experience; AI drafts a review for them to check, copy, and voluntarily submit to Google.

## Deploy
1. Import this GitHub repository into Vercel.
2. In Vercel Project Settings → Environment Variables, add OPENAI_API_KEY with your secret OpenAI API key.
3. Optionally set OPENAI_MODEL to a model enabled for your API account. The source defaults to gpt-6; change it if unavailable to your account.
4. Redeploy after setting variables.
5. Test the customer flow on a phone.

## Important
- Google review link uses the confirmed salon Place ID configured in index.html.
- Customers must read/edit, choose their Google star rating and submit themselves. This app does not submit reviews.
- The draft must accurately reflect the customer's own experience. Do not filter by sentiment or offer incentives for positive reviews.
- The project does not store customer feedback or include tracking analytics.
- After Vercel deployment, create a QR code to the deployed website URL, not the direct Google link.
