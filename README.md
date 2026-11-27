# Maruan Aguerdouh

Software engineer in Brussels. I spent three and a half years on Odoo's Bugfix team, taking production tickets through to a merged fix in a very large Python and JavaScript ERP — mail, the web client, accounting, events, eLearning, inventory, POS, and the website.

I have 107+ merged pull requests in public [odoo/odoo](https://github.com/odoo/odoo/pulls?q=is%3Apr+author%3AEphoniz), plus work in the private `odoo/enterprise` repo that can't be linked here. Odoo merges through a bot, so GitHub shows those pull requests as closed rather than merged.

These days I am building [Onky](https://github.com/Ephoniz/Onky), a native desktop audio mixer, and [Odoo Atlas](https://github.com/Ephoniz/odoo-atlas), a static, clickable map of Odoo's models, methods and OWL components. I am interested in AI as a tool I want to get better at, not as a skill I am claiming.

Open to software engineer, Odoo, and AI-curious roles. Happy to relocate.

[LinkedIn](https://www.linkedin.com/in/maruan-aguerdouh-ab5443213) · Brussels · `maruan.mx@gmail.com`

## Selected contributions

GitHub cannot pin pull requests, so this list stands in for that. Each one is a fix I authored in [odoo/odoo](https://github.com/odoo/odoo); Odoo's mergebot records the merge commit.

- [Push notifications were cut off, sometimes to an empty body](https://github.com/odoo/odoo/pull/193641) — the truncator ignored encryption overhead and mixed up character length with encoded bytes.
- [Editing a recurring Outlook event from Odoo could email every attendee](https://github.com/odoo/odoo/pull/199663) — even a colleague who was not synced to Outlook could trigger a burst of unwanted updates.
- [Reopening a saved line in a form showed an incomplete record](https://github.com/odoo/odoo/pull/136068) — only the list-view fields were reloaded, which showed up clearly in eLearning course content.
- [The calendar filter for your own attendance always came back empty](https://github.com/odoo/odoo/pull/218878) — it was comparing event IDs to attendee records, which could never match.
- [Partner portal users got a 404 posting on an assigned opportunity](https://github.com/odoo/odoo/pull/252854) — when the opportunity was assigned to the company, not to the person signed in, the chatter access check missed them.
- [Lowering ticket quantity in the cart still left extra registrations open](https://github.com/odoo/odoo/pull/150463) — checkout charged for the new quantity, but the leftover event registrations were not cancelled.
- [Admins got a false "Delivery Failed" when resending someone else's email](https://github.com/odoo/odoo/pull/173406) — the mail could already have gone out; the error was from writing a related field they did not have direct access to.
- [Marking a subcontracting location for replenishment crashed](https://github.com/odoo/odoo/pull/113361) — the location has no warehouse, and the replenishment logic assumed one.
- [Event emails used the wrong company for colours and access](https://github.com/odoo/odoo/pull/236764) — templates followed the sender's company instead of the event's, which also errored in a multi-company database.
- [The Sales Team picker on mobile showed the wrong view](https://github.com/odoo/odoo/pull/116031) — after Odoo dropped `kanban_view_ref`, the replacement had to be applied across 13 modules.
