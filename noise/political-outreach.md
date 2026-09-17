# Political Outreach

**Label:** `Noise/Political Outreach`

**Gmail query:**

```text
(
  from:(mail.house.gov)
  OR from:(senate.gov)
  OR from:Senator

  OR ActBlue
  OR WinRed

  OR "not authorized by any candidate"

  OR (
    {"paid for by" "authorized by"}
    {campaign committee candidate}
  )

  OR "Democratic Party"
  OR "Republican Party"

  OR (
    {
      subject:"I'm running"
      subject:"I’m running"
      subject:"running for"
      subject:endorsement
    }
    {Senate Congress Governor Mayor}
  )
)
-in:spam
-in:trash
-from:postmaster@mail.house.gov
```

**Actions:** Apply label `Noise/Political Outreach`.

**Description:** Identifies campaign, party, PAC, and elected-official outreach using generic political-mail signals rather than campaign-specific sender domains.
