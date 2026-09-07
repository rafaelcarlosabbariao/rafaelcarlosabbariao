## Rafael Carlos Abbariao

founder and maintainer of **gossip**, an open-source social intelligence project, and research
lead at **Back2Human** in new york. i build instruments that measure how people actually behave,
then publish the number — including when the number ends the product.

### whatthefad? — a cultural archaeology engine

**[cultural-archaeology](https://github.com/rafaelcarlosabbariao/cultural-archaeology)** · live at
**[whatthefad.netlify.app](https://whatthefad.netlify.app)**

ask why a trend exists and it traces the thing backward: when it appeared, how it spread, what
conditions made the ground fertile. every analysis runs the same three moves — decode the sign,
name the code, expose the gap between what the trend promises and what the system actually
delivers. the gap is the insight; the rest is supporting evidence. a flattering read means the
third move didn't finish.

```
npm install     # netlify functions only — the site itself has no build step
netlify dev     # site + functions at http://localhost:8888
```

**the hard part** was that one repo holds two apps with opposite threat models. the analyst view
is bring-your-own-key: the Claude key lives in `localStorage` and calls go browser → Anthropic
directly, so the deployment costs nothing to serve no matter who shows up. the Positioning Audit
is the inverse — its staged prompts *are* the product, so both key and prompts stay server-side
behind functions. i shipped both rather than pick one, because either choice alone loses
something real.

**what it still gets wrong:** the cellular-automata spread simulation is illustrative, not
predictive. it renders a plausible diffusion regime; it does not forecast one.

### the rest of the shelf

- **[reins](https://github.com/rafaelcarlosabbariao/reins)** — clinical-trial resourcing analytics
  in pure python (reflex · pandas · plotly). point it at a trial and it reads the resourcing
  demand off that trial's own parameters. every kpi is a reactive computation over one in-memory
  model rather than a stored figure, so changing a filter recomputes the whole board.
  `pip install -r requirements.txt && reflex run`. every committed row is synthetic — a 27-trial,
  18-resource portfolio with no real people or trials in it.
- **[tiktok-service](https://github.com/rafaelcarlosabbariao/tiktok-service)** — small fastapi
  wrapper pulling trending hashtags and sounds without paying a third party for the privilege.
  `MS_TOKEN=... uvicorn app:app --reload`. the boring plumbing under a cultural signal feed, and
  it fails the way unofficial APIs fail: the token expires, and cold starts run 30–60s.
- **[sobrock_analysis](https://github.com/rafaelcarlosabbariao/sobrock_analysis)** — whether john
  mayer's *Sob Rock* is actually soft rock, put to spotify's audio features in R. a cultural
  question that turned out to have a testable shape.
- **[whats-in-that-dijon](https://github.com/rafaelcarlosabbariao/whats-in-that-dijon)** — the same
  move on dijon's production. what is in there, measured rather than described.

### what didn't work

**Supp** was a prompt app for small friend groups — three questions a day, moving playful to
personal. i shipped it, instrumented it, and it did not activate.

- **116 profiles · 51 groups · 5,039 answers**, 2025-10-25 through 2026-06-07. nothing since.
- **2 of 51 groups** ever reached three distinct responders inside a thirty-day window. **zero**
  do today. that is the whole story: the loop never closed.
- the exception is the interesting part. one group ran **1,003 answers across 8 responders and
  127 active days over a 197-day span**. the product worked, intensely, for people who already
  had the habit. it never manufactured the habit in anyone who didn't.
- what people refused is legible too. skip rate was **2.9%** on questions about another member
  and **5.3%** open-ended, against **24.2%** for photo and **32.6%** for audio. asking someone to
  perform costs roughly an order of magnitude more than asking them to answer.

i wrote a growth plan that assumed a working activation loop, then a second one, before checking
whether the loop worked. it didn't — and the numbers that disproved it were already sitting in
the database. that is the part i actually carry: instrument the assumption before you fund it.

### currently

two things, deliberately kept apart. **gossip** is the open-source one, held by its own
operating entity so ownership of an open project stays separable from the ventures that read it:
[Audience Decode](https://thegossip.io/decode/six-layers) builds a working model of an audience so
you can test a move on it before you spend, and [readtheloom.live](https://readtheloom.live) reads
the present out loud from nine live source kinds scored across eight cultural domains.

**Back2Human** is a separate social health venture i co-founded and run with a partner, now
recalibrating into an applied think tank and research service on human infrastructure.

seven years at Pfizer before that — vaccine research informatics, then clinical supply, where a
patient-level demand simulator i built replaced a third-party forecasting product.

---

nyc · [rafaelabbariao.com](https://rafaelabbariao.com) ·
[linkedin](https://www.linkedin.com/in/rafael-abbariao/)
