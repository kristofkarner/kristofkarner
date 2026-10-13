# Kristóf Karner

Independent web developer in Budapest. I build the web systems a business runs
on — booking, payments, automation — and keep them running afterwards.

Most of my work is long-term: maintenance and extension of systems already
running, rather than one-off delivery. I work with small and medium businesses,
in Hungarian and English.

## What I work with

- **Payments and subscriptions** — Stripe Checkout and Billing, webhook-driven
  state changes, idempotent event handling.
- **Access control** — Telegram Bot API: single-use invite links, subscription
  lifecycle, expiry and re-entry.
- **Invoicing** — Számlázz.hu Agent API, including the parts that only matter
  under Hungarian rules.
- **Monitoring** — a daily check of the sites I maintain. That code stays
  private: it describes client systems.
- **The rest** — PHP, Python, JavaScript, plain HTML and CSS; WordPress where
  the client edits the content; and the maintenance that keeps all of it
  running.

## How I work

With AI, every day: Claude Code, and Cursor where it fits better. First I
write down what the system has to do; the code follows that, and a machine
checks the result before it goes live. The decisions and the responsibility
stay with me.

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

I publish what I learn while building, in Hungarian and English. The ones next
to the code above:

- [Stripe subscriptions and automated invoicing](https://kristofkarner.com/en/writing/stripe-automated-invoicing/)
  — webhooks, currency, refunds, and why the same event arriving twice matters
- [Paid Telegram access](https://kristofkarner.com/en/writing/paid-telegram-access/)
  — invites, identifying the payer, expiry, and what the Bot API cannot do
- [Email authentication: SPF, DKIM, DMARC](https://kristofkarner.com/en/writing/email-authentication-spf-dkim-dmarc/)
  — why business mail lands in spam, and how the three records fit together

And from the workshop, on how the work itself is done:

- [Why there is no build step on this site](https://kristofkarner.com/en/workshop/why-there-is-no-build-step/)
  — plain HTML, zero dependencies, and when that is the wrong call
- [I fingerprint every file after a deploy](https://kristofkarner.com/en/workshop/file-fingerprints/)
  — whether anything on the server differs from what was uploaded, and where
  the check is blind
- [Four WP-CLI deploy traps that fail silently](https://kristofkarner.com/en/workshop/wp-cli-deploy-traps/)
  — escaped URLs, permissions carried through tar, an empty database export,
  a collation clash
- [How the agents got into Hugging Face](https://kristofkarner.com/en/workshop/how-the-agents-got-into-hugging-face/)
  — the chain step by step, and what applies from it to a website

All of it: [kristofkarner.com](https://kristofkarner.com/en/)

## Contact

kristof@kristofkarner.com · [LinkedIn](https://www.linkedin.com/in/kristofkarner/)

I don't work from template quotes. Describe what you want to solve, and you get
a price for that job.
