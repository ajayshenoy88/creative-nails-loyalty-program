# Creative Nails Rewards

**Creative Nails Rewards** is a multi-partner loyalty program built for Creative Nails, a nail salon. It lets Creative Nails team up with other nearby businesses (a gym, a spa, a fitness studio, etc.) to send customers to each other with real discounts, tracked digitally instead of on paper punch cards.

This repository holds the project's documentation only. It's shared so anyone evaluating or reviewing the project can see what it does and how it's used, without access to the underlying source code (kept in a private repository).

## The idea in plain terms

A partner business — say, a gym in the same building — tells its members about Creative Nails. A member signs up in a few taps, and gets a series of discount codes for their first few visits to Creative Nails (for example: 20% off visit 1, 15% off visit 2, 10% off visit 3, and a standing 10% off every visit after that). Each code only becomes usable once the customer actually shows up and a code is redeemed in person — nothing is charged or given away just by signing up online.

The same idea works the other way too: Creative Nails' own customers could be sent to a partner business with their own discount codes, if that partnership is set up.

## Who uses it, and how

The app has four kinds of sign-in, each scoped to exactly what that person needs:

- **Customer** — signs in with just a mobile number and a 6-digit PIN they choose themselves (no email, no app download). Sees every code they've earned, across every partner they're enrolled with, and exactly when each one expires.
- **Staff** (Creative Nails front desk) — signs in to a single redemption screen. Looks up a customer, sees their available codes, and marks one as used at checkout. This is the only way a code actually gets redeemed, which keeps the whole system honest.
- **Business** (the partner, e.g. the gym) — one shared sign-in per partner business. They can see everyone enrolled through their program, how many codes have been redeemed, and can enroll a new customer directly (e.g. signing up a new member at their own front desk). They can't see any other partner's data, and can't touch anything Creative Nails itself manages.
- **Admin** (Creative Nails) — full control. Adds and manages partner businesses, sets up each program's discount structure, manages every login, and can look up or adjust any customer's codes if something needs fixing.

## How a customer actually experiences it

1. A partner business shares their enrollment link or a QR code (e.g. a poster at the gym's front desk).
2. The customer taps it, enters their name, mobile number, and picks a 6-digit PIN — takes under a minute.
3. They immediately see their new codes: what's active right now, and what unlocks after future visits.
4. Next time they're at Creative Nails, they mention they have a code; staff looks them up by mobile number and applies the discount.
5. Redeeming one code that day automatically unlocks the next tier for their following visit.
6. To check their codes again later, they just sign back in with their mobile number and PIN — no account to remember, no password to forget (and if they ever do forget their PIN, an Admin can reset it in one click).

## What's in this repository

- `README.md` — this file.
- `PLAN.md` — the complete project plan: every product decision, the data model, the screen-by-screen design, security and validation rules, and the build log. This is the same working document used to build the app, kept here in full for transparency into how and why it was built the way it was.

No application source code, database credentials, or configuration lives in this repository — those are kept in a separate private repository.
