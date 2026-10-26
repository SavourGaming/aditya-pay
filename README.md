# Savour Gaming Tipping Page

A cyan gaming-themed UPI tipping page, hosted free on GitHub Pages.

**Live link:** https://savourgaming.github.io/aditya-pay/

## Features
- Quick amounts (₹50, ₹100, ₹200, ₹500) and a custom amount (₹1 to ₹1,00,000)
- QR code that updates with the amount and UPI ID (works on PC)
- Mobile: Google Pay, PhonePe, Paytm and BHIM buttons open that app directly, plus "Other UPI app"
- Message if the chosen app is not installed
- No server, no API keys, nothing is stored

## Setup (so the link is `savourgaming.github.io/aditya-pay/`)
1. The repository name decides the link. It must be exactly `aditya-pay` under the `SavourGaming` account, and it must be **Public**.
   - Existing repository? Go to **Settings → General → Repository name**, type `aditya-pay` and click **Rename**.
2. Make sure `index.html` is in the repository root (not inside a folder) and named in lowercase.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait 1 to 2 minutes. The link above will open the page directly.

## Change details
Edit the `EDIT HERE` block near the bottom of `index.html`:

```js
const UPI_ID  = "s.adityachaurasiya@fam";
const NAME    = "Aditya";
const CHANNEL = "SAVOUR GAMING";
const AMOUNTS = [50, 100, 200, 500];
```

## Payment notes
- Verify the UPI ID and the name shown in your own UPI app before sharing the link.
- The QR is created inside the browser with the `qrcodejs` library from cdnjs. It needs an internet connection.
- App deep links vary by phone and app. If one does not open, use another app button or scan the QR.
- GitHub Pages is static hosting. This page does **not** verify payments or confirm tips. Money goes straight from the supporter's UPI app to your UPI ID.
- Nothing is paid automatically. The supporter chooses an amount and approves it in their UPI app.
