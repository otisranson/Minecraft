# The Creeper Monument — Blueprint

**Type:** Carved hillside monument + hollow interior complex  
**Face:** 32 blocks wide × 32 blocks tall (8×8 pixel art, 4 blocks per pixel)  
**Face footprint:** X=-76 to X=-45 · Y=70 to Y=101 · Z=-38 (surface)  
**Interior hollow:** 28W × 16H × 24D, behind the face going north  
**Orientation:** South-facing — the monument faces The Ironhold directly  
**Seed:** 2417470717322115627 · Java 1.21 · Hill peak X≈-68, Y=115, Z≈-87

---

## What makes this build different

- **Colossal scale** — a 32×32 creeper face carved into the south slope of the hill, visible from The Ironhold across the valley
- **The hill is the structure** — the face is a facade; the hollow skull behind it houses the ore processing operation and rail terminus
- **Pixel-accurate** — 8×8 pixel art scaled to 4 blocks per pixel, matching the classic creeper face exactly
- **Two entrance arches** at the base (col 3 and col 4) — you walk into the monument through the creeper's own face
- **Rail terminus inside** — the elevated rail from The Ironhold extends north and terminates in the skull cavity
- **Hill peak preserved** — Y=115 peak stays untouched; 14 blocks of natural hill crown the monument

> **Warning:** This build requires ~10,000 blocks of excavation for the hollow interior. Phase the work — carve in 4-block-deep slices going north. Do not attempt to hollow the skull in one session.

---

## Orientation

The face sits flush on the south slope at Z=-38, facing south (toward positive Z, toward The Ironhold at Z≈-1).

```
                NORTH
      Z=-62 ─────────────── interior back wall
           [hollow skull cavity — 24 blocks deep]
      Z=-39 ─────────────── interior front wall
      Z=-38 ████ FACE ████  monument south surface

                SOUTH → The Ironhold (Z≈-1)
```

- **West edge of face:** X=-76
- **East edge of face:** X=-45
- **Face bottom:** Y=70
- **Face top:** Y=101
- **Face surface:** Z=-38 (all face blocks placed at this Z)
- **Interior:** Z=-39 to Z=-62, same XY as face minus 2-block border

---

## Block Key

| Code | Block |
|------|-------|
| `M` | Moss block (creeper skin — green) |
| `B` | Black concrete (eyes and mouth) |
| `f` | Stone bricks (border frame) |
| `w` | Deepslate bricks (interior walls) |
| `s` | Smooth stone (interior floor / ceiling) |
| `R` | Rail |
| `[A]` | Air — entrance arch openings |
| `.` | Air (hollow interior) |

---

## The Face — Pixel Map

8×8 pixel grid. Each pixel = 4×4 blocks. Read top to bottom, west to east.

```
         WEST ←────────────────────── EAST
          Col: 0    1    2    3    4    5    6    7

Row 0:        M    M    M    M    M    M    M    M    Y=98–101  (top)
Row 1:        M    B    B    M    M    B    B    M    Y=94–97   (eyes)
Row 2:        M    B    B    M    M    B    B    M    Y=90–93   (eyes)
Row 3:        M    M    M    B    B    M    M    M    Y=86–89   (nose bridge)
Row 4:        M    M    B    B    B    B    M    M    Y=82–85   (mouth top)
Row 5:        M    M    B    M    M    B    M    M    Y=78–81   (mouth mid)
Row 6:        M    M    B    B    B    B    M    M    Y=74–77   (mouth bottom)
Row 7:        M    M    M   [A]  [A]   M    M    M    Y=70–73   (base / arches)
```

### Column → X coordinate

| Pixel column | X range |
|---|---|
| Col 0 | X=-76 to X=-73 |
| Col 1 | X=-72 to X=-69 |
| Col 2 | X=-68 to X=-65 |
| Col 3 | X=-64 to X=-61 |
| Col 4 | X=-60 to X=-57 |
| Col 5 | X=-56 to X=-53 |
| Col 6 | X=-52 to X=-49 |
| Col 7 | X=-48 to X=-45 |

