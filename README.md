# Kristóf Karner

Independent web developer in Budapest. I build the web systems a business runs
on — booking, payments, automation — and keep them running afterwards.

Most of my work is long-term: maintenance and extension of systems already
running, rather than one-off delivery. I work with small and medium businesses,
in Hungarian and English.

## What I work with

**Payments and subscriptions** — Stripe Checkout and Billing, webhook-driven
state changes, idempotent event handling.
**Access control** — Telegram Bot API: single-use invite links, subscription
lifecycle, expiry and re-entry.
**Invoicing** — Számlázz.hu Agent API, including the parts that only matter
under Hungarian rules.
**The rest** — PHP, WordPress, custom backends, and the maintenance that keeps
all of it running.

## Code

Working references for problems I could not find a decent write-up of
anywhere. Each one is self-contained, and each has a test that runs without a
network.

- **[stripe-szamlazz-hu](https://github.com/kristofkarner/stripe-szamlazz-hu)**
  — a Hungarian fiscal invoice issued from a Stripe webhook. The order of
  operations is the point: verify the signature, reserve the event, then issue.
- **[telegram-subscription-access](https://github.com/kristofkarner/telegram-subscription-access)**
  — paid access to a private Telegram group: single-use invites, pairing a
  payment with a Telegram account, and removal that still lets the member
  return.
- **[dmarc-report-reader](https://github.com/kristofkarner/dmarc-report-reader)**
  — reads DMARC aggregate reports and shows which senders would break under a
  stricter policy, telling misalignment apart from real authentication failure.

## Writing

I publish what I learn while building. These are the practical ones, mostly in
Hungarian — the areas where I could not find a decent local write-up:

- [Stripe subscriptions and automated invoicing](https://kristofkarner.com/en/writing/stripe-automated-invoicing/)
  — webhooks, currency, refunds, and why the same event arriving twice matters
- [Paid Telegram access](https://kristofkarner.com/en/writing/paid-telegram-access/)
  — invites, identifying the payer, expiry, and what the Bot API cannot do
- [Telegram Stars or a custom system?](https://kristofkarner.com/en/writing/telegram-stars-or-custom-system/)
  — when the built-in subscription is enough, and when it is not
- [Email authentication: SPF, DKIM, DMARC](https://kristofkarner.com/en/writing/email-authentication-spf-dkim-dmarc/)
  — why business mail lands in spam, and how the three records fit together

All of it: [kristofkarner.com](https://kristofkarner.com)

## Contact

kristof@kristofkarner.com

I don't cold-contact anyone, and I don't work from template quotes. Describe
what you want to solve, and you get a price for that job.
