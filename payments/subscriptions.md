# Subscription Changes

**Label:** `Payments/Subscriptions`

**Gmail query:**

```text
{
  subject:"subscription will renew soon"
  subject:"subscription renewal"
  subject:"subscription price increase"
  subject:"subscription is expiring"
  subject:"subscription was canceled"
  subject:"subscription has been canceled"
  subject:"subscription will be canceled"

  (
    subject:subscription
    "renewing soon"
  )

  (
    subject:renewal
    subscription
  )

  (
    subject:membership
    {
      subject:renew
      subject:expiring
      subject:ended
      subject:change
    }
  )

  subject:"plan renewal"

  (
    subject:subscription
    subject:"price increase"
  )

  (
    subject:subscription
    subject:cost
  )

  (
    subject:subscription
    {
      subject:canceled
      subject:cancelled
    }
  )

  (
    subject:receipt
    subscription
    {
      renews
      renewed
      continues
    }
  )
}
-in:spam
-in:trash
```

**Actions:** Apply label `Payments/Subscriptions`.

**Description:** Identifies subscription and membership lifecycle notices such as renewals, expirations, recurring renewal receipts, price changes, and cancellations.
