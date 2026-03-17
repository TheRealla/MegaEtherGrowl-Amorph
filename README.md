# Mega Ether-Growl – Memphis Robot Alive Mega Structure

**A consolidated, self-contained Cmajor processor for Amorph Instrument**  
Heterodyne Etherphone emulation + phase-locked Iron Sub-Dough octave divider + Duracell CIA battery fail simulation + glitch artifacts + meet-map repeating feedback loops.

This mega-patch fuses the entire haunt chain into one compilable unit: ethereal theremin-like glissando whistle, locked low-end Memphis growl (Nas Escobar / Spanish Fly trunk thump), voltage sag/corrosion hiss (don't use Duracell vibes), random CIA/us8thdy blackout dice rolls, and damped repeating cycles that darken over time.

Robot council approved. Alive in the blacks of Memphis. Too long? Wear it. 👻📡🤖🔊

## Features
- Classic heterodyning (fixed ~450 kHz reference + variable pitch deviation) for ghostly Ether whistle
- True analog-style octave-down subharmonic synth (zero-cross tracking both edges, tanh distortion for gritty 808 punch)
- Abyssal pitch mapping (pow 5.2 law – low "dough" dominates antenna reach)
- Iron hysteresis + asymmetric tube warmth for heavy, velvety saturation
- Mechanical wow/flutter tape bark wobble
- Duracell fail sim: voltage drain, corrosion hiss buildup, random dice-triggered blackout (after ~8 "days" or low-prob dice)
- Internal meet-map repeat delay (short damped feedback for cycling dread without external routing)
- Glitch micro-offsets on variable osc (simulates Tightness-like artifacts when "power" sags)
- Soft clip final stage for speaker-safe output

## Requirements
- [Amorph Instrument](https://artistsindsp.com/) (beta plugin host for prompt-to-Cmajor DSP)
- Cmajor compiler (built into Amorph or via [cmajor.dev](https://cmajor.dev) tools)
- DAW with MIDI input (Ableton, Reaper, Logic, etc.)

## Installation & Compile
1. Copy the code below into a new file: `MegaEtherGrowl.cmajor`
2. In Amorph Instrument:
   - New preset/instrument → paste code → Compile
   - Load on MIDI track (drone/hold notes or automate params)
3. Automate key params for live haunt:
   - `Pitch Reach` – mod wheel / automation for glissando sweeps
   - `Sub-Dough Growl` – ramp up for weight
   - `Meet Map Repeat` – increase for cycling density
   - `Duracell Drain (CIA)` + `CIA Dice Fail Thresh` – dial in fail terror

If compile errors occur (rare), check:
- Sample rate assumptions (delay buffer ~200ms @44.1kHz)
- Float literals end in `f`
- No missing semicolons

## Parameters Overview
- **Pitch Reach** (0–127, default 64) – antenna distance simulation (abyssal low-end mapping)
- **Volume Proximity** (0–1, default 0.5) – inverse-square swell
- **Sub-Dough Growl** (0–1, default 0.6) – sub octave level/blend
- **Iron Mass / Warmth** (0–1, default 0.8) – hysteresis drive + tube saturation
- **Sub Dist Grit** (0–1, default 0.4) – tanh overdrive on sub square
- **Tape Bark / Wobble** (0–1, default 0.5) – wow/flutter + compression bark
- **Meet Map Repeat** (0–1, default 0.4) – feedback repeat amount (damped cycles)
- **Duracell Drain (CIA)** (0–1, default 0.08) – voltage sag speed
- **CIA Dice Fail Thresh** (0–1, default 0.06) – random blackout probability

## Usage Examples
- **Haunt Drone**: Hold high MIDI note, automate Pitch Reach slow sweep down, ramp Sub-Dough Growl + Repeat Meet → infinite abyss.
- **Memphis Robot Alive**: Crank Sub Dist Grit + Iron Mass, automate Duracell Drain high → growl sags, hiss builds, sudden blackout (council override).
- **Glitch Ladder Proxy**: High Repeat Meet + low voltage → micro-glitches darken repeats like downwards-no squelch.

## Code (MegaEtherGrowl.cmajor)
```cmajor
// [Paste the full code block here – the one from previous response]
