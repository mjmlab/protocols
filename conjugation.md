# Conjugation  

**Day 0**  

1. Plate strains for mating on agar, grow overnight.
  - Donor – *E. coli* on selective LB.  Grow 37°C.
  - Helper – *E. coli* CC118 λpir / pEVS104 [MJM534] on LB-Kan50.  Grow 37°C.
  - Recipient - typically *V. fischeri* on LBS.  Grow 25-28°C.  

**Day 1**  

1. Grow overnight liquid cultures of the strains with antibiotics if necessary.

**Day 2**  

1. Combine 100 μl of each *E. coli* culture only in a 1.5-ml microfuge tube (see controls below).
1. Pellet cells by centrifugation (1 min at 8,000 x g).
1. Add 100 μl of each *V. fischeri* culture to the *E. coli* pellet.
1. Pellet cells by centrifugation (1 min at 8,000 x g); resuspend in 10 μl fresh LBS.
1. Spot this onto a fresh, thick LBS plate.
1. Incubate for ~16 h at 25-28°C.

**Day 3**  

1. Scrape the mating mix off the plate and suspend in 750 μl of LBS. In the case of *V. fischeri*, spot should be yellowish.
1. Plate on selective media and incubate at room temperature (or cooler, e.g., 15°C).
  - This cooler temp enriches for Vibrio over the *E. coli* donor.
  - For "frequent" events like introduction of a stable plasmid, plate dilutions and/or streak purify from the spot.
1. Colonies should appear in 1-2 days at room temperature, or 3-4 days at 15°C.  Streak-purify transconjugants.

A generic tri-parental mating includes an *E. coli* strain with pEVS104 as the conjugal helper plasmid, a second *E. coli* strain with an *oriT*-containing plasmid to be mobilized, and a recipient Vibrio. For quadraparental mating (ex. with mini-Tn7) use 200 µl of the Vibrio recipient.  

Controls: Same as conjugation tube but excluding one of the constituent strains (no donor, no recipient, and no helper controls).

Plate freshness: Fresh LBS plates seem to help a lot.  If possible, use them the same day you pour them; just make sure they’re not "sloppy wet." If you want to compare mating efficiencies of different constructs, be careful to use similar plates or multiple spots on the same plate.  

Citation: [Stabb EV, Ruby EG. RP4-based plasmids for conjugation between Escherichia coli and members of the Vibrionaceae. Meth Enzymol (2002) vol. 358 pp. 413-26](http://www.ncbi.nlm.nih.gov/pubmed/12474404)

# Triparental Conjugation into Klebsiella

This is a protocol describing the triparental conjugation of Tn7 transposon and Tn7 transposase plasmids into a deletion strain of KPPR1. The complementation of VK055_1398 into its deletion strain is used as an example.

**Day 0**  

1. Make overnight cultures of each strain:
   - Transposon Plasmid (pAD13, MJM5668): Grown in LB-Kan50-DAP liquid media at 37C, shaking
   - Transposase Plasmid (pJMP1039, MJM4078): Grown in LB-Carb100-DAP liquid media at 37C, shaking
   - Deletion Strain (∆1398, MJM): Grown in LB at 37C, shaking
   - Positive control (Any previously complemented strain made)


**Day 1: Conjugation**  
**Important: Do all steps in the BSC**

1. Add 500 uL of each strain to a tube, mix well with a pipette
   * At this point, make multiple *negative controls* using just the deletion strain, just the transposase plasmid, just the transposon plasmid, etc.
   * Also make a *positive control* by using the previously complemented strain
2. For all samples:
   * centrifuge for 3 min at max speed
   * Resuspend pellet in 10 uL of LB-DAP
   * Plate 10 uL spot onto LB-DAP plate
   * Wait 10 min for spots to dry
   * Parafilm plates and put into 30C incubator
     * If putting in core room, make sure that you put all plates into box for Klebsiella plates

**Day 2: Plate Klebsiella**  
**Important: Do all steps in the BSC**

1. Take spots out of the incubator
2. For each spot, do the following:
   * Pick up spot using sterile cotton swab soaked in 1x PBS
   * Swirl swab well (about 30 sec) in 1 mL of 1x PBS in 2 mL centrifuge tube
   * Dilute to 10^-2 and 10^-4 using 1x PBS
   * Plate onto LB-Kan50 plate *with no DAP*
   * Parafilm plate
3. Put plates into 30C incubator overnight

**Day 3-5: Kick out plasmids**  

1. Streak 4-8 colonies from yesterday onto 2 different plates:
   * LB-Kan50: Shows that Kleb has the Tn7 site inserted
   * LB-Carb100: If candidates grow on this plate, that means that plasmids haven't been kicked out of the Klebsiella. Restreak until candidate doesn't grow on this plate

Usually it takes 1-2 days for the plasmids to be kicked out

2. If candidates aren't growing on the LB-Carb100 plate, make overnight cultures in LB-Kan50 and grow overnight at 37C shaking

**Day 6: PCR Screen**  

* Use AD_103 + 104 as the primers
  * Sequences are in the lab database as well as in Pep Charusanti's paper
* For template DNA, use a 1:100 dilution of overnight culture
* After screen, run Q5 PCR and PCR purify the product
* Send the purified PCR product to Plasmidsuarus for linear amplicon sequencing

