# HANDOVER - CarswithSammy Content Creation

This file merges the handovers from both chats in the project: content strategy (part 1) and the weekly insights review task (part 2).

## Project setup
Project name: CarswithSammy Content Creation. Purpose: Instagram growth for @carswithsammy - content ideas, insights analysis, follower growth and retention. Niche is automotive, woman in a male-dominated space. One doc: "Carswithsammy Profile", containing only the link instagram.com/carswithsammy. No files saved in the workspace.

## How Claude should behave
Act as Sammy's strategic content partner. Casual and direct, like a friend. Never corporate, no waffle, no bullet points unless asked. Always use the project knowledge, no generic advice. Plain hyphens only, never a comma before "and".

## Profile snapshot (11 Nov 2026, viewed logged out)
25.5k followers, 449 following. Bio: UK Based Car Enthusiast / Cars, Lifestyle, Events / My Own Snow Foam. Highlights: Aura, S55, Europe, GTI, OEM retrofits. Issue: bio says snow foam but the link goes to the Aura interior cleaner.

## Caption ratings, last 12 posts
| Post | Notes | Score |
|---|---|---|
| Switzerland broke my brain | pin, 3,879 likes | 9 |
| Settle something for me | pin, 1,303 likes, 44 comments | 9 |
| Makes me not want to sell it | 1 Nov, 963 likes, 41 comments | 6 |
| Autumn | 11 Nov | 4 |
| Me wondering what to do next | 3 Nov | 4 |
| Polo GTI is unmatched | 21 Oct | 4 |
| I said what I said | 27 Oct reel | 3 |
| Post it's not cringe | 26 Oct | 3 |
| November giveaway | 9 Nov reel | 3 |
| polo gti | 8 Nov | 2 |
| S Class >> | 25 Oct reel | 2 |
| No words for this beast | 22 Oct | 2 |

Average about 4/10.

## Key feedback
Captions went lazy from late October - one-liners with nothing to reply to. What works is a specific opinion or story plus a question answerable in five words. "Not cringe" post is the wrong audience and off-voice. Giveaway reads like Splash wrote it, has a typo ("giving REFUNDING") and needs checking for a free entry route under UK rules. Hashtag typos: #volksvagen, #contentcreater. No Parked Up episode or talking reel in the last 12 posts. 30k by December needs about 4.5k in seven weeks, unlikely on statics alone.

## Captions ready to use
1. "Three years in and I still look back at it every time I park. What's the one thing on your car you'd never change?" (swap in real ownership time)
2. "Every time I get close to selling it I take it for a drive and talk myself out of it. Which car did you sell that you still think about?"
3. "It's stock power and I keep getting told to map it. Honestly not sure it needs it. Would you, or leave it alone?"
4. "20 years old and it still makes most new cars feel a bit soulless. Name a 00s car that's aged better than this."
5. "Nobody needs a supercharged V8 in a car this size. That's exactly why it's good. What's the least sensible car you've ever wanted?"
6. "One's small, loud and mine. One's huge, louder and ours. If you could only keep one, which is it?"
7. "Low sun, wet roads, car's filthy in ten minutes. Still my favourite time of year to drive. Do you keep washing yours through winter or give up till March?"
8. "Parked Up, episode 1. Walked past everything else at [show] to get to this. Daily it or weekends only?"
9. Reel idea: "Things I've been told at car shows that I'm still thinking about."

## Open items
- Rewrite the autumn caption.
- Plan two weeks of posts around the first Parked Up episode.
- Fix bio link mismatch.
- Yahoo mail and the built-in browser are disconnected until the chat is reopened in the desktop app.
- Weekly insights review task is live - see part 2.

---

# Part 2 - Weekly Instagram insights review (scheduled task)

## Goal
A scheduled task that runs every Monday at 8:00am Europe/London. It reviews the previous Mon-Sun of @carswithsammy posts and insights and gives a detailed breakdown of:
- what performed well and why
- what converted followers (follows per post, not just views)
- what to focus on for the week ahead

