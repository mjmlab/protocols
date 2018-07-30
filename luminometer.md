# Luminometer Reading

## Instrument: Promega GloMax 20/20 Single-Tube Luminometer

<!-- TOC depthFrom:3 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Instrument operation](#instrument-operation)
	- [Select the desired protocol and set the instrument to read every time the lid closes](#select-the-desired-protocol-and-set-the-instrument-to-read-every-time-the-lid-closes)
	- [Read samples](#read-samples)
- [Set up user protocol: `6 SEC-Std`](#set-up-user-protocol-6-sec-std)

<!-- /TOC -->

### Instrument operation

#### Select the desired protocol and set the instrument to read every time the lid closes

This needs to be set up every time the instrument is powered on

1. Turn on instrument.
1. Select `Run User Protocol`.
1. Select desired protocl; e.g. `6 SEC-Std`.
> The correct program is now set.

1. Select `Show parameters`.
1. Select `OK`.
1. Select `Tools`.
1. Select `Settings`.
1. Select `Lid start is off`.
> This toggles the lid start to on.

#### Read samples

If dust is present in the instrument clean using a compressed air duster.

1. Open lid.
1. Insert sample.
1. Close lid, allow reading to completely finish.
1. For squid, open lid immediately after reading to prevent expulsion.

**Troubleshooting**: If the lid does not read on close, select `Measure Luminescence` manually. Then reset lid start beginning above at the `Show parameters` step (this commonly happens every 60-70 samples). Confirm that the correct protocol is still selected.

Record the reading (RLU) and the vessel (e.g., Drosophila vial or 1.5 ml microfuge tube with adapter).

Note: For luminescence reading of cultures, vortex for a precise time prior to reading so that samples are uniformly oxygenated. The vortex should be placed next to the luminometer and vortex time (e.g., 5 s) should be measured with a timer.

### Set up user protocol: `6 SEC-Std`

This only needs to be conducted once in the lifetime of the instrument (unless memory is reset, etc.).

**Kinetics**: OFF.

**Frequency**: 1/1 sec.

**Integration 1**: 6 sec, **Total number of measurements**: 10
