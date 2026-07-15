# Mixer Comparisons

This directory contains design files for PC boards intended to help compare different kinds of mixers, particularly in the HF to VHF regime. 

## The basics

This board has inputs for RF, local oscillator and and baseband outputs (if available). The local oscillator is assumed to be at 3.3V logic levels and is locally buffered to get a differential drive. Test points are available for internal signals.

## The contestants

The mixers available include the LT5560 and Tayloe mixers constructed using SN74CBT3253DR (similar to the FST3253), SN74LVC1G3157, or 74LVC1G66 analog switch. In all cases it is assumed that the desired output is limited to <100kHz. There is no presumption about the frequency of the RF or LO inputs other than they should be near enough to produce a useful baseband output.
