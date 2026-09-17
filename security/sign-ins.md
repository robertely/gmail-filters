# Sign-in Alerts

**Label:** `Security/Sign-ins`

**Gmail query:**

```text
{
  subject:"new sign-in"
  subject:"new sign in"
  subject:"new login"
  subject:"login detected"
  subject:"sign-in detected"
  subject:"sign-in alert"
  subject:"sign-in notification"
  subject:"login alert"
  subject:"sign-in from new location"
  subject:"login from a new device"
  subject:"sign in from a new device"
  subject:"signed in with a new device"
  subject:"new device logged in"
  subject:"a new device is using your account"
  (
    subject:"log in"
    subject:"new device"
  )
  (
    subject:"security alert"
    "new sign-in"
  )
}
-in:spam
-in:trash
```

**Actions:** Apply label `Security/Sign-ins`.

**Description:** Identifies account sign-in and new-device security notifications while avoiding broader security notices that are not about a login.
