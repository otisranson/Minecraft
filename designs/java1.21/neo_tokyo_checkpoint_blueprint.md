# The Checkpoint — Neo-Tokyo District Gatehouse

**Footprint:** 20 blocks wide (X) × 10 blocks deep (Z)
**Height:** 12 layers (Y=0 to Y=11), plus cupola lantern detail on top
**Style:** Blackstone + deepslate brick, lime-green and magenta backlit glass, orange/black hazard-stripe lintel, iron bar cage
**Seed:** 2417470717322115627 · Java 1.21
**Anchor build for:** Neo-Tokyo Cyberpunk District (flattened mountain footprint, X≈-243 to -117, Z≈698 to 919, Y=72)

---

## Concept

The first structure travelers hit crossing into the district — a literal border checkpoint. Two heavily fortified guard towers flank an open passage tunnel. Deliberately squat and wide rather than tall, so it reads as authority/infrastructure against the taller spires that will rise around it later.

> **Placement suggestion:** Build near the east edge of the flattened footprint (X≈-117), oriented so the passage tunnel (the Z-axis in this blueprint) runs in whichever direction leads from the approach side into the district interior. Local Y=0 in this blueprint should sit at world Y=72, matching your flatten level.

---

## Orientation

- **Z=0** = front face (approach side — outside the district)
- **Z=9** = back face (district interior side)
- **X=0** = west outer wall of left tower
- **X=19** = east outer wall of right tower
- **Y=0** = platform surface (world Y=72)

Flatten and clear at least 20×10 before starting, plus a few extra blocks of clearance on all sides for approach paths.

---

## Zones

| Zone | X range | Width |
|------|---------|-------|
| Left guard tower | X=0–5 | 6 |
| Passage (open tunnel) | X=6–13 | 8 |
| Right guard tower | X=14–19 | 6 |

---

## Block Key

| Code | Block |
|------|-------|
| `k` | Blackstone |
| `w` | Deepslate bricks |
| `p` | Polished blackstone (passage floor) |
| `d` | Deepslate brick slab (roof/cap) |
| `g` | Lime green stained glass |
| `m` | Magenta stained glass |
| `o` | Orange terracotta (hazard stripe) |
| `b` | Black concrete (hazard stripe) |
| `r` | Iron bars |
| `l` | Sea lantern |
| `.` | Air |

---

## Layers

### Y=0 — Foundation Floor

Blackstone under both towers, polished blackstone pavement through the passage (this is your walkable floor).

```
Z=0  kkkkkkppppppppkkkkkk
Z=1  kkkkkkppppppppkkkkkk
Z=2  kkkkkkppppppppkkkkkk
Z=3  kkkkkkppppppppkkkkkk
Z=4  kkkkkkppppppppkkkkkk
Z=5  kkkkkkppppppppkkkkkk
Z=6  kkkkkkppppppppkkkkkk
Z=7  kkkkkkppppppppkkkkkk
Z=8  kkkkkkppppppppkkkkkk
Z=9  kkkkkkppppppppkkkkkk
     01234567890123456789  ← X
```

---

### Y=1 — Tower Base (Passage Open)

Solid deepslate brick tower mass on both sides. The passage between them is a full open-air tunnel — no walls needed here, the inner tower faces (X=5 and X=14) form the tunnel walls naturally.

```
Z=0  wwwwww........wwwwww
Z=1  wwwwww........wwwwww
Z=2  wwwwww........wwwwww
Z=3  wwwwww........wwwwww
Z=4  wwwwww........wwwwww
Z=5  wwwwww........wwwwww
Z=6  wwwwww........wwwwww
Z=7  wwwwww........wwwwww
Z=8  wwwwww........wwwwww
Z=9  wwwwww........wwwwww
     01234567890123456789  ← X
```

> **Barrier arm (optional detail):** Place two fence posts at X=9 and X=10, Z=0, Y=1–2, with a lever nearby. Purely aesthetic unless you want to wire it to open/close — treat it as a lowered crossing barrier at the entrance.

---

### Y=2 — Tower Base (Solid, No Windows)

_(Grid identical to Y=1)_

---

### Y=3 — Window Slit Row 1

Front and back faces get a single backlit window column per tower. Lime green on the left tower, magenta on the right — your primary and secondary district accent colors.

```
Z=0  wwgwww........wwwmww
Z=1  wwwwww........wwwwww
Z=2  wwwwww........wwwwww
Z=3  wwwwww........wwwwww
Z=4  wwwwww........wwwwww
Z=5  wwwwww........wwwwww
Z=6  wwwwww........wwwwww
Z=7  wwwwww........wwwwww
Z=8  wwwwww........wwwwww
Z=9  wwgwww........wwwmww
     01234567890123456789  ← X
```

> Place a sea lantern directly behind each glass block (one block further into the tower mass) for the backlit glow.

---

### Y=4 — Solid Gap Layer

_(Grid identical to Y=1)_

---

### Y=5 — Solid Gap Layer

_(Grid identical to Y=1)_

---

### Y=6 — Window Slit Row 2

Same window positions as Y=3, second row up.

_(Grid identical to Y=3)_

---

### Y=7 — Hazard Stripe Lintel

The passage opening closes here into a striped warning beam spanning the full tunnel depth — this is the header you walk under, both entering and exiting.

