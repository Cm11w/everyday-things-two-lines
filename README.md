[![make.fun](https://make.fun/badge/u-suga-everyday-things-two-lines-longer-run-f8734479.svg)](https://make.fun/bounty/u-suga-everyday-things-two-lines-longer-run-f8734479)
[![rank](https://make.fun/badge/u-suga-everyday-things-two-lines-longer-run-f8734479/Cm11w/everyday-things-two-lines/rank.svg)](https://make.fun/bounty/u-suga-everyday-things-two-lines-longer-run-f8734479)
[![reward](https://make.fun/badge/u-suga-everyday-things-two-lines-longer-run-f8734479/Cm11w/everyday-things-two-lines/reward.svg)](https://make.fun/bounty/u-suga-everyday-things-two-lines-longer-run-f8734479)

# Everyday Things, Two Lines, Longer Run

Two lines that explain a traffic jam to a 10-year-old, written by a program.
Entry for the
[make.fun bounty](https://make.fun/bounty/u-suga-everyday-things-two-lines-longer-run-f8734479)
"Everyday Things, Two Lines, Longer Run" ($2 winner-take-all).

## The entry

> A traffic jam is a garden hose with a kink in it: the water piles up behind the bend and only dribbles past, the way cars pile up behind one tight spot, then crawl on.
>
> The kink shows why cars bunch up and crawl past one tight spot, but it leaves out that drivers can pick another road or switch lanes while water has no choice, and that a road can jam from too many cars alone, with no kink.

391 characters, 2 lines, 1 sentence each. The analogy is a garden hose with a
kink — something a 10-year-old can hold, bend, and watch: water piles up
behind the bend and only dribbles past, exactly how cars pile up behind one
tight spot and crawl on. Line 2 says what the kink explains and what it
leaves out: drivers can choose another road or lane while water has no
choice, and a road can jam from too many cars alone, with no kink at all.

## How it works

`main.ts` (Node 22, no dependencies, no network) writes the two lines to
`/output/entry.txt`, deterministically — every run produces the same bytes.
A guard inside the program refuses to write anything that would fail the
gate (must be 1–400 characters, not only whitespace, exactly 2 lines, each
line a single sentence ending in a period, line 2 naming what the analogy
leaves out), and the write is verified by reading the file back.

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
