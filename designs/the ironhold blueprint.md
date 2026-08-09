# The Ironhold

**Type:** House (fortified manor with corner towers)
**Version/Edition:** Java 1.21

## Overview

A 24×20 footprint, 15-layer-tall fortified house: deepslate brick walls with dark oak log pilasters, full-bay glass windows, and four crenellated corner towers.

- **Footprint:** 24 blocks wide (X) × 20 blocks deep (Z)
- **Height:** 15 layers (Y=0 to Y=14)
- **Style:** Deepslate bricks, dark oak log pilasters, full-bay glass windows, crenellated corner towers
- **Seed:** 2417470717322115627 · Java 1.21 · Near spawn (X≈-32, Z≈-1)

**What makes this build different**

- **Dark oak log pilasters** run the full 10-block height on all four faces, every 8 blocks — they break up flat walls and cast real shadow lines visible from a distance
- **Full-bay windows** — instead of small punched holes, each bay between pilasters is entirely glass (3 rows tall on ground floor, 2 on upper floor)
- **Four corner towers** — the 4×4 corners keep rising through Y=11–14 while the main roof ends at Y=11, giving 3 blocks of tower above the roofline
- **Iron bar overlook** — Y=7 front face lets you look down from the upper floor into the great hall below
- **Two-tone upper floor** — spruce planks (bedroom left) and dark oak planks (map room right) without needing a dividing wall

> **Warning:** This build uses a lot of deepslate bricks. Get your deepslate mine running before laying the first block.

---

## Materials

| Block | Quantity |
|-------|----------|
| Deepslate bricks | ~620 |
| Smooth stone | ~396 |
| Deepslate brick slab | ~280 |
| Glass pane | ~300 |
| Spruce planks | ~198 |
| Dark oak planks | ~198 |
| Dark oak log | ~60 |
| Bookshelf | 16 |
| Chest | 6 |
| Furnace | 6 |
| Oak door | 2 |
| Iron bars | 3 |
| Crafting table | 1 |
| Enchanting table | 1 |

> Deepslate bricks is the biggest ask by far — stock up before you start. Mine deepslate, smelt to cobbled deepslate, craft into bricks.
> Bookshelves require 6 planks + 3 books each (books = 3 paper + 1 leather). You need 16 total.
> Glass panes are crafted from glass blocks (6 blocks → 16 panes). You'll need to smelt a lot of sand.

---

## Notes

### Orientation

- **Z=0** = front face (door/south side)
- **Z=19** = back face
- **X=0** = west wall
- **X=23** = east wall
- **Y=0** = platform surface (start here)

Extend your platform to at least 24×20 before starting.

### Block Key

| Code | Block |
|------|-------|
| `w` | Deepslate bricks |
| `l` | Dark oak log (pilaster) |
| `s` | Smooth stone |
| `p` | Dark oak planks |
| `b` | Spruce planks |
| `h` | Deepslate brick slab |
| `g` | Glass pane |
| `r` | Iron bars |
| `d` | Oak door (lower — place here) |
| `D` | Oak door (upper — auto-placed, do not place) |
| `K` | Bookshelf |
| `E` | Enchanting table |
| `T` | Crafting table |
| `X` | Chest |
| `F` | Furnace |
| `.` | Air (empty) |

### Pilaster positions

Pilasters (dark oak logs `l`) appear at the following positions on each face, replacing what would otherwise be a wall brick:

- **Front/back faces (Z=0 and Z=19):** X=0, X=8, X=16, X=23
- **Side faces (X=0 and X=23):** Z=0, Z=7, Z=13, Z=19

### Layers

#### Y=0 — Foundation Floor

Lay directly on your platform. Deepslate brick perimeter, smooth stone interior, dark oak logs at corners and mid-wall pilaster positions.

