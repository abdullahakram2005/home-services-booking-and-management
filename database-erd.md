USER
 │
 ├─────────────── CUSTOMER
 │
 └─────────────── SERVICE PROVIDER
                       │
                       │
                       ↓
                    SERVICE
                       │
                       ↓
                    BOOKING
                       │
                       ↓
                    REVIEW

┌──────────────┐
│     USER     │
├──────────────┤
│ userId (PK)  │
│ name         │
│ email        │
│ password     │
│ phone        │
│ address      │
│ role         │
└──────┬───────┘
       │
       │
       ├─────────────────────┐
       │                     │
       ↓                     ↓
┌──────────────┐      ┌──────────────────┐
│   CUSTOMER   │      │ SERVICE PROVIDER │
├──────────────┤      ├──────────────────┤
│ customerId   │      │ providerId (PK)  │
│ userId (FK)  │      │ userId (FK)      │
└──────┬───────┘      │ experience       │
       │              │ location         │
       │              │ availability     │
       │              └────────┬─────────┘
       │                       │
       │                       │
       │              ┌────────↓─────────┐
       │              │     SERVICE      │
       │              ├──────────────────┤
       │              │ serviceId (PK)   │
       │              │ providerId (FK)  │
       │              │ name             │
       │              │ category         │
       │              │ description      │
       │              │ price            │
       │              └────────┬─────────┘
       │                       │
       │                       │
       └──────────┐            │
                  ↓            ↓
             ┌─────────────────────┐
             │       BOOKING       │
             ├─────────────────────┤
             │ bookingId (PK)      │
             │ customerId (FK)     │
             │ providerId (FK)     │
             │ serviceId (FK)      │
             │ date                │
             │ time                │
             │ address             │
             │ status              │
             └──────────┬──────────┘
                        │
                        ↓
                 ┌──────────────┐
                 │    REVIEW    │
                 ├──────────────┤
                 │ reviewId PK  │
                 │ bookingId FK │
                 │ customerId   │
                 │ providerId   │
                 │ rating       │
                 │ comment      │
                 └──────────────┘
