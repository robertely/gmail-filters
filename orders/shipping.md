# Shipping Updates

**Label:** `Orders/Shipping`

**Gmail query:**

```text
{
  subject:shipped
  subject:"out for delivery"
  subject:"delivery update"
  subject:"delivery estimate update"

  (
    subject:delivered
    {
      subject:item
      subject:items
      subject:order
      subject:shipment
      subject:package
    }
  )

  (
    subject:"on the way"
    {
      subject:shipment
      subject:order
      subject:package
    }
  )

  (
    subject:shipment
    subject:order
    -subject:"awaiting shipment"
  )
}
-subject:"Re:"
-in:spam
-in:trash
```

**Actions:** Apply label `Orders/Shipping`.

**Description:** Identifies order shipping and delivery-status updates while excluding reply threads, Spam, and Trash.
