# Power Factor Corrections
**IMPORTANT**: This file is completely hypothetical and unnused in out current project. The idea was to reduce upfront cost while also making the system more efficient as well as for the love of the game. **Use this at your own risk**, if you truely want to make the system more efficient then remove the DeWalt battery charger as well as changing the light bulbs and box fan to DC which will remove the need for the pure sine wave converter as well as any need for pfc.

## Calculations

**Assumptions**:
  * Total used power: 375w (taken from calculations.md)
  * Light bulb pf: 0.8
  * DeWalt Charger pf: 0.7
  * Box Fan pf: 0.6

**Approx Power Factor**

$$
PF = \frac{375w}{(\frac{200w}{0.7}) + (\frac{30w}{0.8}) + (\feac{100w}{0.6})} \approx 0.795957 \rightarrow 0.8
$$

