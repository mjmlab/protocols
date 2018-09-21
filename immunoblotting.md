# Immunoblotting

The following [guide](https://www.bio-rad.com/webroot/web/pdf/lsr/literature/Bulletin_2895.pdf) from Biorad offers extensive information about choosing reagents, performing a blot, and troubleshooting.

## Supplies

- Methanol
- [Transfer Buffer](#transfer-buffer)
- [Membranes](#membranes)
- [Filter paper](#filter-paper)
- [Washing Buffer](#washing-buffer)
- [Blocking Buffer](#blocking-buffer)
- [Primary and Secondary Antibody Solutions](#antibody-solutions)
- Developing Solution (if using HRP conjugate secondary)
- Vacuum sealer and sealer bags

### Transfer Buffer
1x Towbin buffer is typically used. However, 0.1% SDS can be added to help transfer of higher molecular weight proteins.

**10x stock:**
  - Buy either Tris/Glycine (1610734) or Tris/Glycine/SDS (1610732) buffer from Biorad
  - 10x Buffer Recipe:

  Amount | Reagent | Final Concentration
  -- | -- | --
  30g | Tris base | 25mM
  144g | Glycine | 192mM
  10g | SDS - optional | 0.1% w/v
  1L | H2O |

**1x buffer:**
  - For 1L:
      mix 100 ml 10x Tris/Glycine buffer, 200 ml methanol, and 700 ml DI water  
  - For 1.25L (you may need extra for soaking membranes and filling tank):    
      mix 125 ml 10x Tris/Glycine buffer, 250 ml methanol, and 875 ml DI water

### Membranes
Size for miniprotean is 7 x 8.5 cm  

Nitrocellulose membranes are good general purpose membranes. PVDF membranes are less fragile and well suited for western blots.
If using fluorsecent instead of chemiluminescent detection, "low fluorescence" option helps reduce autofluorescence.
0.45 µm size is standard, but 0.2µm may be consdietred for proteins under 15kD.
Helpful [article](https://www.biocompare.com/Bench-Tips/134438-The-Magic-s-In-the-Membrane-Choose-Wisely-for-Best-Western-Blot-Results/) on membrane consideration.  

Biorad: Immun-Blot Low Fluorescence PVDF/Filter Paper Sets #1620261, [manual](https://www.bio-rad.com/webroot/web/pdf/lsr/literature/Bulletin_4006127A.pdf)

### Filter paper
Size for miniprotean is 7 x 8.5 cm

### Washing Buffer
Washing buffer is 1x TBS-T.

**10x TBS:**
- Buy 10x TBS stock (Fisher BP24711)
- Make 10x stock solution

Amount | Reagent
-- | --
24g | Tris-HCL
5.6g | Tris base
88g | NaCl
1L | H2O

Check that pH is 7.6 (mix of Tris-HCl and Tris base should make sure it is close). 

**1x TBS-T:**

Amount | Reagent 
-- | --
100 ml | 10x TBS
900 ml | DI H2O
1 ml | Tween-20  

In 1x buffer, concentrations should be 20mM Tris and 150mM NaCl.  

### Blocking Buffer
Blocking buffer is 5% milk (w/v) in 1x TBS-T.  
See [washing buffer](#washing-buffer) for recipe for 1x TBS-T.  

Amount | Reagent
-- | --
50 ml | 1x TBS
2.5g | non-fat powdered milk

### Antibody Solutions

Antibodies are diluted in 0.5% milk (w/v) in 1x TBS-T. For list of antibodies in the lab, see lab database.  
See [washing buffer](#washing-buffer) for recipe for 1x TBS-T.  

Amount | Reagent
-- | --
10 ml | 1x TBS
0.05g | non-fat powdered milk

If using a **PVDF membrane AND IRDye secondary** add 0.01% SDS to the secondary antibody solution (100 ul of 1% SDS).

Use the following table as a reference for how much antibody to add to 10 ml:

Amount | Concentration
-- | --
200 ul | 1:50
100 ul | 1:100
20 ul | 1:500
10 ul | 1:1,000
2 ul | 1:5,000
1 ul | 1:10,000
0.75 ul | 1:15,000
0.5 ul | 1:20,000

## Dot blot
Instead of running a gel, samples can be spotted directly onto the membrane. This is used for quick check to confirm antibodies work and can be used to gauge antibody concentration that can be used. Handle membrane with forceps minimizing contact with central area of membrane.

1. Place membrane in a dish. If PVDF membrane, soak in 100% methanol for ~1 minute, then equilibrate in 1x TBS buffer until membrane "sinks" in buffer. Let membrane puddles dry, but do not let membrane completely dry out.
1. Spot 2-10ul of sample onto gel.
1. Let spots dry ~15-30min. Make sure they are completely dry
1. Use scissors to clip one corner so you remember which side and orientation the proteins are on.
1. Proceed with [staining](#staining) procedure

## Western Blot Transfer
See page 25 in [guide](https://www.bio-rad.com/webroot/web/pdf/lsr/literature/Bulletin_1658100.pdf) for more details and pictures. Note: For larger gels use the criterion system.
Supplies, including square clear plastic containers that can be used to soak parts, are in protein supply cabinet. Handle membrane with forceps minimizing contact with central area of membrane.  
1. After running [SDS-PAGE gel](sds-page.md), let gel equilibrate in transfer buffer for ~10 min
1. Soak 2 sponges and 2 pieces of filter paper in transfer buffer.
1. Soak membrane in transfer buffer. If using PVDF membrane, wet in methanol first.
1. Assemble the transfer "sandwich". Throughout assembly, transfer buffer can be added by pouring onto sandwich to keep layers wet and help parts come together without air bubbles.
    - On a paper towel pile or within a container, place cassette open with black side as the base.
    - Place on one sponge, followed by one piece of filter paper onto the black base of cassette.
    - Place on gel. Remember, when it gets transferred to the membrane, it will be the mirror image of how you place it in sandwich. Use roller to remove any air bubbles.
    - Place on membrane carefully. Do not adjust membrane once it has touched gel.
    - Place on second piece of filter paper. Use roller to remove bubbles
    - Place on second sponge.
    - Fold clear part of cassette over and clasp. Do this over tank system as excess buffer will be squeezed out when you clasp the cassette.
1. Place cassette into red/black electrode so the black plate is facing the black side and the clear plate it facing the red side.
1. Fill tank with transfer buffer and put on lid
1. Plug tank into HC power supply in the cold room (4C).
1. Run at 100V for 1 hour
    - Alternatively, an overnight transfer (16 hrs) can be done at 30V.
    - If transfer looks uneven, a stir bar can be added to and tank places on a stir block to keep buffer a more uniform temperature. However, placing the entire unit in the cold room has been sufficient thus far.
    - NOTE: For smaller proteins (<30 kD), high voltage may cause them to transfer through the membrane. Use a shorter time (20-30 min) or do an overnight transfer. Most proteins will transfer within 30-45 min, and only large ones (150 kD) need the full 60 min.
1. Remove membrane from the sandwich. Use scissors to clip one corner so you remember which side and orientation the proteins are on.
1. Proceed with [staining](#staining) procedure

## Immunostaining

A list of primary and secondary antibodies we have is located on the lab database. If you are testing a new antibody, please record the antibody in the database along with optimal concentration used.

Besides blocking step, all other steps are carried out at room temperature.

1. Block membrane overnight in 50 ml of 5% non-fat milk. Use clear square containers with lid. Place at 4C.
1. To minimize antibody needed, make small plastic baggie for vacuum sealer that is just larger than the membrane.
1. Place membrane in baggie. Add 10 ml of primary antibody solution. Seal baggie (DO NOT use vacuum setting, just seal). Rock 1 hour.
1. Remove membrane from baggie and place in wash container (blue tip box)
1. Wash 4x for 15 min rocking in 50 ml wash buffer.
1. Place membrane in fresh baggie. Add 10 ml of secondary antibody solution. Seal baggie and wrap with foil since secondary antibodies are light sensitive. Rock 1 hour.
1. Remove membrane from baggie and place in wash container (blue tip box). Cover with foil to protect from light.
1. Wash 4x for 15 min rocking in 50 ml wash buffer. If using IRDye antibody, use TBS instead for the final 15 min wash.
1. If using HRP antibody, use chemical developing solution to activate antibody.
1. Place membrane in plastic wrap and cover with foil to protect from light.
1. Go to 3rd floor core room and use [Li-Cor Odyssey FC](https://www.licor.com/documents/iyu8ffsef0gk2xxd7w8e) to image.
    - This imager can develop chemiluminescent (HRP) or fluorescent (IRDye) blots. There are old fashioned developers on in the 3rd floor and 5th floor cores if you have film paper and want to do it the old fashioned way.
