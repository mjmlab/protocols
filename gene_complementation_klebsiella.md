# Gene Complementation in *Klebsiella Pneumoniae*

This protocol describes complementation of a gene back into Klebsiella using Tn7.

## Insert gene of interest into donor strain's vector backbone using Gibson Assembly

Insert DNA cassette containing the gene of interest from KPPR1(MJM2383) into the pGP-Tn7-Gm backbone.

1.  Use Snapgene to make an *in silico* insert DNA cassette approximately 500 bp downstream and upstream of the gene of interest.
2.	Make Primers on NEBuilder according to the [Gibson Assembly Protocol](https://github.com/mjmlab/protocols/blame/master/gibson-assembly.md).
      * Use the [pGP-Tn7-Gm backbone](https://www.ncbi.nlm.nih.gov/nuccore/JQ429758.1?report=gbwithparts&log$=seqview) as the vector fragment, and amplify the vector from base pairs 1871 to 1824 (The MCS of the backbone).
      * Add the *in silico* insert DNA cassette as a fragment to the vector.
3.  Use the primers from NEBuilder to perform Gibson Assembly.
4.  Using heat shock, transform the donor strain vector into chemically competent β3916 E. *coli* cells (MJM628).
5.  Use PCR screening to determine if the Gibson Assembly and transformation was successful.

## Transform recipient vector into recipient strain

Introduce pSTNSK-Cm into KPPR1 strain with respective deleted gene via electroporation.

1.   Inoculate 100 mL LB with 1 mL of overnight culture. Incubate at 30C with stir bar at ~500 rpm until it reaches OD<sub>600</sub> of 0.6 to 0.8 (approximately 4 hours). 
2.   Centrifuge cells at 6500 rpm for 5 min. Remove supernatant and wash twice with 50 mL of ice cold glycerol (resuspend with glycerol and then centrifuge it again). 
3.   Resuspend cells in residual glycerol solution after final wash. Mix 50 uL of dense suspended cells with 1 ug of plasmid DNA (<= 6 uL) in an electroporation cuvette. Use the manual mode on the electroporation machine and use the arrows to increase the voltage to 2.5V. Make sure that the cuvette is perfectly vertical before pressing the pulse button, or else there's a very large chance of arcing. Add 900 uL SOC medium immediately after electroporation. 
4.   Incubate sample for 1 hour at 30 degrees C on a rotary shaker at 150 rpm and plate onto low salt LB-Cam25 plates.
5.   Incubate plates at 30 degrees C overnight.
6.   Streak colonies onto low salt LB-Cam25 plates, and then again the next day.
7.   PCR Screen for pSTNSK-Cm. 
8.   Freeze successful colonies and use for complementation.


## Deliver Tn7 into Klebsiella

Using classical mating, integrate the Tn7 transposon into the KPPR1 chromosome.

1.  Start overnight cultures of the donor strain and the recipient strain.
2.  Pellet 500 uL of donor and recipient strains in seperate Eppendorf tubes (5 min max speed, Klebsiella may need a longer spin since it doesn't form a tight pellet)
3.  Remove all but 50 uL of LB from each tube and re-suspend each pellet in the remaining LB, then combine the resuspensions in a single tube. 
4.  Plate all 100 uL of mixed suspension on an LB-DAP plate and incubate at 30 degrees Celsius for 5 hrs.
5.  Use a cotton swab dipped in PBS to scrape up the cells, agitate to dislodge the bacteria in 1 mL of PBS in a 2 mL tube.
6.  Create serial dilutions out to 10^-4, and plate out onto LB-GM plates.
7. Incubate plates at 42 C for 4 hours, then 37 C for 18 hrs.
8. Streak out single colonies onto LB-Gm, LB-Carb, LB-Kan and LB-Cam plates.
     * Look for resistance to Gm and Kan, sensitivity to Carb and Cam.
9. Screen complementation candidates using PCR.
10. Freeze successful candidates and send to MIGS for sequencing.
    