## Status (as of 11 Nov 2026)
- The task has not been created yet.
- Blocker: no Instagram data source is connected. Nothing in the session could read Instagram insights.
- Sammy chose to connect an Instagram analytics connector (Windsor.ai or Supermetrics) instead of using Chrome or sending screenshots each week. Not confirmed connected yet.
- The account must be a Creator or Business account to get insights.
- Check that the connector's free tier covers Instagram.
- 14 Nov update: Windsor.ai is connected (Instagram connector, account carswithsammy, id 17841430493341516). A test pull worked: reach, views, likes, comments, saves, shares, follows per post, profile visits, reel watch time and skip rate, plus daily new followers.
- Data gap: Instagram doesn't give follows or profile visits per reel. Reels are judged on daily new followers around the post date instead (an estimate).
- Use media_like_count / media_comments_count. The media_total_* fields came back empty.
- Scheduled task "Weekly Instagram review - carswithsammy" (trig_01H2XmJ4aeBgaRYnLtuD81Gn) runs Mondays 7:47am Europe/London. First run 16 Nov.
- It fires into the original Claude Code session (session_012rHePXNNAMMf1ydsAGp2Vb), because that session has Windsor.ai. A task that starts a fresh session each time couldn't have the connector attached in this organization. Each run also adds a line to the weekly review log at the end of this file.
- No phone push for this kind of task - check that session on Monday mornings.

## Next steps
1. Confirm the connector is live and can pull post-level data for @carswithsammy: reach, views, saves, shares, watch time, follows, profile visits.
2. Create the Monday 8am scheduled task with a standalone prompt that covers the goal above.
3. Fallbacks: Chrome on her computer (must be switched on and logged in at 8am) or screenshots sent each Monday.

## Existing scheduled tasks
- "Email triage" runs daily at 8am. Leave it alone.

## Tone rules for the report
Same as part 1: casual and direct like a friend, never corporate, no waffle. No bullet points unless asked. Plain hyphens only, no em or en dashes. Never a comma before "and". No generic advice - use her actual data.

## Aura snow foam sales (14 Nov)
Aura is sold on splashdetailing.co.uk. The snow foam is £11 (https://splashdetailing.co.uk/products/aura-snow-foam). The Aura Creator Kit (snow foam, shampoo and quick detailer) is £37 and gets free delivery over £30. The full range is at https://splashdetailing.co.uk/collections/aura.
The bio link was still pointing to the Aura interior cleaner page, with a Facebook tracking string on the end. New bio and link setup suggested on 14 Nov.
Sammy doesn't want a discount code - don't suggest one again. Still to do: ask Splash for a sales report or commission and for Instagram product tagging. Giveaway entry is buy plus follow both accounts. A purchase at the normal price is probably fine under UK rules, but Splash should confirm the T&Cs (closing date, how the winner is picked, eligibility). Label snow foam promo posts as an ad or paid partnership, because she has a commercial interest in it.
14 Nov update: bio and links now point to the snow foam and the Creator Kit. Sammy is posting a wash on her Story today and adding it to the Aura highlight. She gets monthly sales reports from Splash. There were no Aura orders in October or November so far, which means the buy-to-enter giveaway has had no entries. Correction: the bio link's text says interior cleaner but it does go to the snow foam page, so the link was never the problem. Likely causes: the snow foam hasn't appeared in any feed post since 15 Oct apart from the giveaway, there was no reason to buy now, and a single £11 order doesn't reach Splash's £30 free delivery. Proposed fixes are in the 14 Nov chat: turn the giveaway into free entry with a Creator Kit prize, a weekly snow foam reel, a post about why she made it, and checking Story link taps.

The '5 things all car enthusiasts know' and 'unpopular opinions' carousels were posted before 15 Oct, so the 30-day Windsor trial can't see them. Waiting on Sammy's in-app numbers for those posts (reach, follows, shares, saves, profile visits). Posting schedule for 16-22 Nov was given in the 14 Nov chat.

## Comment moderation (14 Nov)
Hid 7 sexual or creepy comments via Windsor.ai, with Sammy's approval. They can be reversed with unhide_comment.
17990039684883112 johnyjackson68, 18099891785656259 thereaaldeaall, 17958161841269959 factuals00 and 18082741772356220 eudald_ndt (all on the 1 Nov Polo post). 17914763538475246 user.rvdh (1 Nov). 18154714849553819 podval4ik77 (27 Oct reel, vulgar Russian slang). 18639621445017650 rishabhsingh9404 (1 Nov, asking if she's single).
Left visible but flagged to Sammy: onlyteabatch "Sexay" (22 Oct) and the.v8.kitcar "Dm me we need to model" (22 Oct).
Sammy is replying to comments herself using the drafted replies from the 14 Nov chat.
Car facts: the S55 is a 2004 (W220). The Polo GTI is a 5 door. Comment replies were posted on 14 Nov to capelvehiclecleaning, thememedealer68_, eliteauto_ca, elvis2023__, kyle.b.146 and garebear_003.