```
Z=0  wwwwwwobobobobwwwwww
Z=1  wwwwwwobobobobwwwwww
Z=2  wwwwwwobobobobwwwwww
Z=3  wwwwwwobobobobwwwwww
Z=4  wwwwwwobobobobwwwwww
Z=5  wwwwwwobobobobwwwwww
Z=6  wwwwwwobobobobwwwwww
Z=7  wwwwwwobobobobwwwwww
Z=8  wwwwwwobobobobwwwwww
Z=9  wwwwwwobobobobwwwwww
     01234567890123456789  ← X
```

> **Optional detail:** Add iron bars on the underside of this beam facing into the tunnel (X=6–13, hanging at Z=0 and Z=9 edges) for a caged, oppressive feel looking up as you pass through.

---

### Y=8 — Passage Roof

The tunnel closes here with a deepslate slab roof. Towers keep rising past this point.

```
Z=0  wwwwwwddddddddwwwwww
Z=1  wwwwwwddddddddwwwwww
Z=2  wwwwwwddddddddwwwwww
Z=3  wwwwwwddddddddwwwwww
Z=4  wwwwwwddddddddwwwwww
Z=5  wwwwwwddddddddwwwwww
Z=6  wwwwwwddddddddwwwwww
Z=7  wwwwwwddddddddwwwwww
Z=8  wwwwwwddddddddwwwwww
Z=9  wwwwwwddddddddwwwwww
     01234567890123456789  ← X
```

---

### Y=9 — Cupola Walls (Level 1)

A watch cupola rises centered on the passage roof (X=8–11), flanked by flat walkable roof (X=6–7 and X=12–13). Towers continue solid alongside it. Front and back faces of the cupola are glass; the sides are solid.

**Front/back rows (Z=0 and Z=9):**
```
wwwwwwddggggddwwwwww
```

**Middle rows (Z=1–8):**
```
wwwwwwddwwwwddwwwwww
```

Full layer:
```
Z=0  wwwwwwddggggddwwwwww
Z=1  wwwwwwddwwwwddwwwwww
Z=2  wwwwwwddwwwwddwwwwww
Z=3  wwwwwwddwwwwddwwwwww
Z=4  wwwwwwddwwwwddwwwwww
Z=5  wwwwwwddwwwwddwwwwww
Z=6  wwwwwwddwwwwddwwwwww
Z=7  wwwwwwddwwwwddwwwwww
Z=8  wwwwwwddwwwwddwwwwww
Z=9  wwwwwwddggggddwwwwww
     01234567890123456789  ← X
```

---

### Y=10 — Cupola Walls (Level 2)

_(Grid identical to Y=9)_

---

### Y=11 — Roof Cap (Crenellation + Cupola Roof)

Cupola and flat roof close over with slabs. Both towers finish with a simple alternating crenellation (full block / slab) for a battlement silhouette.

```
Z=0  wdwdwddddddddwdwdwdw
Z=1  wdwdwddddddddwdwdwdw
Z=2  wdwdwddddddddwdwdwdw
Z=3  wdwdwddddddddwdwdwdw
Z=4  wdwdwddddddddwdwdwdw
Z=5  wdwdwddddddddwdwdwdw
Z=6  wdwdwddddddddwdwdwdw
Z=7  wdwdwddddddddwdwdwdw
Z=8  wdwdwddddddddwdwdwdw
Z=9  wdwdwddddddddwdwdwdw
     01234567890123456789  ← X
```

---

### Finishing Details (No Grid Needed)

- **Cupola lantern:** Place 1–2 sea lantern blocks on top of the cupola roof, centered around X=9–10, Z=4–5, for a rooftop beacon glow.
- **Guard overlook (optional):** Add a small barred window on the inner tower faces (X=5 and X=14) around Y=3–4, facing into the tunnel, so it reads as a manned checkpoint watching the passage.
- **Corner finials (optional):** A single dark oak fence post or lantern on each of the four tower-top corners adds a subtle vertical accent above the crenellation line.
- **Approach paths:** Consider a short run of polished blackstone or blackstone slabs extending a few blocks out from Z=0 and Z=9 to mark the checkpoint's "lanes" before the district streets are built out.

---

## Total Materials List (Approximate)

| Block | Quantity |
|-------|----------|
| Deepslate bricks | ~700 |
| Deepslate brick slab | ~200 |
| Blackstone | ~150 |
| Polished blackstone | ~80 |
| Orange terracotta | ~40 |
| Black concrete | ~40 |
| Iron bars | ~40 |
| Lime green stained glass | ~20 |
| Magenta stained glass | ~20 |
| Sea lantern | ~6 |
| Fence | ~4 |
| Lever | 1 |

> Deepslate bricks and slabs dominate again here — same as Ironhold, stockpile before starting.

---

## Build Tips

- **Build order:** Complete one full Y layer before moving to the next, same discipline as Ironhold.
- **Lighting:** Sea lanterns behind every glass panel double as both the neon effect and practical mob-spawn prevention — don't skip them even on layers where it's not called out explicitly.
- **The passage is the whole point:** Don't rush the hazard stripe (Y=7) or the roof (Y=8) — that transition from "open sky tunnel" to "caged, striped, roofed corridor" is what sells the checkpoint feeling as you walk through.
- **Future expansion:** This building intentionally stays low and wide. When you start adding taller spires around it later, the checkpoint should read as the oldest, most "official" structure in the district — everything else can be visually louder.
- **Scaling up:** If the passage feels too tight once you're standing in it, widen X=6–13 symmetrically (e.g. to X=5–14) and adjust tower zones accordingly — the layer logic doesn't change, just the column counts.