```
Z=0  lwwwwwwwlwwwwwwwlwwwwwwl
Z=1  wssssssssssssssssssssssw
Z=2  wssssssssssssssssssssssw
Z=3  wssssssssssssssssssssssw
Z=4  wssssssssssssssssssssssw
Z=5  wssssssssssssssssssssssw
Z=6  wssssssssssssssssssssssw
Z=7  wssssssssssssssssssssssw
Z=8  wssssssssssssssssssssssw
Z=9  wssssssssssssssssssssssw
Z=10 wssssssssssssssssssssssw
Z=11 wssssssssssssssssssssssw
Z=12 wssssssssssssssssssssssw
Z=13 wssssssssssssssssssssssw
Z=14 wssssssssssssssssssssssw
Z=15 wssssssssssssssssssssssw
Z=16 wssssssssssssssssssssssw
Z=17 wssssssssssssssssssssssw
Z=18 wssssssssssssssssssssssw
Z=19 lwwwwwwwlwwwwwwwlwwwwwwl
     012345678901234567890123  ← X
```

#### Y=1 — Ground Floor (Entrance + Furniture)

Double oak door at X=11,12 (center front). Enchanting horseshoe left wing: 16 bookshelves around table at X=5, Z=8 — max level 30. Crafting table X=14, Z=3. Six chests at Z=17, six furnaces at Z=18 (right side back wall).

```
Z=0  lwwwwwwwlwwddwwwlwwwwwwl
Z=1  w......................w
Z=2  w......................w
Z=3  w.............T........w
Z=4  w......................w
Z=5  w......................w
Z=6  w..KKKKK...............w
Z=7  l..K...K...............l
Z=8  w..K.E.K...............w
Z=9  w..K...K...............w
Z=10 w..KKKKK...............w
Z=11 w......................w
Z=12 w......................w
Z=13 l......................l
Z=14 w......................w
Z=15 w......................w
Z=16 w......................w
Z=17 w............XXXXXX....w
Z=18 w............FFFFFF....w
Z=19 lwwwwwwwlwwwwwwwlwwwwwwl
     012345678901234567890123  ← X
```

> **Enchanting table:** X=5, Z=8
> **Bookshelves:** Z=6 (X=3–7), Z=7 (X=3, X=7), Z=8 (X=3, X=7), Z=9 (X=3, X=7), Z=10 (X=3–7). All 16 within Chebyshev distance 2 of table with clear air between them — fully functional for max enchanting.
> **Doors:** Place both oak doors at Y=1. Upper halves at Y=2 are automatic.
> **Ladder:** Place ladder blocks at X=12, Z=2 on the north wall face, running Y=1 up to Y=5 for upper floor access.

#### Y=2 — Ground Floor Walls (Windows + Door Top)

Full bay-width glass panes between each pilaster. Door upper half at X=11,12 is auto-placed.

```
Z=0  lgggggglggDDgggglggggggl
Z=1  g......................g
Z=2  g......................g
Z=3  g......................g
Z=4  g......................g
Z=5  g......................g
Z=6  g......................g
Z=7  l......................l
Z=8  g......................g
Z=9  g......................g
Z=10 g......................g
Z=11 g......................g
Z=12 g......................g
Z=13 l......................l
Z=14 g......................g
Z=15 g......................g
Z=16 g......................g
Z=17 g......................g
Z=18 g......................g
Z=19 lgggggglgggggggglggggggl
     012345678901234567890123  ← X
```

#### Y=3 — Ground Floor Walls (2nd Window Row)

Same pattern as Y=2. No door markers — solid wall where the door was.

```
Z=0  lgggggglgggggggglggggggl
Z=1  g......................g
Z=2  g......................g
Z=3  g......................g
Z=4  g......................g
Z=5  g......................g
Z=6  g......................g
Z=7  l......................l
Z=8  g......................g
Z=9  g......................g
Z=10 g......................g
Z=11 g......................g
Z=12 g......................g
Z=13 l......................l
Z=14 g......................g
Z=15 g......................g
Z=16 g......................g
Z=17 g......................g
Z=18 g......................g
Z=19 lgggggglgggggggglggggggl
     012345678901234567890123  ← X
```

#### Y=4 — Ground Floor Walls (3rd Window Row)

Same as Y=3. Three full rows of glazing (Y=2, 3, 4) creates dramatic floor-to-ceiling windows on the ground floor.

_(Grid identical to Y=3)_

#### Y=5 — Ground Floor Wall Top (Solid)

Solid deepslate brick wall closes the ground floor (5 blocks tall: Y=1–5). Dark oak log pilasters continue through here.

