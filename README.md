# Matt Maggio

I carry a quota and I build the tooling that makes the quota easier to carry.

Day job is Strategic Account Manager at Future Electronics, selling components into
defense, aerospace and industrial accounts. Alongside that I run an independent automation
practice, where the work is building AI systems for companies whose processes live in
spreadsheets and someone's inbox.

Both projects below started the same way. A process was eating somebody's week, there was
no budget to buy a fix, so I built one.

---

## Team store automation

A custom apparel company was running its entire team-store sales cycle by hand: finding
schools, chasing logos, building storefronts one product at a time, and tracking
production on a Monday.com board that knew nothing about the orders. I built the system
that replaced it, from prospecting through to the print files that go to the manufacturer.

A custom CRM is the system of record underneath nine Claude Code agents, with approval
gates that survive headless execution so nothing reaches a customer without a recorded
sign-off. A resumable backfill reconstructed 542 storefronts and $4.09M of order history
into a database the company had never had.

Order-to-print runs on live customer orders today. Several other subsystems are built and
waiting on client-side credentials rather than on more code, and the write-up says which
is which.

[Read the case study →](https://github.com/MattMaggio/team-store-automation)

## FAEagent

An AI sales assistant I built for my own territory work: account research, part finding
and cross-referencing, block diagrams, BOM scrubbing, and assembling design-win
registrations for a legacy Oracle CRM.

The hard part was reliability, not prompting. It routes across two model providers with a
five-rung fallback ladder, classifies failures so a daily quota is not treated like a dead
model, and ships behind an eval harness of 21 cases that gates every deploy. That harness
exists because production broke twice from upstream changes I did not control.

Users bring their own API keys, held in their browser, so there is no central store of
anyone's secrets. Built solo, on my own time, and in real use.

[Read the case study →](https://github.com/MattMaggio/faeagent)

---

Five years in technical customer-facing sales across enterprise IT, defense, and
semiconductor distribution. Previously Dell and Sealing Technologies. B.S. Information
Science, University of Maryland.

Both repositories above are write-ups rather than source. The code is private because it
runs real businesses, and I am happy to walk through either one.
