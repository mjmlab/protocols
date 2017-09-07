# Gene Deletion in *Vibrio fischeri*

This protocol describes gene deletion in *V. fischeri* by allelic exchange.

## Clone the allelic exchange vector

1. Clone approximately 1.6 kb upstream DNA and 1.6 kb downstream DNA adjacent to each other. Aim for similar sized upstream and downstream fragments so that crossovers on either flanking side are equally likely. Suggested method: Gibson Assembly cloning in pEVS79. The following protocol assumes a vector containing chloramphenicol resistance was used and the LBS-Cam concentration was 1.0 μg/ml unless otherwise stated.

<!-- add additional info, vectors, pictures, etc. -->

## Introduce the deletion vector to the *V. fischeri* recipient

1. [Conjugate](conjugation.md) the plasmid from *E. coli* into *V. fischeri*
  - Plate the 10 μl conjugation spot onto LBS agar and incubate overnight at 25°C. Note: Some strain backgrounds mate better on fresh LBS plates and some mate better on older, dry LBS plates.
  - Scrape the spot into 700 μl LBS.
  - Plate 50 μl of the resuspension and 10<sup>-1</sup>, 10<sup>-2</sup>, 10<sup>-3</sup> dilutions of the resuspension onto LBS-Cam plates (make sure the concentration is greater than 2.5 μg/ml to prevent background growth). Incubate overnight at 25°C.

## Isolate single recombinants

Isolate strains in which the allelic exchange vector has integrated at the chromosomal locus through a single crossover either at the upstream flank or the downstream flank.

1. Once single colonies appear (may take 2 days), select approximately 50 isolated colonies (transconjugants) and restreak onto LBS-Cam for single colonies. (Note that you can streak >1 colony per plate - as many as 12 as long as there are isolated colonies). Incubate overnight at 25°C.

1. The next day, streak colonies to LBS and LBS-Cam(0.5), no more than 8 per plate. Include the parent strain as a negative control - this strain will grow very poorly on the intermediate antibiotic concentration. Incubate overnight at 25°C. Alternately, incubate for two nights on the benchtop.

1. Observe the streaks using a stereomicroscope. Most streaks will have a mix of large colonies and tiny colonies that are roughly the size of the parent strain - these are the transconjugants that are in the process of losing the plasmid. Look for the streaks that have only large sized colonies - there will likely be only one or two candidates.
1. Streak the candidate colonies to LBS and incubate overnight at 25°C. As controls, also streak a non-candidate and the parent strain.
1. Patch 4 colonies per candidate (and controls) from the LBS streak onto LBS-Cam and LBS. Incubate overnight at 25°C.
  - Pro tip: patch each set of four in opposite directions to track each isolate: `/ / / / \ \ \ \ / / / /`

1.  Identify transconjugants in which 3 or 4 of the 4 patches are antibiotic resistant. **These are the single recombinants, the isolates in which the allelic exchange vector has integrated into the chromosome--and is therefore maintained even in the absence of selection**. 

1. For each transconjugant in which the plasmid has integrated, inoculate one of the chloramphenicol-resistant patches into 3 ml LBS-Cam and grow overnight at 25°C to prepare a -80°C freezer stock. Simultaneously inoculate 3 ml LBS with the candidate(s) from the LBS plate to identify the double recombinants below (see next step...).

## Isolate double recombinants

Isolate a single recombinant-derived strain in which the allelic exchange vector has recombined out of the chromosomal locus through a single crossover at the opposite flank, leaving the deletion construct instead.

1. From the patch above or from the -80°C freezer stock of the single recombinant, inoculate 3 ml LBS in duplicate. Alternately, dilute in duplicate an overnight culture 1:1000 in 3 ml LBS. Grow at 25°C until slightly turbid (OD<sub>600</sub> ≈ 0.2). 

1. Dilute cultures 1:1000 into 3 ml LBS and grow at 25°C until again slightly turbid.

1. Plate for single colonies on LBS (10<sup>-3</sup>, 10<sup>-4</sup>, 10<sup>-5</sup> dilutions). Incubate at 25°C overnight.

1. Patch ~80 -100 single colonies onto LBS and LBS-Cam. Antibiotic sensitive mutants have likely lost the allelic exchange vector. They may be the potential double recombinant (mutant) or they may have reconstructed the wild-type strain.

1. Screen 8 potential mutants using PCR.


## Verify deletion constructs

1. Screen for:
  - Absence of deletion DNA
  - New junction created by the deletion
  - Absence of plasmid backbone material (i.e., that you are not simply observing mutation of the cam cassette).



Adapted from a protocol from Anne Dunn
