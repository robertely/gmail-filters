# Payment Due Notices

**Label:** `Payments/Due`

**Gmail query:**

```text
{
  (subject:bill subject:due)
  (subject:invoice subject:due)
  (subject:payment subject:due)
}
-subject:paid
-subject:scheduled
-subject:ready
-subject:available
-in:spam
-in:trash
```

**Actions:** Apply label `Payments/Due`.

**Description:** Identifies bills, invoices, and payments that are due or approaching a payment deadline, while excluding paid, scheduled, and simple bill-availability notices.
