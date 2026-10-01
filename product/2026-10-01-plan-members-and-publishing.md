# Plan: Members and publishing (piece 3), second run

Chilli Community. 1 October 2026. Status: Agreed by Priya, 1 October 2026.

This run starts again from the plan, at Priya's choice. It sits beside the 30 September 2026 plan, which stays in the history. Changes from that plan: no test purchase; founding members are added by hand with a free Gumroad code, so there is no add-a-member step in the app; the windowsill starter list and the 7 October confirm-by are dropped.

## The feature in one line
Paying on Gumroad lets a member in on their own. A refund ends their access at once. A cancellation ends it at the end of the month they paid for. Priya adds each week and chooses when it opens. Used by founding members and by Priya.

## The done tests (Priya, 1 October 2026)
- **Bought so in.** Start: someone has bought on Gumroad. Do: sign in with the same email. See: this week straight away.
- **Refunded so out.** Start: a member who got in by buying has been refunded in Gumroad. Do: reload the app. See: "membership not active" and none of the week's content.
- **Cancelled, still in until the month ends.** Start: a member has cancelled in Gumroad partway through a paid month. Do: sign in. See: this week, until the end of the month they paid for; after that, "membership not active". Gumroad's cancel message does not carry the paid month end date, so Priya ends cancelled members by hand for now.

## How members pay and get in (Priya, 1 October 2026)
- Price: £8 a month, the founding price, through Priya's Gumroad link.
- Buying adds the member on its own. They sign in with the same email they bought with and land on This week.
- Founding members Priya invites herself are given a free Gumroad code, so they get in through the same buying path. There is no add-a-member step in the app. Who the founding members are: To be decided.

## How access ends (Priya, 1 October 2026)
- Refunded: access ends at once, on the next reload.
- Cancelled: the member keeps access to the end of the month they paid for. Priya ends them by hand at that point.

## Steps, in build order
1. **Buying lets you in.** The app hears from Gumroad when someone buys and checks the message is from Chilli's product. The buyer becomes a member once, even if the message arrives twice.
2. **Not bought, not in.** An email with no purchase gets a plain page: membership not active yet, and how to join. It shows none of the week's content.
3. **Refund or cancel ends access.** A refund ends access on the next reload. A cancellation ends it at the end of the month paid for (by hand for now).
4. **Priya's area.** Only Priya can open it, with the members list. A member who types its address sees a page saying it is not for members.
5. **Add a week and schedule it.** Priya adds the recipe (photo, ingredients, method, time), the video with captions and the post, and chooses when it opens. It shows as Scheduled. At the opening time it becomes This week, and last week moves to the top of Past weeks with ticks and posts kept. Week one opens Monday 19 October 2026. Which day later weeks open: To be decided.

Nobody buys, cancels or refunds anything. Checks use Gumroad's sample messages only. Priya only looks at her payment page.

## What stays private
- Only signed-in members with active access see weeks, posts, photos and names. A signed-out visitor sees the sign-in page and nothing else.
- A member's email is never shown to other members.
- Only Priya sees the members list and the add-a-week page.
- Who is asking always comes from their sign-in, never from what a page says.
- A message that did not come from Chilli's Gumroad product lets nobody in and changes nothing.

## When something goes wrong
- If Gumroad's message about a purchase does not arrive, the buyer sees "membership not active yet, and how to join". The app sends nothing, so Priya spots the gap by comparing her Gumroad sales with the members list.
- A week saved with no video or no opening time gives a plain message naming what is missing, and nothing already typed is lost.

## What must not change
- Signing in, and This week with its ticks still there after signing out and back in.
- Past weeks.
- The challenge: posting, the one chilli per member rule, removing your own post, and no photo for a signed-out visitor.

## By hand for now (Priya, confirmed 1 October 2026)
1. Write each week's recipe, film the video and write the week's job.
2. Write the rescue card before the first member joins.
3. Create and publish the Gumroad product on Monday 19 October 2026, with the first-month promise ("Kill your chilli plant? Your first month is back").
4. Connect the live Gumroad product to the app.
5. Set up the email service that sends sign-in links, before go-live.
6. Add founding members with a free Gumroad code.
7. Give first-month refunds in Gumroad when someone asks.
8. Send every invitation herself.
9. End cancelled members at the end of the month they paid for.
10. If a paid member is not let in, check the sale in Gumroad and tell Claude.

Dropped this run: the test purchase. Priya will not make one.

## Unknown, left out of the build until Priya decides
- Which day later weeks open.
- How members sign in on the real address: a sign-in link by email is the draft, and needs the email service (by hand, step 5).
- Who the founding members are.

## Not in this feature
Comments, notifications, emails from the app other than the sign-in link, checkout inside the app, Priya removing someone else's post, a page of pilot numbers, an add-a-member step, and Claude adding a week through its connection.