---

## The Face — Full 32-Block Grid

Every block placed at Z=-38. Left = X=-76 (west), right = X=-45 (east). Each character = one block.

```
       X=-76                              X=-45
       |                                     |
Y=101: MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
Y=100: MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
Y=99:  MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
Y=98:  MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM

Y=97:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM  ← eyes
Y=96:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM
Y=95:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM
Y=94:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM

Y=93:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM  ← eyes
Y=92:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM
Y=91:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM
Y=90:  MMMMBBBBBBBBMMMMMMMMBBBBBBBBMMMM

Y=89:  MMMMMMMMMMMMBBBBBBBBMMMMMMMMMMMM  ← nose bridge
Y=88:  MMMMMMMMMMMMBBBBBBBBMMMMMMMMMMMM
Y=87:  MMMMMMMMMMMMBBBBBBBBMMMMMMMMMMMM
Y=86:  MMMMMMMMMMMMBBBBBBBBMMMMMMMMMMMM

Y=85:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM  ← mouth top
Y=84:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM
Y=83:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM
Y=82:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM

Y=81:  MMMMMMMMBBBBMMMMMMMMBBBBMMMMMMMM  ← mouth mid (sides only)
Y=80:  MMMMMMMMBBBBMMMMMMMMBBBBMMMMMMMM
Y=79:  MMMMMMMMBBBBMMMMMMMMBBBBMMMMMMMM
Y=78:  MMMMMMMMBBBBMMMMMMMMBBBBMMMMMMMM

Y=77:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM  ← mouth bottom
Y=76:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM
Y=75:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM
Y=74:  MMMMMMMMBBBBBBBBBBBBBBBBMMMMMMMM

Y=73:  MMMMMMMMMMMMAAAAAAAAMMMMMMMMMMMM  ← base (. = arch openings)
Y=72:  MMMMMMMMMMMMAAAAAAAAMMMMMMMMMMMM
Y=71:  MMMMMMMMMMMMAAAAAAAAMMMMMMMMMMMM
Y=70:  MMMMMMMMMMMMAAAAAAAAMMMMMMMMMMMM
```

> Arch openings span X=-64 to X=-57 (cols 3 and 4 combined, 8 blocks wide), Y=70–73. Frame each side with stone bricks.

---

## The Border Frame

A 2-block-wide stone brick border surrounds the face at Z=-38.

- **Border spans:** X=-78 to X=-43, Y=68 to Y=103
- **Inner opening:** X=-76 to X=-45, Y=70 to Y=101 (the face itself)
- Trim the hillside back to Z=-38 across the entire 36×36 border area before placing any face blocks

---

## The Entrance Arches

Two arches at the base of the face provide entry to the hollow interior.

```
Arch 1: X=-64 to X=-61  (col 3)  Y=70–73  Z=-38  → air
Arch 2: X=-60 to X=-57  (col 4)  Y=70–73  Z=-38  → air
```

Combined width: 8 blocks. Height: 4 blocks. Frame each arch with stone bricks on three sides (top and both uprights). The arches connect directly to the interior hollow.

Carve a flat approach path from the south slope (Z=-27 toward Z=-38) at Y=70. A staircase or carved ledge up the hillside serves as the approach.

---

## The Interior Hollow — Skull Cavity

The hollow skull runs 24 blocks north from the face.

| Dimension | Value |
|---|---|
| Width | 28 blocks (X=-74 to X=-47) |
| Height | 16 blocks clear (Y=70 to Y=85) |
| Depth | 24 blocks (Z=-39 to Z=-62) |
| Walls (N/E/W) | Deepslate bricks, 2 blocks thick |
| Floor | Smooth stone at Y=70 |
| Ceiling | Smooth stone at Y=86 |

