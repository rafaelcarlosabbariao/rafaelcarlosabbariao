## Rafael Carlos Abbariao

data scientist in new york. seven years at Pfizer — vaccine research informatics, then clinical
supply, where a demand model I built replaced a vendor product. now running **Back2Human**: a studio
in two halves, instruments that read how people actually behave and the things built on what they
read.

the method is the same everywhere. instrument it, publish the number, let the number end the
argument. sometimes the number ends the product — [Supp](https://whatssupp.app) reached 51 friend
groups and 5,039 answered prompts, activated 1.7% of the people who installed it, and got sunset
with the numbers public rather than quietly.

### what's public here

- **[cultural-archaeology](https://github.com/rafaelcarlosabbariao/cultural-archaeology)** —
  *WhatTheFad?*, live at [whatthefad.netlify.app](https://whatthefad.netlify.app). ask why a trend
  exists and it traces the thing backward: when it appeared, how it spread, what conditions made the
  ground fertile. every analysis runs the same three moves — decode the sign, name the code, expose
  the gap between what the trend promises and what the system actually delivers. the gap is the
  insight; the rest is supporting evidence. a flattering read means the third move didn't finish.
  five-lens report, cellular-automata diffusion sim, and a positioning-audit pipeline where every
  claim binds to a receipt id.
- **[reins](https://github.com/rafaelcarlosabbariao/reins)** — clinical-trial resourcing analytics
  in pure python (reflex · pandas · plotly). every kpi on screen is a reactive computation over one
  in-memory model rather than a stored figure, so changing a filter recomputes the whole board.
  runs in one command against a synthetic 27-trial portfolio.
- **[sobrock_analysis](https://github.com/rafaelcarlosabbariao/sobrock_analysis)** — whether john
  mayer's *Sob Rock* is actually soft rock, put to spotify's audio features in R. a cultural
  question that turned out to have a testable shape.
- **[tiktok-service](https://github.com/rafaelcarlosabbariao/tiktok-service)** — small fastapi
  service pulling trending hashtags and sounds without paying a third party for the privilege. the
  boring plumbing under a cultural signal feed.

### what isn't, and why

most of the last year is private — client work, and products that aren't only mine to open.

the one i'd most want to show you is a clinical-supply simulator: each patient modeled as a markov
chain walking dosing cycles, monte-carlo'd across the enrollment plan to turn enrollment uncertainty
into a daily demand curve, then inventory rolled forward site by site under an (s,S) policy with lot
expiry and lead times until something runs dry. it replaced a third-party product and saved up to
$500k per study. the reason to forecast it isn't the money — a site running out means a patient
misses a dose. ask and i'll walk you through it.

also not in this list: [rafaelabbariao.com](https://rafaelabbariao.com), a portfolio built as a
windows 98 mockup running a sql engine i wrote by hand in typescript — tokenizer, parser, evaluator
— over my own résumé as the database. querying a person is a strange thing to build. worth it
anyway.

### currently

**theGOSSIP**, the measurement half — [Audience Decode](https://peoplewatching.studio) builds a
working model of an audience so you can test a move on it before you spend, and
[readtheloom.live](https://readtheloom.live) reads the present out loud from nine live source kinds
scored across eight cultural domains.

**the built half** — [Supp](https://whatssupp.app), and then
[Close Friends Only](https://closehumans.com) when supp taught us the group chat was the
distribution and not the destination.

---

nyc · [rafaelabbariao.com](https://rafaelabbariao.com) ·
[linkedin](https://www.linkedin.com/in/rafael-abbariao/)
