# Fuga Romana

A Minecraft-style Latin escape game for Common Entrance Levels 1, 2, 3 and Scholarship. Open `index.html` in a browser, or turn on GitHub Pages for this repository. There is nothing to install.

This is the single home of Fuga Romana. It replaces the two earlier versions, [Escape-room](https://github.com/JE2950/Escape-room) (the illustrated edition) and [Escaperoom2](https://github.com/JE2950/Escaperoom2) (the plain Level 1 edition). Both now redirect here, and their old versions are kept on backup branches.

## Stories

Four stories, each with five places and three locks in each place: 15 Latin questions per story.

1. **Escape from Pompeii**
2. **The Ides of March**
3. **The Fall of Troy**
4. **The Cyclops**

The stories are separate from the CE levels. Any story can be played at any level.

## Choosing the level

The grammar panel on the title screen lists every grammar point in Bass's order, grouped by level. The preset buttons tick a whole level at once:

| Preset | Bass chapters | Sentences in the bank |
|---|---|---|
| Ch 1–8 up to Whole of Level 1 | 2–73 | 477 |
| Level 2 | 74–116 | 318 |
| Whole of Level 3 | 117–140 | 264 |
| Scholarship | 141–154 | 172 |

Ticking any point from a higher level assumes every point from the levels below it. A Level 3 game draws all 15 questions from Level 3 grammar, and may use Level 1 and 2 grammar inside those sentences.

### Level 3 grammar points

Passive (present, imperfect, future), perfect passive, pluperfect passive, volo and nolo, expressions of time, fero, relative clauses, present participles, purpose clauses, indirect commands, perfect participle passive, and place (domus, rus, Roma).

### Scholarship grammar points

Ablative absolute, indirect statement with the present infinitive, the present infinitive passive, indirect statement with the perfect infinitive, deponent verbs, cum + subjunctive, and deponent perfect participles.

## Question types

Translate (choose the English), unscramble the Latin, choose the right form for a gap, and parse a word (person and number, case and number, or tense). The grammar table button shows the relevant table; untick it on the title screen for assessment mode.

## The question bank

The bank sits in the `BANK` section of `index.html`. Each line reads:

```
T(chapter, 'latin', 'English', 'grammar tags', ['wrong 1', 'wrong 2', 'wrong 3'], { u, g, p })
```

Grammar tags are listed in `GRAMMAR` near the top of the script: A–R for Level 1, S–e for Level 2, f–q for Level 3 and r–x for Scholarship.

All Latin comes from the exercises in *Prep School Latin* (R. C. Bass, 2018), apart from 15 sentences carried over from the first illustrated Fuga Romana. The English translations and wrong options were written for this game, as Bass prints no answer key.

## Backups

Before every push, the live version is saved as a branch named `backup/<date>-<label>`. To go back, check out that branch, or open it on GitHub and copy its files over `main`.

## Licence

Latin sentences and grammar from *Prep School Latin* (R. C. Bass, 2018), used under a Creative Commons Attribution-NonCommercial-ShareAlike licence. This game is shared under the same licence.
