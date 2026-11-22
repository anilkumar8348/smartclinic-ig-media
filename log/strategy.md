# @smartclinicindia: content strategy

Read this before making any post. The weekly review rewrites the
"Current focus" section from the numbers in `posts.csv`. Daily runs follow it.

## Goal

Grow followers among clinic owners, doctors, diagnostic/pathology labs and
small hospitals in India, and get keyword comments (leads).

## Current focus (updated 2026-11-22)

Numbers: 18 posts in the last 30 days (7 Reels, 7 carousels, 4 images), all
metrics from Windsor on 22 Nov. Small sample: read every point below as a
direction, not a proof.

- Account: 4 followers (3 a week ago). Reach 15-21 Nov 211 accounts (97%
  non-followers), views 278, vs reach 3 / views 8 on 8-14 Nov. Profile link
  taps 0. Saves 0, shares 0, comments 0, follows from posts 0 on every post.
- Reels carry the account. Median reach per post is 3. Reels: median 25,
  mean 31, outlier multiples 5.7x-23.7x. Carousels: median 2 (0.3x-1.0x).
  Images: median 2. Feed posts only reach the 4 followers.
- Top 3 by outlier multiple: CBC AI Smart Report Reel 17 Nov (71 reach,
  23.7x), RX in the patient's language Reel 20 Nov (49, 16.3x), pharmacy Reel
  21 Nov (29, 9.7x). Bottom 3: physio carousel 22 Nov (1, 0.3x), and five
  feed posts tied at 2 (0.7x). What separates them is format, nothing else
  we can see: every Reel beats every feed post.
- The real problem is the first second of the Reel. Skip rate (left within
  3 s) is 79-94%, so only 6-21% of viewers get past the cover; average watch
  time 1.9-4.5 s on a ~25 s Reel. Best hold: pharmacy 21 Nov (21% held,
  cover "Expired stock is money thrown away.", cost/waste hook) and physio
  22 Nov (15%, "Stop tracking physio progress in a notebook.", negative
  command). Worst: RX 20 Nov 6%, token 19 Nov 7%, CBC 17 Nov 8% (statement
  hooks about patients / waiting room). n=6, so this is weak evidence.
- Reach and hold do not line up yet (CBC and RX got the most reach with the
  worst hold), so reach is still mostly Instagram's test audience, not the
  hook. The fix we can control is the hook.

Do more
- Make every day's Reel the main post; build the carousel so its cover and
  scenes make a strong Reel (week.py turns the carousel into the Reel).
- Cover hooks of 7 words or fewer, a concrete object or task on screen
  (paper register, retyped prescription, CBC sheet), and a loss or a waste
  in the words. Lean on: cost/waste (hooks.json 1), stop/do instead (2),
  old vs new (13), A versus B (17), specific group (14), if you X, this
  fixes it (10). Score with hookscore.py, best of 3.
- Topics with the most Reel reach: AI Smart Report (CBC) and prescriptions
  in the patient's language. Come back to them with a new angle.

Stop
- Long statement hooks about patients ("A full waiting room isn't a sign of
  success."). 7-9% hold.
- Expecting the evening image or the carousel to grow the account: 2 reach
  each. Keep them light; the effort goes into the Reel's first scene.

Next week (2-8 Dec)
- Every confirmed feature has now been used in the last 14 days, so repeat
  topics with a new angle and a new hook formula: AI Smart Report (old vs
  new), live clinic view on the phone (first carousel on it), paper vs
  software for one visit (A versus B), pharmacy dispensing from the
  prescription (cost/waste, our best hold), physio for physiotherapists
  (specific group), prescription on WhatsApp in Bengali (mid-action),
  one GST bill with UPI (the only bill).

Hashtags
- No post got reach from hashtags that we can see (0 saves/shares, all reach
  explained by Reels distribution). Keep the 5-tag mix below unchanged; no
  evidence yet to drop any. Revisit when a post gets 100+ reach.

Profile
- About 200 non-followers reached, 0 follows. With 79-94% skipping in 3 s,
  most never saw enough to visit the profile, so fix hooks first; check the
  profile (ig-profile) once a Reel passes 30% hold.

## Captions

- Hook in the first 125 characters: a concrete problem a clinic owner feels
  (waiting room, paper registers, missed follow-ups, unreadable reports, billing errors).
- Plain words people search: clinic management software, clinic software India,
  OPD software, pathology lab software, pharmacy billing software, GST billing for clinics.
- One ask with one keyword (DEMO, REPORT, QR, TOKEN, ...). No links. No prices.

## Hashtags (Instagram allows max 5)

Use exactly 5, in this mix:
1. Branded, always: #SmartClinicIndia
2. Product category (pick 1): #clinicmanagement #clinicsoftware #hospitalsoftware #pathologylab #healthtechindia
3. Audience (pick 1-2): #doctorsofindia #indiandoctors #clinicowner #diagnosticcentre #physiotherapyindia #pharmacyindia
4. Topic of the post (pick 1): e.g. #opdmanagement #labreport #whatsappforbusiness #gstbilling #digitalprescription
Avoid #viral #explore #fyp #reels and anything unrelated.

## What to log

After every post, append a row to `posts.csv`. Every run also refreshes the
metric columns for posts from the last 30 days.
