# Scheduled Payments

**Label:** `Payments/Scheduled`

**Gmail query:**

```text
{
  subject:"automatic payment"
  subject:"automated payment"
  subject:"upcoming payment"
  subject:"payment is scheduled"
  subject:"payment scheduled"
  subject:"scheduled payment"
  subject:"scheduled for payment"
  (subject:payment subject:"will process soon")
  (subject:payment subject:"will be processed soon")
}
-subject:"set up"
-subject:enrolled
-subject:received
-subject:successful
-subject:failed
-subject:declined
-subject:canceled
-subject:cancelled
-subject:changed
-in:spam
-in:trash
```

**Actions:** Apply label `Payments/Scheduled`.

**Description:** Identifies notices that an automatic or scheduled payment is upcoming, while excluding enrollment, completion, failure, cancellation, and change notices.
