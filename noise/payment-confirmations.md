# Payment Confirmations

**Label:** `Noise/Payment Confirmations`

**Gmail query:**

```text
(subject:"payment received" OR subject:"payment is received" OR subject:"payment has been received" OR subject:"payment accepted" OR subject:"payment has been accepted" OR subject:"payment submitted" OR subject:"payment confirmation" OR subject:"payment receipt" OR subject:"payment success" OR subject:"thanks for your payment" OR subject:"thank you for your payment" OR (subject:"we've received your" subject:payment)) -subject:"payment request"
```

**Actions:** Apply label `Noise/Payment Confirmations`.

**Description:** Identifies successful payment acknowledgements and receipts while excluding payment requests.
