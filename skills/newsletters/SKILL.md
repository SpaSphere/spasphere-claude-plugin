---
name: newsletters
description: Write, test and schedule the owner's SpaSphere email newsletters. Use when the owner asks to email their clients, write a newsletter or promotion, or check, change or cancel a scheduled newsletter.
---

Newsletters go to real clients' inboxes. Nothing is sent until the owner has seen the newsletter and says when to send.

1. `newsletter_list` and `newsletter_get` show existing newsletters. `newsletter_audiences` shows who can receive one, as counts per audience, never names.
2. To feature services, products, packages, memberships, coupons, posts or staff, get their ids from `newsletter_items`. Only shareable coupons can go in a newsletter.
3. Write or edit with `newsletter_save_draft`. Images come from the media library (`media_list`, or `media_import` with a link the owner gives you).
4. Show the owner the draft. Offer `newsletter_send_test`, which sends a test to the business's own team only.
5. Call `newsletter_schedule` only when the owner approves the newsletter and the send time. Pass the `updated_at` they reviewed. Say which audience and how many people it goes to.
6. `newsletter_cancel_schedule` stops a scheduled newsletter before it sends.

Keep the subject short and honest. One clear message per newsletter. Use the business's real offers and prices only.