```
Z=0  lwwwwwwwlwwwwwwwlwwwwwwl
Z=1  w......................w
Z=2  w......................w
Z=3  w......................w
Z=4  w......................w
Z=5  w......................w
Z=6  w......................w
Z=7  l......................l
Z=8  w......................w
Z=9  w......................w
Z=10 w......................w
Z=11 w......................w
Z=12 w......................w
Z=13 l......................l
Z=14 w......................w
Z=15 w......................w
Z=16 w......................w
Z=17 w......................w
Z=18 w......................w
Z=19 lwwwwwwwlwwwwwwwlwwwwwwl
     012345678901234567890123  ← X
```

#### Y=6 — Upper Floor (Bedroom Left + Map Room Right)

Spruce planks (X=1–11) = bedroom. Dark oak planks (X=12–22) = map room/study. Two-tone floor divides the space without a wall.

```
Z=0  lwwwwwwwlwwwwwwwlwwwwwwl
Z=1  wbbbbbbbbbbbpppppppppppw
Z=2  wbbbbbbbbbbbpppppppppppw
Z=3  wbbbbbbbbbbbpppppppppppw
Z=4  wbbbbbbbbbbbpppppppppppw
Z=5  wbbbbbbbbbbbpppppppppppw
Z=6  wbbbbbbbbbbbpppppppppppw
Z=7  lbbbbbbbbbbbpppppppppppl
Z=8  wbbbbbbbbbbbpppppppppppw
Z=9  wbbbbbbbbbbbpppppppppppw
Z=10 wbbbbbbbbbbbpppppppppppw
Z=11 wbbbbbbbbbbbpppppppppppw
Z=12 wbbbbbbbbbbbpppppppppppw
Z=13 lbbbbbbbbbbbpppppppppppl
Z=14 wbbbbbbbbbbbpppppppppppw
Z=15 wbbbbbbbbbbbpppppppppppw
Z=16 wbbbbbbbbbbbpppppppppppw
Z=17 wbbbbbbbbbbbpppppppppppw
Z=18 wbbbbbbbbbbbpppppppppppw
Z=19 lwwwwwwwlwwwwwwwlwwwwwwl
     012345678901234567890123  ← X
```

> **Bed:** Place at X=2–3, Z=14–15 (bedroom left side).
> **Map wall:** Leave Z=19 back wall (X=12–22) bare — place item frames here for your exploration map display.
> **Ladder access:** The ladder from Y=1 terminates at this floor. Break one block at X=12, Z=2 in this layer so the ladder has somewhere to arrive.

#### Y=7 — Upper Floor Walls L1 (Iron Bar Overlook)

Iron bars at X=10,11,12 on the front face create an interior overlook above the entrance. Solid deepslate brick everywhere else.

```
Z=0  lwwwwwwwlwrrrwwwlwwwwwwl
Z=1  w......................w
Z=2  w......................w
Z=3  w......................w
Z=4  w......................w
Z=5  w......................w
Z=6  w......................w
Z=7  l......................l
Z=8  w......................w
Z=9  w......................w
Z=10 w......................w
Z=11 w......................w
Z=12 w......................w
Z=13 l......................l
Z=14 w......................w
Z=15 w......................w
Z=16 w......................w
Z=17 w......................w
Z=18 w......................w
Z=19 lwwwwwwwlwwwwwwwlwwwwwwl
     012345678901234567890123  ← X
```

#### Y=8 — Upper Floor Walls (Windows)

Full bay-width windows matching the ground floor pattern. From outside, both stories show aligned window bays framed by the continuous pilasters.

_(Grid identical to Y=3 — full bay glass on all faces, pilasters at Z=7 and Z=13 on sides)_

#### Y=9 — Upper Floor Walls (2nd Window Row)

Second row of upper floor windows. Same as Y=8.

_(Grid identical to Y=8)_

#### Y=10 — Upper Floor Wall Top (Solid)

Solid wall closes the upper floor. Dark oak log pilasters complete their full 10-block vertical run (Y=1–10). Above this the main roof begins and the corner towers continue rising.

_(Grid identical to Y=5)_

#### Y=11 — Main Roof + Corner Tower Bases

Deepslate slabs fill the main roof. Battlements ring the perimeter — alternating raised bricks and flat slabs. The four corner sections (X=0–3 and X=20–23, at Z=0–3 and Z=16–19) continue as solid tower walls above the roofline.

