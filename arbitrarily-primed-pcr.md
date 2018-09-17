# Semi-Arbitrarily-Primed PCR to Identify Transposon Insertion Sites


## Primers

Select one ARB primer and one transposon-specific primer for each round.


| Transposon               | Round | Primer        | Sequence (5'-3')                       |
| ------------------------ | ----- | ------------- | -------------------------------------- |
| Any                      | 1     | ARB1          | GGCCACGCGTCGACTAGTACNNNNNNNNNNGATAT    |
| Any                      | 1     | ARB6          | GGCCACGCGTCGACTAGTACNNNNNNNNNNACGCC    |
| Any                      | 2     | ARB2          | GGCCACGCGTCGACTAGTAC                   |
| pMJM10, pEVS170, pEVS168 | 1     | 170Ext        | GCACTGAGAAGCCCTTAGAGCC                 |
| pMJM10, pEVS170, pEVS168 | 2     | M13 For (-20) | GTAAAACGACGGCCAGT                      |
| pMarVF1                  | 1     | MJM-440       | TCAACACACTCTTAAGTTTGCTTC               |
| pMarVF1                  | 2     | MJM-477       | TTCCATAACTTCTTTTACGTTTCC               |
| pJNW684                  | 1     | MJM-715       | CATCCTGTCTCTTGATCAGAGCTT               |
| pJNW684                  | 2     | MJM-716       | CTTCCCAACCTTACCAGAGG                   |

Use the transposon-specific Round 2 primer for DNA sequencing.

### Primer notes

MJM-477 (pMarVF1): Sequence is in the direction opposite that of the erm cassette (i.e., plus direction sequence indicates that the erm cassette is inserted into the chromosome in the minus orientation).

MJM-716 (pJNW684): Sequence is in the direction opposite that of the kan cassette (i.e., plus direction sequence indicates that the kan cassette is inserted into the chromosome in the minus orientation).


## DNA Preparation

Prepare genomic DNA (gDNA) from each candidate using the Qiagen DNeasy Blood & Tissue Handbook, using the Gram negative  pretreatment. Elute in 100 μl H<sub>2</sub>O, determine DNA concentration by Nanodrop, and normalize the concentration to 28.6 ng/μl.


## Semi-arbitrarily-primed PCR, Round 1

Recipe is for 50 μl reactions. Prepare master mix of a minimum of 10 reactions to avoid pipetting tiny volumes.

| Arb-PCR, Round 1                     | 50 μl Reaction | Master (n=20) |
| ----------------                     | -------------: | ------------: |
| 5X GoTaq Reaction Buffer (colorless) | 10.00          | 200           |
| dNTP Mix, 2.5 mM each                | 4.00           | 80            |
| primer1 (50 μM) - ARB1               | 0.50           | 10            |
| primer2 (50 μM) - Tn-specific1       | 0.50           | 10            |
| GoTaq DNA Polymerase (5u/μl)         | 0.25           | 5             |
| H2O                                  | 27.75          | 555           |
| gDNA of candidate (28.6 ng/μl)       |  7.00          | --            |


***ARB1***

    - 1 cycle:
        - 95 °C, 5 m
    - 5 cycles:
        - 94 °C, 30 s
        - 30 °C, 30 s
        - 72 °C, 1 m 30 s
    - 30 cycles:
        - 94 °C, 30 s
        - 45 °C, 30 s
        - 72 °C, 2 m
    - 1 cycle:
        - 72 °C, 5 m
    - Hold at 12 °C (and move to 4 °C fridge)


## Column purification

Purify each sample with the Qiagen QIAquick PCR Purification Kit. Elute in 50 μl H2O. Use 1 μl eluate as template for Arb-PCR Round 2.

## Semi-arbitrarily-primed PCR, Round 2

| Arb-PCR, Round 2                     | 50 μl Reaction | Master (n=20) |
| ----------------                     | -------------: | ------------: |
| 5X GoTaq Reaction Buffer (colorless) | 10.00          | 200           |
| dNTP Mix, 2.5 mM each                | 4.00           | 80            |
| primer1 (50 μM) - ARB2               | 0.50           | 10            |
| primer2 (50 μM) - Tn-specific2       | 0.50           | 10            |
| GoTaq DNA Polymerase (5u/μl)         | 0.25           | 5             |
| H2O                                  | 33.75          | 675           |
| Purified Round 1 Product             |  1.00          | --            |

***ARB2***

    - 30 cycles:
        - 94 °C, 30 s
        - 55 °C, 30 s
        - 72 °C, 1 m 30 s
    - 1 cycle:
        - 72 °C, 5 m
    - Hold at 12 °C (and move to 4 °C fridge)


## Column purification

Purify each sample with the Qiagen QIAquick PCR Purification Kit. Elute in 50 μl H2O.

*Note that even for successful samples a band is typically not observed by gel electrophoresis.*


## Sequencing

Check by Nanodrop. Yield should be 5-20 ng/ul; concentrate with a DNA Speedvac if concentration <5 ng/μl, and submit for DNA sequencing.


## Scaling Up

For large numbers of samples, consider the following changes to scale up the analysis:
- Use colonies or overnight culture diluted (1:100) in water, instead of gDNA prep.
- Do 10 μl PCR reactions.
- Use EXOSAP-IT in place of each column purification. This inactivates the previous round primers, so removing them is no longer necessary. Add 4 μl EXOSAP-IT to the Round 1 products and incubate. Then dilute the sample to 100 μl and use 1 μl of that sample in the Round 2 Arb reaction. Add 4 μl EXOSAP-IT to the Round 2 product and incubate. Then add sequencing primer and submit.

### EXOSAP-IT incubation
    - 1 cycle:
        - 37 °C, 15 m
        - 80 °C, 15 m
    - Hold at 12 °C (and move to 4 °C fridge)