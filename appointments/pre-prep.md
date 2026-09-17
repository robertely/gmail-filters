# Appointment Pre-Prep

**Label:** `Appointments/Pre-Prep`

**Gmail query:**

```text
{
  (
    subject:"check in"
    {
      subject:appointment
      subject:visit
    }
  )

  (
    subject:"check-in"
    {
      subject:appointment
      subject:visit
    }
  )

  subject:"when you arrive, check in here"
  subject:"patient forms"

  (
    subject:forms
    {
      subject:patient
      subject:appointment
      subject:visit
    }
  )

  subject:"before your visit"
  subject:"before your appointment"

  (
    subject:questionnaire
    {
      appointment
      visit
      patient
    }
  )
}
-in:spam
-in:trash
```

**Actions:** Apply label `Appointments/Pre-Prep`.

**Description:** Identifies appointment preparation messages such as online check-in, patient forms, questionnaires, pre-registration, and other tasks to complete before a visit.
