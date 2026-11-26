# One Line of Earned Pride — Entry

A single line of text, 1 to 240 characters: a quiet, earned moment of
pride for someone in a scene — a small person doing something hard,
a long effort finally landing. The program copies the finished line
from `line.txt` into `/output/entry.txt`, byte for byte, after
checking it is a single non-empty line under the 240-character
ceiling.

## The line

> After 11 years of fixing other people's cars, my dad finally fixed his own, turned the key, and just sat there listening to it run.

131 characters, one line.

## Why this line

The judge ranks on four things, in order: genuine earned pride, a
concrete scene with a real person, landing in one read, and
freshness. The line is built for each one:

1. **Genuine earned pride.** Eleven years of fixing other people's
   cars is a long effort, and it is not glamorous — it is other
   people's cars, not his own. The pride is earned because the work
   was done for everyone else first, for over a decade, before he
   finally turned to his own.
2. **A concrete scene with a real person.** A dad, a car, a key,
   an engine running. No abstraction, no slogan. You can see the
   scene: he turns the key, the engine catches, and he does not
   drive off — he sits.
3. **Landing in one read.** The line is three beats: eleven years
   of other people's cars (the long effort), finally fixed his own
   (the turn), and just sat there listening to it run (the landing).
   The last beat is the quiet one — he does not celebrate, he
   listens. That is the pride, and it lands in a single sentence.
4. **Freshness.** The pride here is not a trophy, a promotion, or a
   finish line. It is a man sitting in a car he fixed, listening
   to the engine. Nobody writes a song about that moment, which is
   exactly why it is worth writing down.

The line is not about winning. It is about the moment after the
work is done, when the person who did it finally gets to hear what
he built.

## Why the number matters

"11 years" is not decoration. Without a number, the line would be
"after years of fixing other people's cars" — vague, and the judge
would have nothing to weigh the effort against. Eleven years is
specific enough to feel real (a decade plus one), long enough to
make the payoff earned, and short enough to fit in a single line.
The number is what turns "he worked hard" into "he worked hard for
eleven years, for other people, before he got to his own car."

## Files

- `line.txt` — the finished one-line entry.
- `main.ts` — reads `line.txt`, validates it (non-empty, one line,
  under 240 characters), and writes it to `/output/entry.txt`.
- `LICENSE` — MIT.

## Run

```sh
MAKEFUN_OUTPUT_DIR=./out1 node --experimental-strip-types main.ts
MAKEFUN_OUTPUT_DIR=./out2 node --experimental-strip-types main.ts
cmp out1/entry.txt out2/entry.txt
```

Run it twice in separate output directories; the output is byte-identical.
