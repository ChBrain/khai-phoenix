---
khai: plan
title: "Run the Cycle"
language: english
license: CC-BY-NC-SA-4.0
status: active
stamp:
  owner: Choregos (Nicias and Pericles)
  version: v0.1.0
  date: "2026-08-17"
---

# Plan: Run the Cycle

## Taxonomy

A production directive: the order in which the bestiary is built, and the reasons that fix it. Issued by the Choregos, carried by the Playwright and the Director.

## Owner

- Owner: the project, khai-phoenix

> **The first standing plan of the house.** The cycle is planned at
> 52 beasts and three exist. Nothing in the repository says which beast comes
> next or why, so the sequence lives only in a numbering that was never a
> production order. This plan fixes the running order and the reasons
> behind it, and it is the file to amend when a reason changes.

## Direction

The catalogue numbering in the plan is an index, not a schedule. It groups by
domain, which is how a reader browses, and it says nothing about what the house
can actually build next. Three things decide that instead: whether the beast has
a member to stand on, whether it collides with a beast already written, and
whether it depends on beasts that do not exist yet.

Run the cycle in waves that respect those three, so that no session opens with
the question of what to work on, and no beast is improvised because its engine
was not ready. The house builds in the order the machinery permits, and the
catalogue keeps its own order for the reader.

## Orders

1. **Finish Zunderkind.** It has its play and its captured run and no board.
   Mode B, eight Company members and four plots. It is the only beast whose
   spine is the regime rather than a named phenomenon, and the exception is
   definitional: it is fire before it is a kind of fire.

2. **Run the smoulder thread to its end, in this order:** 04 Zombiefeuer
   (`holdover`), then 05 Wurzelfresser (`duff`). They continue the descent the
   published three already made, they share a register with Moorleiche and
   Erdbaecker, and their spines are ready. 05 shares its spine with 03 and must
   differentiate by lean or be cut.

3. **Then the surface and the run:** 07 Steppenwind (`grass`), 08 Harzrausch
   (`chaparral`), 14 Funkenreiter (`spotting`). Each has a clean spine and no
   dependency on anything unwritten.

4. **Hold the crown cluster until the collision is resolved.** 09, 10, 11 and 12
   all take `process_crown` as their spine, and 11 Vollbrand is already written:
   it is the closing movement of Zunderkind, three valleys and all. Decide
   whether 11 is cut, rewritten as a separate production, or the cluster is
   differentiated by lean, before any of the four is authored.

5. **Then renewal:** 15 Aschenwiege (`serotiny`). Across the birth and the two
   real runs the fire has only ever persisted; the burn that is a beginning has
   not been claimed once. Nothing later in the cycle should be built before the
   house has staged it at least once.

6. **Hold the six that have no spine.** 06 Streufeuer, 13 Dreigesicht, 16
   Zuendwiege, 20 Geisterwolke, 26 Strahlenschlag and 35 Kaskadenbrand have no
   combustion member to stand on. Three of them appear nowhere in the engine at
   all; three exist only as description inside other members, which is enough to
   lean on and not enough to spine on. They are engine work in `khai`, not
   improvisation here.

7. **Domains 2, 3 and 4 follow in catalogue order** once Domain 1 is clear,
   since their beasts are mutually independent and no wave logic applies.

8. **52 Roestaromen is written last.** It is the only beast whose meaning depends
   on the ones before it: the renewal reads as renewal only if the cycle has
   earned the burn. It is also the only place the house speaks past its own
   science, and that licence is spent once.

## Implementation

One beast per item directory under `bestiary/`, each carrying its play, its
board, and the captured runs it has produced. The spine and leans for every
beast are fixed in the dependency map; that table is the input to this plan and
the two are amended together.

Per beast, in stages, one pull request each: the play (Mode A), then the board
(Mode B), then the captured run. Source and tests never share a branch. The
`entity/*` lane owns `bestiary/**`; `governance/*` owns this file. Every pull
request carries a changeset, empty where it ships no beast.

Four gates bite reliably and are cheaper to obey than to rediscover: a German
play needs `declared` beside its English `title`; a description is capped at 120
characters; a piece carries `Place` before `Load Bearing`; and any `place` file
must link a combustion member in `Shown`, at fail level, whatever the beast's
own spine is.

## Targets

- [x] The running order is fixed and recorded, with its reasons
- [x] The six beasts with no combustion spine are named and held
- [x] The crown collision is named as a decision, not left to discovery
- [x] The keystone is placed last, with the reason stated
- [ ] Zunderkind carries its board
- [ ] The crown collision is resolved by the Choregos
- [ ] The smoulder thread is complete: 04, 05
- [ ] The surface and run wave is complete: 07, 08, 14
- [ ] Renewal is staged at least once: 15
- [ ] The six held beasts have members in the combustion engine, or are cut
