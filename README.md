# Cascode OpAmp

A Cascode Operational Amplifier (Cascode Op-Amp) is an operational amplifier that uses cascode transistor configurations (a common-source/common-emitter transistor stacked with a common-gate/common-base transistor) to achieve very high voltage gain, high output resistance, and improved bandwidth.

A Cascode Op-Amp is an operational amplifier in which one or more amplification stages employ a cascode configuration to increase the amplifier's gain by increasing its output resistance while reducing the Miller effect, thereby improving frequency response and stability

## Tool used

- Cadence Virtuoso
- tsmc Node65

## What is a Cascode?

A cascode is formed by connecting:

Bottom transistor: Common Source (CS) MOSFET

Top transistor: Common Gate (CG) MOSFET

The top transistor shields the bottom transistor from large drain voltage variations.

      VDD
       |
      M2 (Common Gate)
       |
      M1 (Common Source)
       |
      GND

Input → Gate of M1

Output → Drain of M2

## Why use a Cascode in an Op-Amp?

A simple differential amplifier has limited gain because its output resistance is limited.

The cascode configuration:

- Increases output resistance (ro)
- Increases voltage gain
- Reduces Miller capacitance
- Improves bandwidth
- Improves isolation between input and output

## Voltage Gain

For a simple amplifier:

	​


For a cascode amplifier:

​
or approximately

Since the output resistance becomes much larger, the gain increases significantly

## Components used

**Schematic**
- pch_25
- nch_25

## Advantages

Very high DC gain

High output resistance

Better frequency response

Reduced Miller effect

Improved stability

Better isolation between input and output

## Disadvantages

Reduced output voltage swing

Requires higher supply voltage

More transistors

Increased circuit complexity

## Cascode Op-Amp — Definition

A cascode operational amplifier (cascode op-amp) is an op-amp that uses cascode transistor configurations in its internal stages to achieve high output resistance, high voltage gain, and improved performance compared with a conventional op-amp.

**In simple words:**

A cascode op-amp combines an operational amplifier with cascode transistor stages, where one transistor is stacked on top of another to increase the output resistance and therefore the voltage gain

## Why is the cascode used?

The stacked transistors provide:

🔹 Higher voltage gain — due to increased output resistance
🔹 Higher output resistance
🔹 Better current-source behavior
🔹 Improved isolation between input and output
🔹 Better gain accuracy
