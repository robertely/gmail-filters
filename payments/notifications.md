# Payment Notifications

**Label:** `Payments/Notifications`

**Gmail query:**

```text
{
  (
    subject:bill
    {
      subject:ready
      subject:available
    }
  )

  (
    subject:"billing document"
    available
  )
}
-in:spam
-in:trash
```

**Actions:** Apply label `Payments/Notifications`.

**Description:** Identifies notices that a bill or billing document is ready or available to view, without treating the notice itself as a payment-due or payment-confirmation message.
