# Flight One E6B Computer
#### Aviation Calculator for Students and Pilots

## Help
Version 1.0.0

### About

Thank you for downloading the Flight One E6B app.

This app is designed to help you preform pre-flight planning and performance calculations quickly and efficiently on the ground.

The functions are organized into groups to help speed up your workflow. You can find more information about each group of functions in the sections below.

### Entering data

In all functions, inputs are highlighted with a box, whereas computed values, or outputs, are not:

![alt text](https://github.com/rajjeshang/E6B/blob/main/InputOutput.PNG?raw=true)

In the example above, the output displays a value 2x the input. Each input has a valid range, depending on the function. For example, in the app, the input above has a valid range of -99 and 99. 

When you enter a value, all connected outputs update in real time. Data is automatically saved, so you can pick up where you left off when you re-launch the app. 

### Rounding

Certain outputs are rounded to the nearest integer where a decimal point is irrelevant, such as a heading. For example, a heading of 135.4° will be displayed as 135°, and 135.5 reads 136°.

### E6B

These are functions you'll find useful in planning your flight. The order of calculations is such that inputs at the top affect outputs below, as well as left to right. However, you can input values in any order you prefer.

#### *Clouds*

Cloud base is determined based on what altitude the spread between Outside Air Temperature (OAT) and Dew Point is at 0.

Freezing point is estimated based on a temperature lapse rate of 1.98°C every 1000ft of altitude.

#### *Altitudes*

Indicated altitude is limited to a range of -2000 feet through 36000 feet. 

#### *Wind*

Wind direction ranges from 1° to 360°. If you enter a value outside this range, it is rewrapped. Examples: 0° is rewrapped to 360°, 361° becomes 1°, and 720° becomes 360°.

#### *Wind Speed*

When wind speed is greater than the True Air Speed (TAS), there is no solution for wind correction. In this case, wind correction is set to 0.

#### *Airspeeds*

You can enter either the Calibrated Air Speed (CAS) or True Air Speed (TAS). One is computed from the other you entered. [Or: When you enter one, the other will be computed based on that speed.]

#### *Wind Components*

Enter the runway number you plan to use. Valid input ranges from 1 through 36.

Wind direction and speed use the inputs from the Wind section above. Crosswind and head/tail wind components are calculated based on zero airspeed.

The L or R in the crosswind output tells you which direction the wind is blowing from. Similarly, the H or T in the head/tail wind component tells you if you’re got a head or tail wind.

#### *Flight Time*

Time needed to fly the distance entered is based on your ground speed.

### Fuel Calculator

Convert between the weight and volume of Avgas and Jet-A, and calculate the endurance given a volume of useable fuel.

Weight and Balance
Like a weight and balance sheet, add the stations you need. For each station, enter the weight and the arm. The final CG and total weight are displayed at the top.

Moments are hidden by default to save space on smaller screens. You can enable them by setting the preferences above.

You can delete individual stations by swiping left.

### Linear Interpolator
This function is designed to help interpolate performance tables and other data found in the Pilot’s Operating Handbook.

Suppose you need to calculate short field takeoff distance, at a pressure altitude of 4580 feet. This is what the POH lists:

| Press Alt	| Ground Roll	| Total distance to clear 50ft obstacle |
|-----------|-------------|---------------------------------------|
| 4000 | 870 | 1490 |
| 5000 | 955 | 1635 |

First, enter the lower-bound values: 4000, 870, and 1490

Then enter the upper-bound values: 5000, 955, and 1653

Finally, enter 4580 in the “Interpolated A” field.

The outputs will show:

| Interpolated A	| Interpolated B	| Interpolated C |
|-----------------|-----------------|----------------|
| 4850 | 919 | 1585 |

Therefore, at a pressure altitude of 4580 feet, your ground roll will be 919 feet, and the total distance required to clear a 50-foot obstacle will be 1585.

It will also show 4580 to be 58% between 4000 and 5000. Note, if you enter a value that is below 0% or above 100%, you are extrapolating. This may not be what you want, and a warning indicator will be displayed next to all interpolated values.

Interpolator inputs have a valid range of -99999 through 99999.


### Conversions
This function provides the following conversions between imperial and metric units. You can enter values on either side:

Feet ↔ Meters
<br>Inches of mercury ↔ Millibars
<br>Nautical miles ↔ Statute miles ↔ Kilometers
<br>Fahrenheit ↔ Celsius ↔ Kelvins
<br>Gallons ↔ Liters
<br>Pounds ↔ Kilograms

### Time Calculator
Two functions are available here: Add or subtract time in the HH:MM:SS format, and convert time between HH:MM:SS and decimal hours, minutes, and seconds.

In the Add Time function, add as many time units as you need. Swipe left to delete individual time units.

In the convert time function, start with any input. The others will update to display the corresponding value.

## Privacy Policy:

Flight One E6B does not collect any data about you or your device. All calculations are saved locally on your device. You can reset all inputs by going to "Help & Preferences" and tapping "Reset all inputs"
