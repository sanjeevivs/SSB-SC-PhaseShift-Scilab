# Simulation Instructions for SSB-SC Using Xcos

## Tools Required:
- Scilab 6.x
- Xcos Simulation Environment

## Steps:
1. **Open Xcos** from Scilab.
2. **Drag and Drop:**
   - 1 Signal Generator → Message Signal
   - 1 Gain Block → Simulate Hilbert Transform (90° phase shift)
   - 2 Signal Generators → Cosine and Sine carriers (set phases to 0° and 90° respectively)
   - 2 Product Blocks → Multipliers
   - 1 Sum Block → Combines the two paths
   - 1 CSCOPE → Output visualization
3. **Parameter Settings:**
   - Message Signal: Frequency ~100 Hz
   - Carrier Signal: Frequency ~1 kHz, Phases: 0° (cos) and 90° (sin)
4. **Connections:**
   - Message → Product (cosine carrier)
   - Phase-shifted Message → Product (sine carrier)
   - Sum of both → CSCOPE
5. **Run the Simulation.**
6. **Capture output screenshots.**

