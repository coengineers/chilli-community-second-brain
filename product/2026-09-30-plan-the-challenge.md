# Plan: The challenge (piece 2)

Chilli Community. 30 September 2026. Agreed by Priya, 30 September 2026.

## The feature in one line

A signed-in member posts a photo and a caption to the week's challenge, sees the other members' posts, and adds a chilli to one they like. For founding members, starting with Nadia, Megan and Jo.

## Done test (Priya's, decided before building)

I'm signed in and on the week's post. I add a photo and a caption. I see my post at the top, and a second member can see it and add a chilli. It must work on a phone.

## Decisions made in the Week 16 lab (Priya, 30 September 2026)

- The done test above, confirmed as written.
- What stays private: the list below, confirmed as right.
- The app shrinks photos for the member, so nobody has to resize anything.

## The steps, in build order

1. **Post to the week.** A member chooses a photo (from the camera or their photos), writes a caption and posts. The post appears at the top with their display name, the photo, the caption and 0 chillies.
2. **See everyone's posts.** The other members' posts for the week show below, newest first, each with name, photo, caption and chilli count.
3. **Add a chilli.** One chilli each per post: tapping again takes it away. The count is still right after a reload.
4. **Photos only.** If a member chooses a document instead of a photo, they see a plain message that only photos can be posted, and nothing is posted.
5. **Remove my own post.** A confirm step first, then the post and its photo are gone for everyone. Nobody sees a remove option on anyone else's post.

## What each member sees

- Their own post at the top straight after posting, and a chilli button under everyone else's.
- On a phone, everything fits with no sideways scrolling.

## What stays private

- Only signed-in members see posts, photos and names.
- A signed-out visitor gets the sign-in page, and no photo even from its exact address.
- A member can add one chilli per post.
- Only the poster can remove their own post.

## When something goes wrong

If the connection drops while posting, the member sees a message that it did not post and a Try again button. Their photo and caption are still there, and with the connection back it posts once.

## What must not change in the first journey

- This week's recipe, video and job, with ticks that stay after signing out and back in.
- Home opening on this week's job, and "3 of 3 done".
- Past weeks, and Yours from the start.
- Sign-in, My account, My files and Getting started.
- The Week 14 Home words, the button text and the wordmark.

## By hand for now

Priya removes nothing from the app. If a post needs to go, she asks the member or asks Claude.

## Not in this piece

Comments, notifications, emails, Gumroad and scheduling weeks (piece 3).
