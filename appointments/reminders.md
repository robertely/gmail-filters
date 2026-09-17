# Appointment Reminders

**Label:** `Appointments/Reminders`

**Gmail query:**

```text
(
  (
    subject:appointment
    {
      subject:reminder
      subject:upcoming
      subject:"is on"
      subject:"is today"
      subject:"see you"
      subject:"please confirm"
    }
  )
  OR subject:"upcoming visit"
  OR (
    subject:reminder
    subject:session
  )
)
-subject:changed
-subject:rescheduled
-subject:canceled
-subject:cancelled
-subject:confirmed
-subject:"new appointment booked"
-subject:"appointment details"
-subject:"how was"
```

**Actions:** Apply label `Appointments/Reminders`.

**Description:** Identifies reminders for upcoming appointments, visits, and sessions while excluding common confirmation, reschedule, cancellation, and post-visit messages.
