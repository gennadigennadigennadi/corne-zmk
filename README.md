# Corne ZMK Config

ZMK firmware config for a **Corne-34** split keyboard (`nice_nano_v2` + `nice_view` displays).
Default layout is **Colemak-DHM** with home-row mods and ZMK Studio support.

## Key matrix

```
╭─────────────────────╮ ╭─────────────────────╮
│  0   1   2   3   4  │ │   5   6   7   8   9 │
│ 10  11  12  13  14  │ │  15  16  17  18  19 │
│ 20  21  22  23  24  │ │  25  26  27  28  29 │
╰──────╮ 30  31  32   │ │  33  34  35 ╭───────╯
       ╰──────────────╯ ╰─────────────╯
```

## Layers

### Layer 0 — `colemak` (default)

Home-row cells show the tap key (top) and the held modifier (bottom).

```
╭─────┬─────┬─────┬─────┬─────╮   ╭─────┬─────┬─────┬─────┬─────╮
│  Q  │  W  │  F  │  P  │  B  │   │  J  │  L  │  U  │  Y  │  '  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│  A  │  R  │  S  │  T  │  G  │   │  M  │  N  │  E  │  I  │  O  │
│ SFT │ CTL │ ALT │ GUI │     │   │     │ GUI │ ALT │ CTL │ SFT │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│  Z  │  X  │  C  │  D  │  V  │   │  K  │  H  │  ,  │  .  │  /  │
╰─────┴─────┴─────┴─────┴─────╯   ╰─────┴─────┴─────┴─────┴─────╯
            ╭─────┬─────┬─────╮   ╭─────┬─────┬─────╮
            │ ESC │ SPC │ TAB │   │ RET │ RSE │ BSP │
            │     │ L1  │     │   │     │ L2  │     │
            ╰─────┴─────┴─────╯   ╰─────┴─────┴─────╯
```

### Layer 1 — `left` (EXT — symbols / nav)

```
╭─────┬─────┬─────┬─────┬─────╮   ╭─────┬─────┬─────┬─────┬─────╮
│  !  │  @  │  #  │  $  │  %  │   │  ^  │  &  │  *  │  ~  │  `  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ ESC │ CTL │ ALT │ GUI │ SFT │   │ LFT │ DWN │ UP  │ RGT │ BSP │
│     │ sk  │ sk  │ sk  │     │   │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ C-Z │ C-X │ C-C │     │ C-V │   │ ::  │ ->  │ =>  │     │     │
╰─────┴─────┴─────┴─────┴─────╯   ╰─────┴─────┴─────┴─────┴─────╯
            ╭─────┬─────┬─────╮   ╭─────┬─────┬─────╮
            │ trn │ trn │     │   │     │ L3  │     │
            ╰─────┴─────┴─────╯   ╰─────┴─────┴─────╯
```

Legend: `C-x` = Ctrl+x, `sk` = sticky modifier, `::` `->` `=>` = macros, `trn` = transparent, `LFT/DWN/UP/RGT` = arrow keys.

### Layer 2 — `right` (sym — symbols / numbers)

```
╭─────┬─────┬─────┬─────┬─────╮   ╭─────┬─────┬─────┬─────┬─────╮
│  !  │  @  │  #  │  :  │  ;  │   │  =  │  7  │  8  │  9  │  +  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│  \  │  |  │  {  │  (  │  [  │   │  *  │  4  │  5  │  6  │  -  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│  -  │  _  │  }  │  )  │  ]  │   │  0  │  1  │  2  │  3  │  /  │
╰─────┴─────┴─────┴─────┴─────╯   ╰─────┴─────┴─────┴─────┴─────╯
          ╭─────┬─────┬─────╮   ╭─────┬─────┬─────╮
          │     │ L3  │     │   │ RET │ trn │     │
          ╰─────┴─────┴─────╯   ╰─────┴─────┴─────╯
```

### Layer 3 — `both` (Sym2 — F-keys / media / Bluetooth)

```
╭─────┬─────┬─────┬─────┬─────╮   ╭─────┬─────┬─────┬─────┬─────╮
│ BT0 │ BT1 │ BT2 │ BT3 │ BT4 │   │ trn │ F7  │ F8  │ F9  │  `  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ CLR │ PRV │ PLY │ RWD │ FWD │   │ trn │ F4  │ F5  │ F6  │  ~  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ BR- │ BR+ │ MUT │ VL- │ VL+ │   │ trn │ F1  │ F2  │ F3  │  ?  │
╰─────┴─────┴─────┴─────┴─────╯   ╰─────┴─────┴─────┴─────┴─────╯
            ╭─────┬─────┬─────╮   ╭─────┬─────┬─────╮
            │     │     │ trn │   │     │ trn │ trn │
            ╰─────┴─────┴─────╯   ╰─────┴─────┴─────╯
```

Legend: `BTn` = Bluetooth profile select, `CLR` = clear pairing, `PRV/PLY/RWD/FWD` = media prev/play/rewind/next, `BR-/BR+` = brightness, `MUT/VL-/VL+` = mute/volume, `trn` = transparent (falls through to lower layer).

## Home-row mods

Positional hold-tap (`hml` / `hmr`) on the home row. Tap for the letter, hold for the modifier.

| Finger | Left (`A R S T`) | Right (`N E I O`) |
|--------|------------------|-------------------|
| Pinky  | A → Shift        | O → Shift         |
| Ring   | R → Ctrl         | I → Ctrl          |
| Middle | S → Alt          | E → Alt           |
| Index  | T → Gui          | N → Gui           |

Center index keys (`G`, `M`) are plain — no mod.

**Behavior config:** `balanced` flavor, `tapping-term-ms 200`, `quick-tap-ms 150`, `require-prior-idle-ms 100`, `hold-trigger-on-release`. Positional triggers restrict `hml` holds to right-hand + thumb keys and `hmr` holds to left-hand + thumb keys, reducing same-hand misfires.

## Macros

| Macro | Output |
|-------|--------|
| `small_arrow` | `->` |
| `big_arrow` | `=>` |
| `double_colon` | `::` |

## Building & flashing

Firmware builds on every push/PR via GitHub Actions
(`.github/workflows/build.yml` → `zmkfirmware/zmk` reusable workflow).
Download the `.uf2` artifacts for each half from the workflow run, then flash
by double-tapping reset and copying the file to the mounted drive.

### ZMK Studio

The left half exposes a USB serial port (`studio-rpc-usb-uart` snippet) for
live keymap editing via [ZMK Studio](https://zmk.dev/docs/features/studio).

### Local build

```bash
west config manifest.path config
west update
west build -s zmk/app -d build/corne_left  -b nice_nano_v2 -- -DZMK_CONFIG=config
west build -s zmk/app -d build/corne_right -b nice_nano_v2 -- -DZMK_CONFIG=config
```

## Repo layout

| Path | Purpose |
|------|---------|
| `config/corne.keymap` | Keymap, macros, hold-tap behaviors |
| `config/corne.conf` | Kconfig (debounce, BT power, ZMK Studio, idle) |
| `config/corne.json` | Physical layout for the ZMK Visualizer |
| `config/west.yml` | ZMK dependency manifest |
| `build.yaml` | CI board/shield matrix |

