# Gene Complementation in *Klebsiella Pneumoniae*

This protocol describes complementation of a gene back into Klebsiella using Tn7.

## Insert gene of interest into donor strain's vector backbone using Gibson Assembly

Insert DNA cassette containing the gene of interest from KPPR1(MJM2383) into the pGP-Tn7-Gm backbone.

1.  Use Snapgene to make an *in silico* insert DNA cassette approximately 500 bp downstream and upstream of the gene of interest.
2.	Make Primers on NEBuilder according to the [Gibson Assembly Protocol](https://github.com/mjmlab/protocols/blame/master/gibson-assembly.md).
      * Use the [pGP-Tn7-Gm backbone](https://www.ncbi.nlm.nih.gov/nuccore/JQ429758.1?report=gbwithparts&log$=seqview) as the vector fragment, and amplify the vector from base pairs 1880 to 1810 (The MCS of the backbone).
      * Add the *in silico* insert DNA cassette as a fragment to the vector.
3.  Use the primers from NEBuilder to perform Gibson Assembly.
4.  Using heat shock, transform the donor strain vector into chemically competent S17-1 λ pir *E. coli* cells (MJM661).

## Transform recipient vector into recipient strain

Using heat shock, transform pSTNSK into KPPR1. ????

## Deliver Tn7 into Klebsiella

Using classical mating, integrate the Tn7 transposon into the KPPR1 chromosome.

1.  Start overnight cultures of the donor strain and the recipient strain.
2.  Pellet 500 uL of donor and recipient strains in seperate Eppendorf tubes (5 min max speed, Klebsiella may need a longer spin since it doesn't form a tight pellet)
3.  Remove all but 50 uL of LB from each tube and re-suspend each pellet in the remaining LB, then combine the resuspensions in a single tube. 
4.  Plate all 100 uL of mixed suspension on an LB plate and incubate at 30 degrees Celsius for 5 or 18 hrs.
5.  Use a cotton swab dipped in PBS to scrape up the cells, agitate to dislodge the bacteria in 1 mL of PBS in a 2 mL tube.
6.  Create serial dilutions out to 10^-8, and plate out onto LB-GM plates.
    * Incubate plates at 42 C for 4 hours, then 37 C for 18 hrs.
7. Streak out single colonies onto LB-Gm, LB-Carb, and LB-Km plates.
  * Look for resistance to Gm, sensitivity to Carb and Km.
8. Screen complementation candidates using PCR.
9. Freeze successful candidates and send to MIGS for sequencing.
    


