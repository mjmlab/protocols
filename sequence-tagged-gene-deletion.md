# Sequence Tagged Gene Deletion
by Hector Burgos

This protocol details how to generate a clean deletion of target genes in *Vibrio fischeri* where each deletion strain is tagged with a unique sequence or "barcode".
SOE-PCR is used to generate the Mutagenic DNA (linear dsDNA carrying Erm<sup>R</sup> and the barcode, flanked by FRT sites and upstream and downstream homology to target gene; arranged as follows: US homology-FRT-Erm<sup>R</sup>-FRT-barcode-DS homology) and *tfoX* transformation is used to insert it into *V. fischeri* where it recombines into the chromosome based on sequence homology.
This technique then allows for the excision of the Erm<sup>R</sup> cassette by expressing FLP recombinase, which uses the FRT sites to remove the antibiotic cassette.
The resulting scar is in-frame (reduces likelihood of polar effects on gene expression) and carries a barcode that allows identification of the specific deletion strain through sequencing.
One important detail is that the start codon and the last 7 codons (including stop codon) of the targeted gene are preserved and form part of the deletion scar.
The overall approach is summarized below:

<IMG SRC="/images/sequence-tagged-gene-deletion/sequence-tagged-gene-deletion-approach.png" WIDTH=425>

## Oligo Design

<IMG SRC="/images/sequence-tagged-gene-deletion/Oligos-Gene-Deletion.png" WIDTH=900>
<br><br>
Oligos F1 and R1-LUH amplify 1Kb upstream of target gene including the start codon, while oligos F2-RUH and R2 amplify the 1 Kb downstream of target gene including the last 7 codons (last 6 aa and the stop codon).
Oligo FO anneals 1.5 Kb upstream of target gene and is used to amplify from outside the junction of the mutation to verify insertion of cassette in correct genomic location.
Oligos FW and RW anneal within target gene and should produce no product from a successful gene deletion strain.

1. Generate a sequence file containing the gene of interest and 2 Kb of flanking sequence.
2. Substitute the coding sequence of the gene of interest with the barcoded Erm<sup>R</sup>-Marker within the start codon and the last 7 aa plus stop codon of the gene of interest. [Example: *ΔcueR*::erm-bar.](https://benchling.com/s/seq-b4AyxNqFLv25wjchrTqZ)
3. Using the distances shown in the image above as a guide, select oligos with a Tm = 60 ± 3°C (verify Tm with the "Analyze" function of [IDT's OligoAnalyzer 3.1 tool](https://www.idtdna.com/calc/analyzer)). \*Make sure oligo R1 starts with the start codon of the gene of interest, while F2 should include the last 7 codons.
4. Attach the reverse complement of LUH to R1 and RUH to F1 to form the R1-LUH and F1-RUH oligos (LUH Reverse complement = CTGGCGAAGCATATATAAGAAGCTCGTCTCGT; RUH = GACTTGACCTGGATGTCTCTACCCACAAGATCG).
5. Calculate the predicted secondary structures for the oligos using the "Hairpin" function of [IDT's OligoAnalyzer 3.1 tool](https://www.idtdna.com/calc/analyzer) and reject oligos with predicted structures with a Tm ≥ ~45°C.

## Ordering Oligos
1. Sign in to [Shop@UW](https://mds.bussvc.wisc.edu/order/shopper_lookup.asp) using the Mandel Lab login, select "Shop at External Suppliers & UW-Madison MDS Warehouse",
 and navigate to IDT's webpage.
2. Under "Products & Services" tab, go to "Custom DNA oligos" and select "DNA oligos".
Oligos can be ordered in tubes or in 96-well plates (24 oligos minimum; select "all ordering options" when navigating to "DNA oligos").
3. For ordering multiple oligos:
  - In tubes: select "bulk input", download an oligo input template, fill in your oligos, then upload to IDT.
  - 96-well plate: select "upload plate", download the "Excel plate ordering template", fill in your oligos, and upload. Name your plate with a unique but simple name, as oligo location is entered into Mandel Lab database in the "Plate, well" format. Under "plate specifications", select "normalized yield" for "normalization type", and "calculate" the "quantity (nmol)" and input the max option (e.g., 4-5 nmol).

\* Oligos are generally ordered at the 25 nm scale, where oligo size is limited to 60 bp for tubes and 80 bp for 96-well plate.
If oligos are larger than the allowed size (usually R1-LUH and F2-RUH), delete bases from the 5'-end of the oligo until size is reduced to the allowed size (up to 5 bp can be deleted without causing issues downstream; I haven't tested longer deletions); otherwise you can order in 100 nm scale, though this is not recommended for plates as you will have to order a separate plate for each synthesis scale.

4. Once you are sure that your order is set up correctly, place order in IDT, which will take you back to Shop@UW, then follow the prompts to finish the order.
5. Record order in Mandel Lab supplies log.
6. Once oligos arrive, record order as received, add TE to 100 µM, then prepare 10 µM working dilutions of the oligos (when using plates, prepare the 10 µM working dilutions in 0.2 mL striptubes; this allows the use of a multichannel pipette and ensures appropriate storage of the oligos).

## Amplification of Upstream (US) and Downstream (DS) Homology Arms

## Amplification of Barcoded Erm<sup>R</sup> Marker

## SOE-PCR and Generation of Mutagenic DNA

## *tfoX* Transformation

## Screening and Sequencing Δ*gene*::erm-bar Candidates

## Removal of Erm<sup>R</sup> by FLP Recombinase

## Screening and Sequencing Δ*gene*::bar Candidates

## Adding Deletion Strains to Database
\* Barcode in notes?