```
Z=0  wwwwhwhwhwhwhwhwhwhwwwww
Z=1  wwwwhhhhhhhhhhhhhhhhwwww
Z=2  wwwwhhhhhhhhhhhhhhhhwwww
Z=3  wwwwhhhhhhhhhhhhhhhhwwww
Z=4  whhhhhhhhhhhhhhhhhhhhhhhw
Z=5  hhhhhhhhhhhhhhhhhhhhhhhh
Z=6  whhhhhhhhhhhhhhhhhhhhhhhw
Z=7  hhhhhhhhhhhhhhhhhhhhhhhh
Z=8  whhhhhhhhhhhhhhhhhhhhhhhw
Z=9  hhhhhhhhhhhhhhhhhhhhhhhh
Z=10 whhhhhhhhhhhhhhhhhhhhhhhw
Z=11 hhhhhhhhhhhhhhhhhhhhhhhh
Z=12 whhhhhhhhhhhhhhhhhhhhhhhw
Z=13 hhhhhhhhhhhhhhhhhhhhhhhh
Z=14 whhhhhhhhhhhhhhhhhhhhhhhw
Z=15 hhhhhhhhhhhhhhhhhhhhhhhh
Z=16 wwwwhhhhhhhhhhhhhhhhwwww
Z=17 wwwwhhhhhhhhhhhhhhhhwwww
Z=18 wwwwhhhhhhhhhhhhhhhhwwww
Z=19 wwwwhwhwhwhwhwhwhwhwwwww
     012345678901234567890123  ← X
```

#### Y=12 — Corner Tower Extension (Level 1)

Only the four corner sections continue above the main roof. Everything else is open sky.

```
Z=0  wwww................wwww
Z=1  wwww................wwww
Z=2  wwww................wwww
Z=3  wwww................wwww
Z=4  ........................
Z=5  ........................
Z=6  ........................
Z=7  ........................
Z=8  ........................
Z=9  ........................
Z=10 ........................
Z=11 ........................
Z=12 ........................
Z=13 ........................
Z=14 ........................
Z=15 ........................
Z=16 wwww................wwww
Z=17 wwww................wwww
Z=18 wwww................wwww
Z=19 wwww................wwww
     012345678901234567890123  ← X
```

#### Y=13 — Corner Tower Extension (Level 2)

Same as Y=12. Towers now stand 2 blocks above the main roofline.

_(Grid identical to Y=12)_

#### Y=14 — Corner Tower Tops (Crenellated)

Final layer. Checkerboard crenellations on each tower top — alternating raised and low blocks on all four sides. Build complete.

```
Z=0  whwh................whwh
Z=1  hwhw................hwhw
Z=2  whwh................whwh
Z=3  hwhw................hwhw
Z=4  ........................
Z=5  ........................
Z=6  ........................
Z=7  ........................
Z=8  ........................
Z=9  ........................
Z=10 ........................
Z=11 ........................
Z=12 ........................
Z=13 ........................
Z=14 ........................
Z=15 ........................
Z=16 whwh................whwh
Z=17 hwhw................hwhw
Z=18 whwh................whwh
Z=19 hwhw................hwhw
     012345678901234567890123  ← X
```

### Build Tips

- **Extend your platform first.** You need at least 24×20 before laying block one.
- **Build order:** Always complete one full Y layer before moving to the next. Never skip ahead.
- **Lighting while building:** Drop torches on the interior floor as you go up — prevents mob spawning inside the shell.
- **Doors:** Place both oak doors at Y=1 simultaneously so they form a proper double door.
- **Ladder:** At X=12, Z=2 — place the ladder running Y=1 up to Y=5. Break the floor block at Y=6 so you can step off at the top.
- **Pilasters:** The dark oak logs at the pilaster positions replace wall blocks. Do NOT put both a log and a deepslate brick in the same position.
- **Map room:** Once your exploration is done, fill the Z=19 back wall (X=12–22) with item frames and place your maps in them.
- **Future expansion:** The main roof (Y=11) leaves room to add a third floor if you want — just keep building walls above Y=11 in the main body section and add another roof layer.
- **Deepslate tip:** Mine deepslate in bulk before you start. You will run out mid-build if you don't stockpile.
