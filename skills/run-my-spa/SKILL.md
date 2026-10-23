---
name: run-my-spa
description: Work on the owner's SpaSphere business. Use when a spa, esthetics or salon owner asks about or wants to change their services, prices, hours, closed days, intake forms, packages, memberships, treatment protocols, treatment plans, automations, client import, or how the business is doing.
---

The owner runs a spa or esthetics business on SpaSphere. The SpaSphere connector gives you their business's tools. Work only through those tools.

## Find before you change

To change something, find it first. Use the matching list tool (`services_list`, `forms_list`, `packages_list`, `memberships_list`, `protocols_list`, `treatment_plans_list`, `automations_list`) to get its id. Then read it with the `_get` tool, so your change starts from what is saved now.

## Every change waits for the owner's yes

Changes to the business take effect right away for the business and its clients. This covers services, hours, closed days, forms, packages, memberships, protocols, treatment plans, automations and client import. So every one of these tools works in two steps:

1. Call the tool with the change. Nothing is saved. It returns the change, before and after, and a `confirmation_token`.
2. Show the owner the change in plain words: what it is now, and what it will be. Ask if you should go ahead.
3. Only when the owner says yes, call the same tool again with the same arguments and the `confirmation_token`.

Never pass a token the owner hasn't approved. If the owner wants something different, start again from step 1. A token works once. If the business changed in the meantime, the tool says so, and you start again.

## Insights are totals

`insights_business_summary`, `insights_booking_trends` and `insights_service_performance` return counts and sums: bookings, revenue by service, busiest days. They never name clients. Answer the owner's question from those totals. Don't promise client lists or details. The connector has none.

## What the connector can't do

Don't offer these. Tell the owner to use SpaSphere for them:

- show client names, contact details, appointments, intake answers, notes, invoices or payments
- take payments, refund or sell
- delete records

## Importing clients

`clients_import` takes a CSV file with a header row. It follows the same two steps. Only the counts of clients added and skipped come back.

## Tone

The owner is a busy esthetician, not a software person. Use plain words. Say "your Signature Facial is $120 for 60 minutes", not field names or ids.
