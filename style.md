# Style and Writing Guide

> Please use this page as a guide, not as a definitive resource. My goal here is to help us adopt shared  nomenclature and avoid common mistakes. It is somewhat opinionated (needed for a standard); likely has some errors (I'm not an expert writer); and is subject to evolve over time. The overall goal is always clarity, so if you have an unusual case, it is better to be clear than to strictly adhere to these guidelines.


## Style Guide

### Basic description

Chromosome genotype / plasmid genotype (e.g., `MJM1100 / pVSV102`).

Do:
- Use the full MJM numbers (MJM1100 instead of 1100)
- Use the MJM number as the chromosome genotype instead of the strain common name (MJM1100 instead of ES114); this helps to show the lineage.
- Add in the `Parent` field any genomes that contributed DNA. E.g.:
    - If you transform genomic DNA from MJM1299 into MJM1529, then list the Parent as: `MJM1529;MJM1299`
    - If you conjugate a plasmid from MJM580 into MJM1100, then list the Parent as: `MJM1100;MJM580`
    - The order of strains listed in the `Parent` field does not matter.

Avoid:
- If the strain comes from another lab and/or has unknown lineage, do not substitute an MJM number for a genotype. i. E.g., if you receive a plasmid from a lab and the genotype is listed as DH5α / pUC18, record this as the genotype. Do not enter an MJM number for the chromosomal genotype. This is because we are using this information to track lineage, and it was not derived from our lab’s stock of DH5α. 

### Genes versus proteins

Bacterial genes are denoted with italics and first letter lowercase (e.g., *rpoS*) whereas proteins are not italics and have first letter uppercase (e.g., RpoS). 

More broadly, DNA is denoted in italics (including sites, etc.), and gene products are not italics with first letter uppercase (e.g., small RNA products).

In the database we will not worry about italics.

### Point mutations

Typically, use the protein address since this is what is widely used. It's a bit of a mismatch of the gene nomenclature with the protein change, but for clarity this seems to make the most sense for our typical usage.

- MJM1100 *binK*(H362Q)
- MJM1100 *binK*(H362Q, D794A)

If you need to use the DNA address indicate so with `nt` for nucleotide:

- Deleted base: *sypE*(ntG33Δ)
- Deleted multiple bases (small number): *sypE*(ntGAA33Δ)
- Deleted multiple bases (large number): *sypE*(nt33-65Δ)

Inserted base: sypE(nt33::G)

## Fusions

Transcriptional fusion: MJM1100 *binK’-gfp<sup>+</sup>*

Translational fusion: MJM1100 *binK’-‘gfp*

## Transposon insertions
 
Insertions are denoted by two colons, which are not italicized: `::`

Typical practice for our lab been to record using the antibiotic of the transposon: MJM1198 *dnaJ*::Tn*erm*

Separately in the database record indicate the transposon used.

In some cases you will see more information about the transposon, which should typically be italicized: e.g., Tn*5*.

# Plasmid naming

Three options:
- pBinK or other functional information.
- pAB1, pAB2, etc. (use your initials).
- pM3000 for the plasmid first deposited as MJM3000.

## Genotypes for common gene manipulation procedures

Plasmid complementation: 
- Plasmid name, pBinK (or see other options above)
- Plasmid genotype: pVSV104-*binK*
- In the Notes section of the database for this plasmid, list methods for its construction (primer sequences, amount of DNA upstream/downstream cloned, etc.)

Chromosomal complementation:
- Plasmid: pEVS107-*binK*
- Chromosomal genotype: MJM2251 *att*Tn*7*::*binK-erm*

Plasmid-based deletion:
- Plasmid for deletion of binK: pEVS79-Δ*binK*
- Single integrant: MJM1100 *binK*::pEVS79-Δ*binK*
- Double integrant: MJM1100 Δ*binK*

erm-bar and bar alleles:
- *copA*::*erm-bar*
- *copA*::*bar*

Avoid spaces in plasmid names (use dash “-“ instead).

## Alleles from another strain/species

From another strain/species:
- pVSV104-*binK*<sub>MJM1125</sub>. In the database, could record this as `pVSV104-binK[MJM1125]`

## Promoters
P<sub>*binK*</sub>-*gfp*<sup>*+*</sup>
- binK promoter driving GFP.

## Locus tags

NCBI locus tags for Vibrio fischeri ES114 look like VF_0001 (chr 1 gene 0001), VF_A0001 (chr 2 gene 0001), or VF_B0001 (plasmid pES100 gene 0001). The underscore should be included in all relevant genotypes. Note that earlier versions of NCBI locus tags lacked the underscore (and had 2-digit plasmid gene numbers); therefore, to find all records for binK you should search for all three terms: binK, VF_A0360, and VFA0360. The first set of plasmid locus tags had only two digits (VFB55) but now all have four digits (VF_B0055). Additionally, some locus tags have been combined due to corrections to the genome. You can search NCBI and find any “old_locus_tag”s for a gene of interest. 

More information about the VF locus tags is available in [Mandel et al. 2008 BMC Genomics](https://bmcgenomics.biomedcentral.com/articles/10.1186/1471-2164-9-138).

The above VF locus tags should be used, and not the VF_RS locus tags.

## Writing Guide

### Write plainly to improve clarity

Change `in order to` to `to`.

Change `utilize` to `use` (unless you are utilizing something for an unintended purpose).

Here are some examples of [words and phrases to avoid from Laura Helmuth](https://twitter.com/laurahelmuth/status/1158039072067264515?s=12), and the replies have some others' corrections (and pet peeves).

### Singular/plural and ensure noun-verb agreement

`The group of animals are found in Hawaii.`: Replace `are` with `is` to agree with the singular `group`.

The word `data` is plural. Many will disagree, and in modern usage it is often used as a "singular mass noun." But we don't!

### Which vs that

`which` typically follows a comma, while `that` does not:

The bacteria grew well, which indicated that the mutation did not impact viability.

### Capitalization

`Gram` (Gram stain; Gram-negative; Gram-positive) is capitalized for [Hans Christian Gram](https://en.wikipedia.org/wiki/Hans_Christian_Gram).

`Southern` blot capitalized for [Edwin Southern]; northern blot and western blot are lowercase.

Some journals may disagree.

### Separating clauses

#### However

Improper use:

```Blah blah, however bluh bluh.```

Proper alternatives (as long as "blah blah" and "bluh bluh" are both independent clauses):

```
Blah blah. However, bluh bluh.
Blah blah; however, bluh bluh.
Blah blah, yet bluh bluh.
```

#### And (and commas)

Use a comma before `and` only if you are joining two independent clauses (i.e., two phrases that could be full sentences on their own):

Improper use:

```
This experience allowed me to learn more, and impacted my life.
```

Proper alternatives:

```
This experience allowed me to learn more and impacted my life.
This experience allowed me to learn more, and it impacted my life.
```

### Space out

There should be a space between a value and its unit.

```
8 mm
25 °C
100 μl
```

The exception to this if you are describing an angle: `90° right angle`

### Special characters

In general, use unicode symbols, not the symbol font. This way, as you change fonts (or submit your abstract to an online system, etc.) you do not lose information.

Mac shortcuts (if known):

| Symbol  | Keyboard Shortcut  |
|---------|--------------------|
| µ       | Option-m           |
| ∆       | Option-j           |
| ≤       | Option-,           |
| ≥       | Option-.           |
| ≈       | Option-x           |
| ‰       | Option-Shift-R     |
| π       | Option-p           |
| β       |                    |
| λ       |                    |
| σ       |                    |
| α       |                    |

Use `µl` instead of `ul`

[Here](https://cdn.shopify.com/s/files/1/0810/3669/files/us-international-pc_1024x1024.png?6574517274645660029) is a diagram that may be helpful to print, from this [post by Sebastian Kończak](https://keyshorts.com/blogs/blog/41999105-the-ultimate-guide-to-macbook-keyboard).

Another hack: copy the symbols you need from above, or from a [relevant Wikipedia article](https://en.wikipedia.org/wiki/Greek_alphabet). Paste them without formatting (e.g., in your browser's address bar) to confirm that you have a unicode symbol, then copy it from there and paste the plain text version of it into your document.

### Italics

- `7` in Tn*7* 
- `5` in Tn*5*
- *in vivo*
- *in vitro*

Additional detail above in the [Style Guide](#style-guide) for genes, promoters, etc.

### American English

Use the common American English spelling and usage (unless writing specifically for a British English audience).

| Use             | Avoid            |
|-----------------|------------------|
| Acknowledgments | Acknowledgements |
| behavior        | behaviour        |
| color           | colour           |
| among           | amongst          |


### Wild type vs wild-type

I'll admit to often getting this one wrong! `Wild-type` is an adjective (`wild-type bacterium`) whereas 
`wild type` is a noun (`the wild type did not have the phenotype`). [This post from Kathryn Sobek](https://filipodia.com/2017/03/01/is-it-wild-type-or-wild-type/) has additional examples.

### References

Include spaces before citations (unless they are superscript, or this format is required by the journal). 

`See this paper(10)` should instead be: `See this paper (10)`

When possible, put all references at the end of the sentence. It makes it easier for the reader to read and understand your writing. the exception to this is when you have a citation that must be cited precisely with a certain word/phrase, such as:

`The consensus in the literature is X (1, 2), but our data suggest otherwise (Fig. 2).`

In the bibliography list, pay attention to formatting. Italicize genus/species/gene names if they are italicized in the original manuscript title. Use superscript/subscript as appropriate. Here is code you can add to your titles in Paperpile so that it fills correctly:

```
<i>Vibrio fischeri</i> colonizes the Hawaiian bobtail squid, <i>Euprymna scolopes</i>
Transcription is controlled by σ<sup>54</sup>
Subscripts are less common in paper titles<sub>Am I right?</sub>
```

### This

Whenever you have a sentence that begins with `This`, be sure you are explaining what `This` is.

As examples:

`This highlights the power of our approach.` might be better expressed as `The depth of the results we obtained highlights the power of our approach.`

`This makes it clear that more investigation is needed.` could be `This finding that many insertions cannot be explained makes it clear that more investigation is needed.`

### Hyphenation

Avoid hyphenation on posters. When you have narrow text blocks, many programs will hyphenate the ends of lines. This becomes distracting when it occurs too often.

This issue occurs frequently in Illustrator for posters: In `Paragraph`, deselect the `Hyphenate` option.

This issue occurs rarely in Word, though you can disable hyphenation in `Paragraph` | `Line and Page Breaks` | `Don't hyphenate`

### Tracking changes

After accepting/rejecting comments, be sure to review for issues of 2 spaces or 2 periods in a row. Do a search in the whole document for these issues, and review each manually.

