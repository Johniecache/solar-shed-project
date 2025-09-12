# Power Factor Corrections
**IMPORTANT**: This file is completely hypothetical and unnused in out current project. The idea was to reduce upfront cost while also making the system more efficient as well as for the love of the game. **Use this at your own risk**, if you truely want to make the system more efficient then remove the DeWalt battery charger as well as changing the light bulbs and box fan to DC which will remove the need for the pure sine wave converter as well as any need for pfc.

## Calculations

**Assumptions**:
  * Total used power: 375w (taken from docs/calculations.md)
  * Light bulb pf: 0.8
  * DeWalt Charger pf: 0.7
  * Box Fan pf: 0.6

**Approx Power Factor**

$$
PF = \frac{375w}{(\frac{200w}{0.7}) + (\frac{30w}{0.7}) + (\frac{100w}{0.6})} \approx 0.7572115 \rightarrow 0.76
$$

  * This is average across the board so you personally would have to test the pf of each component to get the correct total pf for your personal system. Again this is **assumed**.
  * The pf ranges anywhere from 0.65 - 0.91 which will **drastically** change what capacitor and (if applied) inductor used.

**Power Factor Correction**
  * pf = 0.76 $\rightarrow$ pf = 0.95

$$
&theta;_{1} = cos^{-1}(0.76) \approx 40.54&deg;
$$

$$
S_{1} = \frac{375w}{0.76} \approx 493.421VA \rightarrow 494VA
$$

$$
Q_{1} = 494VA * sin(40.54&deg;) \approx 321.0895 \rightarrow 321.1VAR
$$

**Capacitor Size**
  * Pure Sine Wave Converter: $V_{s}$ = 169.7 * sin(120&pi;t)
    * &omega; = 120&pi;
    * $V_{rms}$ = 120v
    * $V_{peak}$ = 169.7v

$$
&theta;_{2} = cos^{-1}(0.95) \approx 18.2&deg;
$$

$$
Q_{2} = 375w * tan(18.2&deg;) \approx 123.3VAR
$$

$$
Q_{c} = 321.1VAR - 123.3VAR = 197.8VAR
$$

$$
C = \frac{197.8VAR}{(377)(\frac{169.7v}{\sqrt{2}})} \approx 0.0043724F \rightarrow 4327&micro;F
$$