### Interior layout (top-down, Y=70 floor)

```
         Z=-39 (south — face wall)              Z=-62 (north)
         |                                            |
X=-74:   ww [arch] ................................ [arch] ww
              |                                       |
              | RRRRRRRRRRRRRRRRRRRR  ← rail terminus |
              |                                       |
              | [furnace bank — west side]            |
              |                                       |
              | [chest storage — north + east walls]  |
              |                                       |
X=-47:   ww [arch] ................................ [arch] ww
```

### Rail terminus

The minecart rail enters from the south through a tunnel at Y=68 (2 blocks below interior floor level), beneath the face. At Z=-42 inside the hollow the rail ramps up to Y=70. Powered rails at both ends for acceleration and deceleration. Terminate with a deepslate brick buffer wall at the north end.

### Storage and processing

- **West side** (X=-74 to X=-63): furnace bank with hoppers — smelt ore directly at the monument
- **North wall** (Z=-60 to Z=-62): double-chest rows for bulk output storage
- **East side** (X=-55 to X=-47): sorted output chest bank + crafting table

---

## Build Order

| Phase | Task |
|---|---|
| 1 | Terrain prep — flatten south slope to Z=-38 across the 36×36 border area |
| 2 | Border frame — place 2-block stone brick border first as your reference boundary |
| 3 | Face blocks — row by row, bottom to top (Y=70 to Y=101). One Y-layer at a time |
| 4 | Arch openings — clear Y=70–73 at cols 3–4; add stone brick arch frames |
| 5 | Hollow excavation — carve Z=-39 to Z=-62 in 4-block-deep slices going north |
| 6 | Interior lining — deepslate brick walls, smooth stone floor and ceiling |
| 7 | Rail tunnel — dig entry tunnel from south at Y=68, connect to existing rail |
| 8 | Interior fitout — furnaces, chests, rail terminus, lighting |
| 9 | Approach stair — carve or build path from valley floor up to Y=70 at Z=-38 |

---

## Materials List

| Block | Quantity | Notes |
|---|---|---|
| Moss block | ~580 | Creeper skin — face M pixels |
| Black concrete | ~320 | Eyes and mouth — face B pixels |
| Stone bricks | ~350 | Border frame around face |
| Deepslate bricks | ~800 | Interior walls and tunnel lining |
| Smooth stone | ~700 | Interior floor and ceiling |
| Rail | ~48 | Interior terminus track |
| Powered rail | ~12 | Acceleration at terminus ends |
| Redstone torch | ~6 | Power for powered rails |
| Torch | ~80 | Interior lighting (mob prevention) |

**Moss blocks:** craft from cobblestone + vine, or source from lush caves. In quantity, lush caves are fastest.  
**Black concrete:** craft black concrete powder (sand + gravel + black dye from ink sacs), wet with a water bucket. Squid farms near the river for ink sacs.  
**Excavation payback:** the 28×16×24 hollow yields thousands of stone, gravel, and ore. Much of your smooth stone and deepslate brick supply comes from mining the hill itself.

---

## Build Tips

- **Scaffold at X=-76.** Build a reference column at the west edge first, then work east. The pixel map row labels give you Y checkpoints as you climb.
- **Temporary markers.** Place dirt at the corner of each pixel square before filling — verify the grid, then replace with final blocks.
- **Light as you go.** The hollow gets dark fast during excavation. Keep torches on interior walls as you carve north.
- **Sightline check.** Stand at The Ironhold entrance and look north — the full face should be visible. If the valley slope blocks the lower portion, clear some terrain for sightlines.
- **Iron bars in the mouth (optional).** At Y=78–81, cols 3–4 (X=-64 to X=-57) are moss on the exterior. Swap to iron bars or glass panes so interior torch light bleeds through the mouth at night.
- **Leave the peak.** Do not excavate above Y=101. The 14 blocks of natural hill above the face are part of the design.
