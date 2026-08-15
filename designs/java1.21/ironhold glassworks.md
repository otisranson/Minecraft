# The Ironhold Glassworks

Decorative greenhouse — companion build to The Ironhold

**Footprint:** 12 blocks wide (X=0–11) × 10 blocks deep (Z=0–9)  
**Height:** 5 layers (Y=0 to Y=4)  
**Style:** Deepslate bricks · Dark oak logs · Glass panes · Glass blocks  
**Seed:** 2417470717322115627 · Java 1.21

---

## What makes this build work

The Glassworks uses the same deepslate brick base and dark oak log frame as The Ironhold, so the two structures read as a matching pair from a distance. The dark oak log roof beams run east-to-west in three parallel lines, leaving large panes of glass between them — the greenhouse silhouette is recognisable from the outside while still looking deliberate and built, not like a random glass box.

The interior water channel at Z=4 hydrates every farmland row in both directions. All 70 farmland blocks are within Chebyshev distance 4 of the water — no hoe patches will dry out.

---

## Orientation

- **Z=0**  = front face (door/south side)
- **Z=9**  = back face
- **X=0**  = west wall
- **X=11** = east wall
- **Y=0**  = platform surface — start here

Place this structure to the side or rear of The Ironhold, leaving at least 3 blocks of gap between them for pathing and aesthetics. A path of deepslate brick slabs connecting the two doors ties the compound together.

---

## Block Key

| Code | Block |
|------|-------|
| `w` | Deepslate bricks |
| `l` | Dark oak log |
| `g` | Glass pane |
| `G` | Glass block (roof) |
| `d` | Oak door (lower — place here) |
| `D` | Oak door (upper — auto-placed, do not place) |
| `f` | Farmland |
| `W` | Water source block |
| `.` | Air (empty) |

---

## Layers

### Y=0 — Foundation Floor

Lay directly on your platform. Deepslate brick perimeter with dark oak log corners. Interior is all farmland except the central water channel at Z=4, which runs the full interior width (X=1–10).

```
Z=0  lwwwwwwwwwwl
Z=1  wffffffffffw
Z=2  wffffffffffw
Z=3  wffffffffffw
Z=4  wWWWWWWWWWWw
Z=5  wffffffffffw
Z=6  wffffffffffw
Z=7  wffffffffffw
Z=8  wffffffffffw
Z=9  lwwwwwwwwwwl
     012345678901  <- X
```

> **Farmland:** X=1–10 across Z=1–3 and Z=5–8 (70 blocks total).  
> **Water:** X=1–10 at Z=4. Every farmland block is within 4 of this channel — all rows are permanently hydrated.  
> **Note:** Do not put dirt here — place farmland directly, or hoe dirt after laying.

---

### Y=1 — Base Walls

One-block-tall solid deepslate brick wall around the perimeter. Dark oak logs at all four corners. Double oak doors at X=5 and X=6 on the front face (Z=0). Interior is open.

```
Z=0  lwwwwddwwwwl
Z=1  w..........w
Z=2  w..........w
Z=3  w..........w
Z=4  w..........w
Z=5  w..........w
Z=6  w..........w
Z=7  w..........w
Z=8  w..........w
Z=9  lwwwwwwwwwwl
     012345678901  <- X
```

> **Doors:** Place both oak doors at Y=1 simultaneously so they form a proper double door. Upper halves at Y=2 are auto-placed.

---

### Y=2 — Glass Walls (Lower) + Door Upper Halves

Glass panes replace the deepslate brick on every wall face. Dark oak logs remain at all four corners. The `D` markers at X=5 and X=6 are the upper halves of the doors placed at Y=1 — do not place these manually.

```
Z=0  lggggDDggggl
Z=1  g..........g
Z=2  g..........g
Z=3  g..........g
Z=4  g..........g
Z=5  g..........g
Z=6  g..........g
Z=7  g..........g
Z=8  g..........g
Z=9  lggggggggggl
     012345678901  <- X
```

---

### Y=3 — Glass Walls (Upper)

