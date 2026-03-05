# Experiment 17: Binary Phase Shift Keying (BPSK)

## Objectives
- Generate a BPSK signal.
- Observe 180° phase shifts at digital logic transitions.
- Demodulate using a product detector.
- Restore the digital signal with a comparator.
- Understand BPSK’s relation to DSBSC modulation.

## Materials
- **Trainer:** Emona Telecoms-Trainer 101 + power-pack  
- **Oscilloscope:** Dual-channel 20MHz  
- **Modules:** Master Signals, Sequence Generator, Multiplier, Tuneable LPF, Comparator, Variable DCV  
- **Leads:** Oscilloscope and patch leads  

## Background
BPSK transmits data by inverting the phase of a carrier signal (180° shift) for logic changes. It is similar to DSBSC modulation, as the carrier amplitude stays constant and only phase changes. BPSK is more noise-resistant than ASK or FSK.

## Procedure
1. **Signal Generation**
   - Connect Sequence Generator output and 100kHz sine carrier to a Multiplier.
   - Observe BPSK signal on oscilloscope; note phase reversals at logic transitions.

2. **Demodulation**
   - Use a second Multiplier + Tuneable LPF as a product detector.
   - Recover the baseband digital signal.

3. **Signal Restoration**
   - Feed LPF output to Comparator with Variable DCV reference.
   - Adjust threshold to match recovered digital signal to original.

## Observations
- BPSK shows 180° phase shifts at logic transitions.
- Product detector + LPF recovers baseband but edges are slightly rounded.
- Comparator restores sharp transitions for clean digital output.

## Q&A
- **Logic transitions:** 180° phase shift in BPSK signal.  
- **DSBSC feature:** Envelope follows data and crosses zero at polarity changes.  
- **Imperfection in recovered signal:** LPF rounds edges.  
- **Signal cleanup:** Comparator or Schmitt trigger.  
- **DC voltage effect:** Changes comparator threshold, altering pulse width.

## Summary
BPSK encodes data as phase reversals of a constant-amplitude carrier. Demodulation using a product detector recovers the signal, and a comparator restores it to digital form. The experiment illustrates BPSK modulation, demodulation, and robustness in digital communication.
