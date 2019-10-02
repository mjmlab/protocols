# Luminescence assay

This protocol overviews how to perform a culture-based assay to assess luminescence quorum sensing in *vibrio fischeri*  
Please note that the protocol takes 8 hours on one day and requires you to be present once an hour to take readings.

## Supplies

Media: SWTO
SWTO is a variant of seawater trytone (SWT) media with the addition of extra NaCl to be a closer osmolarity to seawater are cited in [Bose & Stabb et al (2007) Mol Micro](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1365-2958.2007.05809.x).

|           Amount | Reagent                |
|-----------------:|:-----------------------|
|              5 g | Bacto-Tryptone         |
|              3 g | Yeast Extract          |
|             6 ml | 50% Glycerol           |
|           700 ml | Instant Ocean [1]      |
|           8.76 g | NaCl (150 mM)          |
| to 1000 ml total | with dI H<sub>2</sub>O |

## Protocol

**Day 0**
Make overnight cultures of desired strains in 3ml of LBS.

**Day 1**
Subculture the overnight 1/1000 into 3ml SWTO in a culture tube and culture with aeration at 25C. Duplicate or triplicate tubes can be made for technical replicates for each strain being tested  
Every hour, do the following to take measurements:
1. Remove tube from incubator and read OD600 of entire tube in the WPA Biowave CO8000 cell density meter.
1. Remove 100 ul from the culture tube into a 1.7 ml  microtube.
1. Place culture tubes back on the incubator
1. Vortex each microtube for 10 seconds and immediately read the luminescence. Information on using the luminometer can be found [here](luminometer.md). Make sure to fill a tube with 100 ul SWTO to use to get a blank reading.
1. Note: If the OD reading was above 2.00 (indicated by a flashing reading of 2.00 on the meter), remove the 100 ul from the microtube to a cuvette and dilute with 400ul of SWTO. Multiply the reading by 5 to get the OD.

## Analysis
The raw luminescence reading is the relative luminescence (RLU). To calculate the specific luminescence (SLU) which is normalized to cell number, divide the RLU by OD. To graph the data, plot the SLU on the y-axis on a log scale with the OD on the x-axis. Error bars can be added.

## Alternative approaches and notes
[Bose & Stabb et al (2007) Mol Micro](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1365-2958.2007.05809.x) and other papers from the Stabb lab describe using higher volume cultures for the assay (both 25 ml and 50 ml). If desired, 25 ml cultures in 125 ml flasks works well in our small shaking incubators. If this higher volume is used, remove 500 ul from the flask into a microtube every hour. Read the luminescence and then transfer to a cuvette to read OD. Dilute 1:1 in SWTO if OD reading is above 2.00.

One experiment done by Denise indicated that for luminescence, the 500 ul amount would give a higher reading than the 100 ul amount. However, readings were still within the same log and the same overall results were gained. If nothing restricts you to preferring a smaller amount of media, this approach may be slightly more sensitive though more data is needed to confirm this. Other experiments performed by Denise indicated that SWTO over SWT yields a greater increase in luminescence and that a 1/1000 dilution over a 1/100 dilution leads to a more drastic curve during the growth. Finally, using the plate reader to read luminescence was not as effective.