Identical to Y=2 but without the door markers. Two full rows of glass (Y=2 and Y=3) give the greenhouse tall, airy walls. From the outside the dark oak log corners frame each glass panel clearly.

```
Z=0  lggggggggggl
Z=1  g..........g
Z=2  g..........g
Z=3  g..........g
Z=4  g..........g
Z=5  g..........g
Z=6  g..........g
Z=7  g..........g
Z=8  g..........g
Z=9  lggggggggggl
     012345678901  <- X
```

---

### Y=4 — Roof (Log Beams + Glass Blocks)

Three east-to-west dark oak log beams span the full width of the structure at Z=0, Z=4, and Z=9. The beams also run along both long sides (X=0 and X=11, Z=1–8). Glass blocks fill every remaining position, giving a fully glazed roof with visible structural framing.

```
Z=0  llllllllllll   <- front edge beam
Z=1  lGGGGGGGGGGl
Z=2  lGGGGGGGGGGl
Z=3  lGGGGGGGGGGl
Z=4  llllllllllll   <- centre beam
Z=5  lGGGGGGGGGGl
Z=6  lGGGGGGGGGGl
Z=7  lGGGGGGGGGGl
Z=8  lGGGGGGGGGGl
Z=9  llllllllllll   <- back edge beam
     012345678901  <- X
```

> **Glass blocks — not panes — for the roof.** Panes placed flat become invisible or misalign. Use glass blocks for a solid horizontal surface.  
> The centre beam at Z=4 sits directly above the water channel below — a visual callback that makes the structure feel considered.  
> **Optional:** Hang lanterns on chains from the underside of the centre beam (Z=4, X=2/5/8) for interior night lighting without a lit floor.

---

## Total Materials List

| Block | Quantity |
|-------|----------|
| Deepslate bricks | ~70 |
| Dark oak log | ~70 |
| Glass pane | ~75 |
| Glass block | ~70 |
| Farmland | 70 (hoe dirt in place) |
| Water source block | 10 |
| Oak door | 2 |
| Chain (optional) | ~6 |
| Lantern (optional) | ~6 |

> **Dark oak logs:** this build uses roughly the same quantity as The Ironhold. If you haven't sourced a Dark Forest yet, you will need to before starting the roof. The walls (Y=0–3) only need corner logs — 16 total — so you can build the shell now and save the logging expedition for the roof phase.  
> **Glass panes** are crafted from glass blocks (6 blocks → 16 panes). For 75 panes you need roughly 29 glass blocks smelted from sand, in addition to the 70 glass blocks used directly in the roof. Budget around 100 sand total.

---

## Interior Decoration Notes

Once the shell is complete, the interior (Y=1 floor level, X=1–10, Z=1–8) is yours to fill.

- **Crops:** Wheat, carrots, potatoes, and beetroot all grow on farmland. Mix crop types across rows for a proper working-farm look. Bone meal speeds early growth.
- **Flower pots:** Place on the farmland edges (X=1 or X=10, any Z) with ferns, dandelions, or azure bluets for a decorative touch.
- **Composter:** One or two at the back wall (Z=8) turn excess crops into bone meal — keeps the space self-sufficient.
- **Lighting:** The glass roof provides natural daylight for crop growth. To prevent mob spawning after dark, hang lanterns on chains from the roof beam undersides to keep interior light above level 8.

---

## Build Tips

- **Platform first.** Extend your build platform to at least 12×10 before placing any blocks.
- **Build order:** Complete each Y layer fully before moving to the next.
- **Corner logs replace wall blocks.** At every corner, the dark oak log is the block — do not place both a log and a deepslate brick in the same position.
- **Doors:** Stand outside and place both doors at Y=1 together. The double door forms correctly when both halves are in place before you enter.
- **Mob spawning:** Drop a torch on the interior farmland while building above Y=2. Remove and replace with lanterns when the roof is complete.
- **Connecting path:** Deepslate brick slabs between the Ironhold front door and the Glassworks front door make the compound feel intentional. 3–5 blocks of gap between the two structures is enough for visual separation and practical movement.
