# Mega Ether-Growl – Memphis Robot Alive Mega Structure

**Consolidated self-contained Cmajor processor for Amorph Instrument**

Heterodyne Etherphone emulation  
+ phase-locked Iron Sub-Dough octave divider  
+ Duracell CIA battery fail simulation  
+ glitch artifacts  
+ meet-map repeating feedback loops

This mega-patch fuses the full haunt chain into **one compilable unit**:  
ethereal theremin-like glissando whistle + locked low-end Memphis growl (Nas Escobar / Spanish Fly trunk thump style) + voltage sag / corrosion hiss + random blackout dice rolls + damped darkening repeat cycles.

**Robot council approved. Alive in the blacks of Memphis.**  
Too long? Wear it. 👻📡🤖🔊

## Core Features

- Classic heterodyning (~450 kHz fixed reference + variable pitch deviation) → ghostly Ether whistle  
- Analog-style octave-down subharmonic synthesis (zero-cross tracking both edges + tanh distortion) → gritty 808-style punch  
- Abyssal pitch mapping (power 5.2 law) → low "dough" dominates antenna reach  
- Iron hysteresis + asymmetric tube warmth → heavy velvety saturation  
- Mechanical wow/flutter + tape compression bark wobble  
- Duracell fail simulation: voltage drain, corrosion hiss buildup, random dice-triggered blackout  
- Internal meet-map repeat delay → short damped feedback loops for cycling dread (no external routing needed)  
- Glitch micro-offsets on variable oscillator → Tightness-like artifacts during power sag  
- Soft-clip final output stage → speaker-safe

## Requirements

- [Amorph Instrument](https://artistsindsp.com/) (beta host for prompt-to-Cmajor DSP)  
- Cmajor compiler (included in Amorph or available via [cmajor.dev](https://cmajor.dev))  
- Any DAW that supports MIDI input (Ableton Live, Reaper, Logic Pro, etc.)

## Quick Start / Installation

1. Copy the full code from the section below (or from `MegaEtherGrowl.cmajor` if separate)  
2. In Amorph Instrument:  
   - New preset / instrument  
   - Paste code → **Compile**  
   - Load on MIDI track (hold notes, drone, or automate parameters)  
3. Recommended automation targets for live performance:  
   - **Pitch Reach** → mod wheel / envelope → sweeping glissandi  
   - **Sub-Dough Growl** → build weight  
   - **Meet Map Repeat** → increase cycling density  
   - **Duracell Drain (CIA)** + **CIA Dice Fail Thresh** → introduce random terror/failure

**Troubleshooting compile issues** (rare):  
- Ensure float literals end in `f`  
- Check sample-rate assumptions (~44.1–48 kHz delay tuning)  
- Verify no missing semicolons or brace mismatches

## Exposed Parameters

| Parameter                  | Range     | Default | Description                                      |
|----------------------------|-----------|---------|--------------------------------------------------|
| Pitch Reach                | 0–127     | 64      | Antenna distance → abyssal low-end mapping       |
| Volume Proximity           | 0–1       | 0.5     | Inverse-square proximity-based swell             |
| Sub-Dough Growl            | 0–1       | 0.6     | Sub-octave level & blend                         |
| Iron Mass / Warmth         | 0–1       | 0.8     | Hysteresis drive + tube saturation               |
| Sub Dist Grit              | 0–1       | 0.4     | tanh overdrive on sub square wave                |
| Tape Bark / Wobble         | 0–1       | 0.5     | Wow/flutter + compression artifacts              |
| Meet Map Repeat            | 0–1       | 0.4     | Damped feedback repeat amount                    |
| Duracell Drain (CIA)       | 0–1       | 0.08    | Voltage sag / drain speed                        |
| CIA Dice Fail Thresh       | 0–1       | 0.06    | Random blackout probability                      |

## Typical Use Cases

- **Haunt Drone**  
  Hold high MIDI note → slow downward **Pitch Reach** sweep → ramp **Sub-Dough Growl** + **Meet Map Repeat** → infinite darkening abyss  

- **Memphis Robot Alive**  
  Max **Sub Dist Grit** + **Iron Mass** → automate high **Duracell Drain** → growl sags, hiss builds, sudden council blackout  

- **Glitch Ladder Proxy**  
  High **Meet Map Repeat** + low voltage state → micro-glitches darken each repeat progressively

## Full Processor Code – MegaEtherGrowl.cmajor

```cmajor
// ════════════════════════════════════════════════════════════════════════
// PASTE YOUR COMPLETE CMAJOR PROCESSOR CODE HERE
//
// This should be the full working processor definition including:
// - input / output streams & events
// - node graph definitions
// - state variables
// - processing logic
// - all DSP nodes (oscillators, filters, delays, saturators, etc.)
//
// Example skeleton (REPLACE ENTIRELY with your actual code):

processor MegaEtherGrowl
{
    input event noteOn;
    input event noteOff;
    input event pitchBend;
    input event controller;

    input stream<float> audioIn;   // optional if you want to process incoming audio
    output stream<float> audioOut;

    // === Your nodes, parameters, graphs, logic here ===

    // node fixedOsc        = Oscillator(...);
    // node variableOsc     = Oscillator(...);
    // node heterodyne      = Multiply(...);
    // node subTracker      = ZeroCrossTracker(...);
    // node voltageSag      = ...;
    // node repeatDelay     = FeedbackDelay(...);
    // etc.

    // Your main process function / graph connections
}

// If your code is very long (>400–500 lines), consider keeping it in a separate .cmajor file
// and linking to it instead of inlining everything here.
// ════════════════════════════════════════════════════════════════════════
