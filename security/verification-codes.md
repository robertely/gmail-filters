# Verification Code Mail

**Label:** `Security/Verification Codes`

**Gmail query:**

```text
{
  subject:"verification code"
  subject:"login code"
  subject:"security code"
  subject:"one-time passcode"
  subject:"one time passcode"
  subject:OTP
  subject:"access code"
  subject:"single-use code"
  subject:"single use code"
  subject:"login PIN"
  subject:"two-factor sign in code"
  subject:"two-factor sign-in code"
}
-in:spam
-in:trash
```

**Actions:** Apply label `Security/Verification Codes`.

**Description:** Organizes one-time code messages used during account access or identity checks.
