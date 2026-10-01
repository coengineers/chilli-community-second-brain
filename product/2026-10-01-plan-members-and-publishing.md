# Plan: Members and publishing

Chilli Community. 1 October 2026. Status: Agreed by Priya, 1 October 2026.

This replaces the plan of 1 October 2026 that was written in the earlier Week 16 run. Changes from that plan: Past weeks and the challenge are left out of this feature and out of what must not change, because the product plan puts both on hold for version 1; last week simply stops showing to members and is kept, not deleted; the "write the rescue card" by-hand step is removed, because offer version 6 cut the rescue card.

## The feature in one line
Paying on Gumroad lets a member in on their own. A refund or cancel ends their access. Priya adds each week and chooses when it opens. Used by founding members and by Priya.

## The done tests (Priya, 1 October 2026, confirmed as drafted)
- **Bought, so in.** Start: someone has bought on Gumroad. Do: sign in with the same email. See: this week straight away.
- **Refunded, so out.** Start: a member who got in by buying is refunded in Gumroad. Do: reload the app. See: "membership not active" and none of the week's content.
- **Cancelled, still in until the month ends.** Start: a member has cancelled in Gumroad partway through a paid month. Do: sign in. See: this week until the end of the month they paid for, then "membership not active". Gumroad's cancel message does not carry the paid month end date, so Priya ends cancelled members by hand for now.

## Steps, in build order (agreed as drafted, Priya, 1 October 2026)
1. **Buying lets you in.** The app hears from Gumroad when someone buys and checks the message is from Chilli's product. The buyer becomes a member once, even if the message arrives twice. They sign in with the same email and land on This week.
2. **Not bought, not in.** An email with no purchase sees a plain page: membership not active yet, and how to join. None of the week's content shows.
3. **Refund or cancel ends access.** A refund ends access on the next reload. A cancellation ends it at the end of the month paid for, which Priya does by hand for now.
4. **Priya's area.** Only Priya can open it, with the members list. A member who types its address sees a page saying it is not for members.
5. **Add a week and schedule it.** Priya adds the recipe (photo, ingredients, method, time), the video with captions and the post, and chooses when it opens. It shows as Scheduled and at the opening time becomes This week. Last week stops showing to members and is kept, not deleted. Week one opens Monday 19 October 2026.

## What stays private (confirmed by Priya, 1 October 2026)
- Only signed-in members with active access see the week.
- A signed-out visitor sees the sign-in page and nothing else.
- A member's email is never shown to other members.
- Only Priya sees the members list and the add-a-week page.
- A message that did not come from Chilli's Gumroad product lets nobody in.

## When something goes wrong
- If Gumroad's message about a purchase does not arrive, the buyer sees "membership not active yet, and how to join". The app sends nothing, so Priya spots the gap by comparing her Gumroad sales with the members list.
- A week saved with no video or no opening time gives a plain message naming what is missing, and nothing already typed is lost.

## What must not change
- Signing in.
- This week, with its ticks still there after signing out and back in.

## By hand for now
1. Write each week's recipe, film the video and write the week's job.
2. Create and publish the Gumroad product on Monday 19 October 2026, with the first-month promise.
3. Connect the live Gumroad product to the app.
4. Set up the email service that sends sign-in links, before go-live.
5. Add founding members with a free Gumroad code.
6. Give first-month refunds in Gumroad when someone asks.
7. Send every invitation herself.
8. End cancelled members at the end of the month they paid for.
9. If a paid member is not let in, check the sale in Gumroad and tell Claude.

Nobody buys, cancels or refunds anything while checking. Checks use Gumroad's sample messages only.

## To be decided, left out of the build
- Which day later weeks open.
- Who the founding members are.
- How members sign in on the real address (a sign-in link by email is the draft, and needs the email service in by-hand step 4).

## Not in this feature
Past weeks, the challenge, comments, notifications, emails from the app other than the sign-in link, checkout inside the app, a page of pilot numbers, an add-a-member step, and Claude adding a week through its connection.
