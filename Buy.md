🔐 EmbryoLock — How to Buy (Crypto Only)

No account.
No email.
No recovery.
Pay → Verify → Download.

🚀 One-Click Pay (Recommended)

Click the tier you want:

Basic (BTC)
👉 https://embryolock-pay.azieltherevealerofthesealed.workers.dev/pay/basic?chain=btc

Neon (BTC)
👉 https://embryolock-pay.azieltherevealerofthesealed.workers.dev/pay/neon?chain=btc

Stealth+ (BTC)
👉 https://embryolock-pay.azieltherevealerofthesealed.workers.dev/pay/stealth?chain=btc

Each link:

Shows exact amount

Shows exact address

Cannot be misconfigured

🧾 What You’ll See After Clicking

Example response:

{
  "tier": "neon",
  "chain": "btc",
  "pay_to": "bc1q8cg7hmgmu7x9yaja8j249np0vt84d4y8duugr7",
  "amount": "9017",
  "unit": "sats"
}


Send exactly that amount to that address.

💸 Step 1 — Pay

From any Bitcoin wallet:

Send the shown amount

To the shown address

Wait for the transaction hash (TXID)

⚠️ Partial payments will not unlock.

✅ Step 2 — Verify Payment (Required)

After payment, verify it by sending your transaction hash.

One-Click Verify (copy & paste)

Replace PASTE_TXID_HERE with your real TXID:

curl -X POST https://embryolock-pay.azieltherevealerofthesealed.workers.dev/check/neon \
  -H "Content-Type: application/json" \
  -d '{
    "chain": "btc",
    "txid": "PASTE_TXID_HERE"
  }'


You must include "chain": "btc".

🎁 Step 3 — Download

If payment is valid, you’ll receive:

{
  "ok": true,
  "redeem_url": "/redeem?token=XXXXXXXX"
}


Open the redeem link in your browser to download your file.

⏳ Links expire after 30 minutes.
🔒 Each token is single-use.

❗ Important Notes (Read This)

There is no password recovery

There is no support email

There are no refunds

If you forget to verify payment, nothing unlocks

This is intentional

EmbryoLock is designed for people who understand finality.

🧠 FAQ

Q: Can I pay without clicking the link?
Yes — but the link prevents mistakes.

Q: What if I send the wrong amount?
It will not unlock.

Q: What if I forget to verify?
The system does nothing until verification.

Q: Is this anonymous?
Yes. No accounts. No tracking.

✅ TL;DR (Fast Path)

Click tier link

Pay exact amount

POST TXID

Download

Done
