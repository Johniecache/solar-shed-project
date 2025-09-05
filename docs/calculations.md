# Calculations
All calculations and assumptions used in the solar shed project

## Assumptions
* Useage (Summer): 2 $$\frac{days}{week}$$ x 4 $$\frac{hours}{day}$$ ≈ 8 $$\frac{hours}{week}$$
* Direct Sunlight (Summar): 5 $$\frac{hours}{day}$$

## Power
### Item Consumption
* 2x 15w lights
* 1x 100w fan
* 2x 100w chargers
* Efficiency of 90% (0.9)

### Total Consumption
$$
(2 * 15w) + (100w) + (2 * 100w) = 330w
$$
$$
\frac{330}{0.9} \approx 375w
$$
$$
375w(4h)(2d) = 3000w
$$

### Battery Capacitance
$$
\frac{3000w}{12v} = 250Ah 
$$

### Solar Panel
* Inefficiency Modifier (Aprox) 140% (1.4)

$$
\frac{3000w}{5d} = 600w/day
$$
$$
\frac{600w}{5h} = 120w
$$
$$
120w * 1.4 = 168w 
$$

### Summary
* Useage Time:
  * Only in summer (mowing, bush trimming, branch removal, etc.)
  * Mostly clear skys with little overcast
* Battery: 
  * LiFePO4 with Deep Cycle and BMS
  * 250Ah Absolute Minimum - 280Ah to 300Ah recommended
  * 12v System
* Solar Panel:
  * 200w Absolute Minimum
