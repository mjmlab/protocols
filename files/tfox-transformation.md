# Transformation in *Vibrio fischeri* using inducible *tfoX*-expressing vectors

This protocol describes transformation of an antibiotic resistant cassette in *V. fischeri* using transient *tfoX* induction. The *V. fischeri* recipient expresses *tfoX* from the pLostfoX or pLostfoX-Kan vector; introduces the donor DNA and selects for its integration; and then releases selection for the vector to allow it to be lost. Diagnostic PCR is used to confirm incorporation of the cassette at the expected chromosomal locus.

### Choice of transformation vector

pLostfoX has a chloramphenicol-resistant (Cam<sup>R</sup>) backbone

- If instead a kanamycin-resistant (Kan<sup>R</sup>) vector is desired, use pLostfoX-Kan (originally called pJFB9) and substitute 100 μg/ml Kan for each instance of 2.5 μg/ml Cam denoted by asterisks (\*\*).
- Here we will use MJM1538 (MJM1100 / pLostfoX).  
- pLostfoX can be introduced to other strains by [conjugation](files/conjugation.md) from MJM1529 (DH5α / pLostfoX) with selection for Cam.  
- MJM2076 is MJM1100 / pLostfoX-Kan.  
- pLostfoX-Kan can be introduced to other strains by [conjugation](files/conjugation.md) from MJM2090 (DH5α λpir / pLostfoX-Kan) with selection for Kan.  


### Materials

**Recipient**: *V. fischeri* containing pLostfoX

**Donor** Genomic DNA (gDNA): 2.4 μg prepared with the Qiagen DNeasy kit, eluted in ddH<sub>2</sub>O. Final concentration of > 100 μg/ml.

[Antibiotic](files/antibiotics.md) to select for your marker of interest.

[Antibiotic](files/antibiotics.md) to select for the pLostfoX plasmid (Cam)\*\*.

[LBS](files/media.md#lbs) liquid and agar as noted, some containing antibiotics.

Tris-GlcNAc-Cam: [Tris minimal medium](files/media.md#tris-minimal-medium) with 10 mM GlcNAc and 2.5 µg/ml Cam\*\*.


1. **Day 1** - Inoculate 3 ml LBS-Cam<sup>2.5</sup>\*\* with the recipient. Grow culture overnight in the 25 °C rotator.

1. **Day 2** - Inoculate 3 ml fresh Tris-GlcNAc-Cam\*\* with 30 μl of the overnight culture of the recipient. Grow culture overnight in the 25 °C rotator.  

1. **Day 3** - Subculture 150 μl of the overnight minimal culture into 3 ml fresh Tris-GlcNAc-Cam\*\*, and grow at 25 °C with aeration.
1. At OD<sub>600</sub>=0.2, transfer 500 μl of culture to a 2 ml microfuge tube and add 2.4 μg gDNA (typically < 25 μl). Vortex briefly, then leave culture at room temperature without shaking for 30 min.
1. Add 1 ml LBS, transfer to a 16 mm diameter glass culture tube, and incubate in the 25 °C rotator for recovery overnight (can reduce to 1 h if needed to limit siblings).

1. **Day 4** - Plate 50 μl onto selective media (e.g., LBS-Erm<sup>5</sup> for transfer of an erythromycin-resistance cassette).

1. **Day 5** - Restreak on selective media (pursue 3 candidates/each).

1. **Day 6** - Patch candidates onto media to check for the presence of the transformation plasmid (e.g., LBS-Cam<sup>2.5</sup> \*\*), and media to ensure transformation (e.g. LBS-Erm<sup>5</sup>). While patching, inoculate the same candidates into liquid medium (e.g., LBS-Erm<sup>5</sup>) to grow overnight.

1. **Day 7** - The desired colonies will have gained the desired selectable marker and subsequently lost the pLostfoX plasmid (i.e., are now Cam<sup>S</sup>\*\*).  For a candidate that is resistant to your selective marker and Cam<sup>S</sup>\*\*, freeze a glycerol stock in the MJM collection.  Verify that the marker of interest was transferred by site-specific PCR. Typically chromosomal insertions are stable in *V. fischeri*; it is a good idea to also check that the strain remains resistant to the cassette marker (e.g., Erm<sup>R</sup>) even after non-selective passage.


### References

Protocol from [Brooks et al., PMID: 25404340](https://www.ncbi.nlm.nih.gov/pubmed/25404340) and updated [here](https://github.com/mjmlab/protocols/blob/master/tfox-transformation.md)

pLostfoX: [Pollack-Berti et al., PMID: 21966921](https://www.ncbi.nlm.nih.gov/pubmed/21966921)

pLostfoX-Kan: [Brooks et al., PMID: 25404340](https://www.ncbi.nlm.nih.gov/pubmed/25404340)
