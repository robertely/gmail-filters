# Orders Placed

**Label:** `Orders/Placed`

**Gmail query:**

```text
(
  subject:ordered
  OR subject:"order received"
  OR subject:"order confirmed"
  OR subject:"order is confirmed"
  OR subject:"order has been confirmed"
  OR (subject:order subject:confirmed)
  OR subject:"thanks for your order"
  OR (subject:"thanks for your" subject:order)
  OR subject:"thank you for your order"
  OR subject:"we got your order"
  OR subject:"order placed"
  OR subject:"new order"
  OR subject:"purchase confirmation"
  OR subject:"order confirmation"
  OR subject:"order of"
  OR (subject:order "thank you for placing your order")
)
-subject:"Re:"
-subject:shipped
-subject:shipment
-subject:"out for delivery"
-subject:delivered
-subject:"on the way"
-subject:payment
-"transaction type sale"
-in:spam
-in:trash
```

**Actions:** Apply label `Orders/Placed`.

**Description:** Identifies order-placement and purchase-confirmation messages while excluding shipping-status updates, payment-only messages, replies, Spam, and Trash.
