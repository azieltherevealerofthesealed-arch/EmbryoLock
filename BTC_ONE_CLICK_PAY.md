🔘 One-Click Pay Buttons (BTC)

These buttons open the user’s Bitcoin wallet pre-filled with the exact address + amount.

🟢 BASIC — One-Click Pay
<a
  href="bitcoin:bc1q8cg7hmgmu7x9yaja8j249np0vt84d4y8duugr7?amount=0.00001999"
  style="
    display:inline-block;
    padding:12px 20px;
    background:#00ff99;
    color:#000;
    font-weight:bold;
    border-radius:8px;
    text-decoration:none;
  "
>
  Pay for EmbryoLock Basic (BTC)
</a>

🔵 NEON — One-Click Pay
<a
  href="bitcoin:bc1q8cg7hmgmu7x9yaja8j249np0vt84d4y8duugr7?amount=0.00009017"
  style="
    display:inline-block;
    padding:12px 20px;
    background:#00ccff;
    color:#000;
    font-weight:bold;
    border-radius:8px;
    text-decoration:none;
  "
>
  Pay for EmbryoLock Neon (BTC)
</a>

🟣 STEALTH+ — One-Click Pay
<a
  href="bitcoin:bc1q8cg7hmgmu7x9yaja8j249np0vt84d4y8duugr7?amount=0.00014999"
  style="
    display:inline-block;
    padding:12px 20px;
    background:#cc66ff;
    color:#000;
    font-weight:bold;
    border-radius:8px;
    text-decoration:none;
  "
>
  Pay for EmbryoLock Stealth+ (BTC)
</a>

⚠️ IMPORTANT 
After payment, you MUST verify your transaction to unlock the download.

Verification step:
POST /check/{tier}

Example:
curl -X POST https://embryolock-pay.azieltherevealerofthesealed.workers.dev/check/neon \
  -H "Content-Type: application/json" \
  -d '{
    "chain": "btc",
    "txid": "YOUR_TRANSACTION_ID"
  }'
