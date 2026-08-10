# Redstone Logic Gates — Minecraft Build Reference

Quick reference for building the five core logic gates in survival Minecraft using
redstone dust and torches. All designs are compact, survival-craftable, and work in
Java 1.21.

---

## Block key

```
R   redstone dust (one block of wire)
T   redstone torch (mounted on the side of an adjacent block)
■   solid block (stone, cobblestone, deepslate — anything solid)
A   input A
B   input B
Q   output
.   air / empty space
```

Diagrams are top-down unless noted. Torches face the direction of their output.

---

## NOT — 1 torch

Inverts the signal. A=ON gives Q=OFF. A=OFF gives Q=ON.

```
A ━━━ ■ T━━━ Q
      ↑
  torch mounted on
  the right side of block
```

**Build:** Run dust from A into the left side of a solid block. Mount a torch on
the right side of that same block. The torch output becomes Q.

**How it works:** Powering the block (via A) extinguishes the torch. When A is
off the torch stays lit and Q is high. The block is the inversion point.

| A | Q |
|---|---|
| 0 | 1 |
| 1 | 0 |

---

## OR — 0 torches

Either input ON gives output ON.

```
A ━━━┓
     ┣━━━ Q
B ━━━┛
```

**Build:** Run dust from A and dust from B so they meet at the same junction.
Any dust continuing from that junction is Q. No extra components needed.

**How it works:** Redstone dust combines signals naturally — any powered path
reaching a node keeps it powered. This is the simplest gate, but also the one
Minecraft gives you for free.

| A | B | Q |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

---

## AND — 3 torches

Both inputs must be ON for output to be ON.

```
A ━━━ ■ T━┓
          ┣━━━ ■ T━━━ Q
B ━━━ ■ T━┛
```

**Build:**
1. A into a block → torch T1 on right side of that block
2. B into a block → torch T2 on right side of that block
3. T1 and T2 outputs both feed into a third block
4. Torch T3 on that third block — its output is Q

**How it works:** Uses De Morgan's law under the hood. T1 inverts A, T2 inverts B.
Their outputs are OR'd into T3, which inverts again.
NOT(NOT A OR NOT B) = A AND B.

When both inputs are ON: T1 and T2 both go off, third block loses power, T3 turns
on. Wait — that's wrong. Let's walk it through carefully:

- A=1, B=1 → T1 off, T2 off → third block unpowered → T3 on → Q = 1 ✓
- A=1, B=0 → T1 off, T2 on → third block powered → T3 off → Q = 0 ✓
- A=0, B=0 → T1 on, T2 on → third block powered → T3 off → Q = 0 ✓

| A | B | Q |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 1 | 1 |

---

## NAND — 2 torches

Output is OFF only when both inputs are ON. Inverse of AND. Actually simpler
to build than AND — it just drops the final inverting torch.

```
A ━━━ ■ T━┓
          ┣━━━ Q
B ━━━ ■ T━┛
```

**Build:**
1. A into a block → torch T1
2. B into a block → torch T2
3. Both torch outputs feed into a shared dust junction — that junction is Q

**How it works:** When both A and B are on, both torches go off and Q drops.
Any other combination keeps at least one torch lit.

| A | B | Q |
|---|---|---|
| 0 | 0 | 1 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 0 |

---

## NOR — 1 torch

Output is ON only when BOTH inputs are OFF. OR then inverted.

```
A ━━━┓
     ┣━━━ ■ T━━━ Q
B ━━━┛
```

**Build:**
1. Merge A and B dust at a junction (the OR step)
2. Run that merged signal into a solid block
3. Torch on that block — output is Q

**How it works:** If either input is on, the block is powered and the torch goes
off (Q=0). Only when both inputs are off does the block stay dark, keeping the
torch lit (Q=1).

NOR is actually one of the most useful gates in practice — your braking circuit
is essentially a NOR with one input tied high.

| A | B | Q |
|---|---|---|
| 0 | 0 | 1 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 1 | 0 |

---

## XOR — 5 torches

Output is ON when inputs differ. The most complex gate to build.

```
     ┏━━━ ■ T1 ━━━━━━━━━━━━━━━━━━┓
     ┃                           ┃
A ━━━╋━━━━━━━━━━━━━━━━━━━━━━━━━━━╋━━━ ■ T5 ━━━ Q
     ┃                           ┃
     ┗━━━ ■ T3(NOR) ━━━━━━━━━━━━┛
     ┃         ↑
B ━━━╋━━━━━━━━━┛
     ┃
     ┗━━━ ■ T2 ━━━━━━━━━━━━━━━━━━┛ (also feeds T5 block)
```

The ASCII gets messy at this complexity. Here is the cleaner verbal build:

**Build — 5 steps:**

1. **T1:** A into a block → torch. Output = NOT A
2. **T2:** B into a block → torch. Output = NOT B
3. **T3 (NOR):** Both A and B feed into a block → torch. Output = NOR(A,B)
   — this is high only when both inputs are off
4. **T4:** Feed T3's output and NOT-A (from T1) into a block → torch
5. **T5:** Combine T4's output and NOT-B (from T2) into a block → torch.
   Output of T5 is Q

**Practical note:** XOR needs roughly 10×4 blocks of space. Build it in a flat
test area first before integrating into a real circuit. Most practical redstone
(farms, gates, launchers, brakes) never actually requires XOR — it mainly shows
up in binary adders and counters.

| A | B | Q |
|---|---|---|
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 0 |

---

## Materials at a glance

| Gate | Torches | Solid blocks | Dust runs |
|------|---------|--------------|-----------|
| NOT  | 1       | 1            | short     |
| OR   | 0       | 0            | short     |
| AND  | 3       | 3            | medium    |
| NAND | 2       | 2            | medium    |
| NOR  | 1       | 1            | short     |
| XOR  | 5       | 5            | long      |

---

## Build order recommendation

1. **NOT** — one torch, teaches the inversion mechanic everything else relies on
2. **NOR** — OR + NOT, immediately useful (your brake circuit is close to this)
3. **NAND** — two torches, teaches the inverted-inputs pattern
4. **AND** — NAND with one more torch chained on the end
5. **OR** — trivially simple, save it for when you need a merge point
6. **XOR** — last, only when you actually need it

---

## Common pitfall: torch burnout

If you feed a signal into a torch loop that updates too fast (sub-tick), Minecraft
will detect the infinite loop and burn the torch out — it goes permanently dark and
drops as an item. If a torch mysteriously disappears, this is why. Add a repeater
set to 2–4 ticks anywhere in the loop to slow the signal down.
