# Weak spots: Chilli Community

Week 20, Make it stronger. Written 30 September 2026.

This record is what Priya told Claude, plus the Chilli records already in this second brain (the hardening report of 24 September, the launch record and the member test). Claude did not open the Weak-spots page or the app, and did not see the fix. Anything not listed here is Unknown.

## In one line

Six weak spots, ranked by harm to members with security first. The worst, a cancelled member still seeing the week's post, is fixed and rechecked by Priya on her phone. The Gumroad check is still to do and waits for the real test purchase on Monday 19 October 2026. One spot needs no work because Priya says test and live are already separate.

## The ranking

| # | Weak spot | Who it affects | State | Call | Date |
|---|---|---|---|---|---|
| 1 | A member who cancelled could still see the week's post | Every paying member: members-only content reached by someone who no longer pays | Fixed, rechecked by Priya on her phone | Fix | Done |
| 2 | A Gumroad sale notice is trusted without asking Gumroad | Members: a stranger let in without paying could see members' photos and names | Still to do | Fix | Monday 19 October 2026, with the real test purchase. The doors stay shut until it passes. |
| 3 | Test and live may share one database plan | Members: practice accounts and untested changes beside real members' things | Priya says already separate. Not checked from the lab. | No work | None |
| 4 | No backup and no practice restore | Every member: ticks, posts and photos could be lost for good | Not done | Fix | Friday 16 October 2026 |
| 5 | The way back is written but never tried | Every member if something goes wrong; only Priya can put up the back soon page (Unknown) | Not tried | Fix | Sunday 18 October 2026 |
| 6 | Errors are not kept and no usage alerts are set | Members who hit a fault Priya never hears about | Accepted for the pilot | Accept, look again | Monday 26 October 2026 |

Order confirmed by Priya: she put the cancelled member first, then the rest in Claude's order.

## 1. A member who cancelled could still see the week's post

- **What Priya saw:** a member whose paid month had ended still saw the week's post.
- **What it should do:** access ends at the end of the month the member paid for (the product plan's draft rule). This was a bug, not the rule.
- **The fix:** made in Claude Code on the web.
- **Recheck by Priya, on her phone:** a member whose paid month has ended no longer sees the week's post. Priya's score for the recheck: yes.
- **Not reported, so Unknown:** that a member with a paid month still running gets straight in; that a member who never paid sees the not-active page; that signed-out people still cannot see members' posts and photos; whether Ed has reviewed this fix.

## 2. A Gumroad sale notice is trusted without asking Gumroad

- **Why it matters:** the app lets someone in when a notice arrives at its private address naming Chilli's product. Gumroad does not sign its notices, so anyone who learned the address could let someone in without paying.
- **Why it waits:** the check that asks Gumroad about each sale needs the real Gumroad product and an access key. The product is created on Monday 19 October 2026.
- **The plan:** the check is built and tried with the real test purchase on Monday 19 October 2026. Priya chose to keep this plan. Claude's suggestion to build it earlier with test sales, by Sunday 18 October, was offered and not taken.
- **Rule:** the doors stay shut until it passes.

## 3. Test and live

Priya says the test and live versions are already separate. Claude did not check this.

## 4. Backup and practice restore

Not done. Planned for Friday 16 October 2026. A data export alone would not bring back members' photos, so the practice restore includes them.

## 5. The way back

Written, one hour to try a fix and then a back soon page, Priya decides. To try it once by putting the page up and taking it down again: Sunday 18 October 2026.

## 6. Errors and usage

Accepted for the pilot. Reason: low harm for 10 to 20 members. Look again on Monday 26 October 2026, then watch weekly as in the hardening report.

## Check-in answers, as Priya gave them

- Email sending for sign-in links is connected and links work: 9 out of 10.
- Privacy note and terms approved: 8.
- Ed reviewed the app changes: 8.
- Video words and photo upload fixes done: 7. They read Fixed only once Jo repeats those steps; when she does is To be decided.
- Nadia, Megan and Jo confirmed their place.
- First backup and practice restore: not done.

## Unknown

- Whether the fix for weak spot 1 covers a paying member, a never-paid person and signed-out people (see above).
- Whether Ed has reviewed the weak spot 1 fix.
- Whether test and live are separate (Priya's word only).
- Who besides Priya can put up the back soon page.
