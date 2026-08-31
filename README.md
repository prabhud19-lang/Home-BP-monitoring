# Home BP Monitor

Full-stack, mobile-first 7-day home blood pressure monitoring app.

## Run

```bash
npm install --cache /private/tmp/home-bp-npm-cache
npm start
```

Open `http://localhost:3000`.

Demo account: `demo@example.com` / `demo123`.

## Email delivery

Copy `.env.example` to `.env` and set `SMTP_HOST`, `SMTP_PORT`, `SMTP_USER`, `SMTP_PASS`, and `SMTP_FROM`. Without those variables, Excel download remains available and the UI explains that email needs configuration.

## Included

- SQLite relational data model with user ownership and monitoring cycles
- JWT authentication, bcrypt hashing, rate-limited login/register routes
- Onboarding/profile management and protected API routes
- 7-day, two-session protocol with raw readings and last-two average logic
- Historical cycles, editable sitting entries, and simple trend visualization
- Server-generated Excel workbooks and SMTP email attachment support
- Seeded active and complete demo monitoring cycles
