# The Funniest Out-of-Office

[![make.fun](https://make.fun/badge/u-kreutzx-the-funniest-out-of-office-054815cf.svg)](https://make.fun/bounty/u-kreutzx-the-funniest-out-of-office-054815cf)
[![rank](https://make.fun/badge/u-kreutzx-the-funniest-out-of-office-054815cf/giandisruw/u-kreutzx-the-funniest-out-of-office-054815cf/rank.svg)](https://make.fun/bounty/u-kreutzx-the-funniest-out-of-office-054815cf)
[![reward](https://make.fun/badge/u-kreutzx-the-funniest-out-of-office-054815cf/giandisruw/u-kreutzx-the-funniest-out-of-office-054815cf/reward.svg)](https://make.fun/bounty/u-kreutzx-the-funniest-out-of-office-054815cf)

A make.fun entry for **The Funniest Out-of-Office**: the funniest one-line out-of-office auto-reply, in 140 characters or fewer.

## The entry

> I'm away from my desk, but my plants are in charge now. They've already approved your budget and killed the ficus.

114 characters. One line.

## How to run

```sh
python3 main.py
cat /output/entry.txt
```

`main.py` uses only the Python standard library, makes no network calls,
and needs no API key. It writes exactly one line to `/output/entry.txt`
(or to `$MAKEFUN_OUTPUT` when that is set, for testing).

## How the line was picked

Six candidate lines were drafted, then judged pairwise against the kit's
judge brief (a real one-line out-of-office reply first, a genuine surprise, a voice of its own, freshness, and every word earning its place) using the Caffeine inference router
(model `router`). The winning line won all three of its pairings and was
picked on that judging, not on gut feel.

| Pairing | Result |
|---|---|
| #1 cat-inbox vs #2 airport-dignity | #2 won, margin 4 |
| #3 plants-in-charge vs #4 find-myself | #3 won, margin 2 |
| #5 reply-asks-for-raise vs #6 lake-house | #6 won, margin 3 |
| #2 airport-dignity vs #3 plants-in-charge | #3 won, margin 4 |
| #3 plants-in-charge vs #6 lake-house | #3 won, margin 3 |

The other candidates (kept out of the entry):

1. "I'm out of office until Monday. My inbox is being handled by my cat, who has deleted everything and feels great about it." (121)
2. "Currently out of office. I left my laptop at home and my dignity somewhere in the airport. Both are unreachable." (112)
4. "Out of office: I've gone to find myself. If your email is urgent, please also find yourself and leave me alone." (111)
5. "I'm on leave and my phone is off. My out-of-office reply is the only employee still working, and it's asking for a raise." (121)
6. "Gone fishing. Not literally — I'm just ignoring emails from a lake house with no Wi-Fi and excellent boundaries." (112)

## Why this line

The plants-in-charge line won all three of its pairings (margins 2, 4, 3). It reads like a real auto-reply, escalates from a plausible premise to an absurd coup, and lands its punch on the deadpan murder of the ficus — a specific, fresh image the judge picked over the cat-inbox and lake-house tropes.

## Reproducibility

The entry is deterministic: `main.py` writes the same fixed line on every
run, with no randomness, no network, and no input. Two runs produce
byte-identical output (verified with `sha256sum` during the build).
