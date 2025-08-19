---
# MIOP terms
methodology_category: Omics Analysis
project: Marine Biodiversity Observation Network (MBON)
purpose: PCR [OBI:0000415]
analyses: PCR [OBI:0000415]
geographic_location: Monterey Bay [GAZ:00002509]
broad_scale_environmental_context: marine biome [ENVO:00000447]
local_environmental_context: upwelling [ENVO:01000005]
environmental_medium: sea water [ENVO:00002149]
target: 18S [NCIT:C48172]
creator: # names separated by commas
materials_required: vortexer [OBI:0400118], PCR instrument [OBI:0000989], agarose gel electrophoresis system [OBI:0001134]
skills_required: sterile technique, pipetting skills, standard molecular technique
time_required: # minutes (integer)
personnel_required: 1
language: en
issued: # YYYY-MM-DD
audience: scientists
publisher: # institution
hasVersion: 1
license: CC0 1.0 Universal
maturity level: mature

# FAIRe terms
pcr_0_1: # 1
thermocycler: Bio-Rad T100
amplificationReactionVolume: 75
assay_name: # ssu16sv4v5_emp
assay_validation: # not provided
targetTaxonomicAssay: 18S rRNA gene sequencing targeting the V9 region using primers 1391F and EukBr
targetTaxonomicScope: Eukaryotes with a focus on microbial eukaryotes
target_gene: 18S rRNA
target_subfragment: V9
ampliconSize: ~260 +/- 50 bp
pcr_primer_forward: GTACACACCGCCCGTC
pcr_primer_reverse: TGATCCTTCTGCAGGTTCACCTAC
pcr_primer_name_forward: 1391F
pcr_primer_name_reverse: EukBr
pcr_primer_reference_forward: 10.1371/journal.pone.0006372
pcr_primer_reference_reverse: 10.1371/journal.pone.0006372
pcr_primer_vol_forward: 3.0
pcr_primer_vol_reverse: 3.0
pcr_primer_conc_forward: 5
pcr_primer_conc_reverse: 5
probeReporter: not applicable
probeQuencher: not applicable
probe_seq: not applicable
probe_ref: not applicable
probe_conc: not applicable
commercial_mm: AmpliTaq Gold™ Fast PCR Master Mix
custom_mm: PCR reactions were run in 75 uL reaction volumes, with 3.0 uL of DNA, 37.5 uL of AmpliTaq Gold, 28.5 uL of water, and 3.0 uL of each primer (5 uM)
pcr_dna_vol: 3.0
pcr_rep: 1
nucl_acid_amp: # https://doi.org/10.1111/1462-2920.13023
pcr_cond: initial denaturation:95_10;denaturation:94_0.75;annealing:57_0.50;elongation:68_1.5;final elongation:72_10;35
annealingTemp: 57
pcr_cycles: 35
pcr_analysis_software: not provided
pcr_method_additional: not provided
---

# Environmental DNA (eDNA) 18S metabarcoding PCR Protocol V.3

## PROTOCOL INFORMATION

### Minimum Information about an Omics Protocol (MIOP)

- MIOP terms are listed in the YAML frontmatter of this page.
- See [MIOP_definition.md](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/MIOP_definition.md) for list and definitions.

### Making eDNA FAIR (FAIRe)

- FAIRe terms are listed in the YAML frontmatter of this page.
- See <https://fair-edna.github.io/download.html> for the FAIRe checklist and more information.
- See <https://fair-edna.github.io/guidelines.html#missing-values> for guidelines on missing values that can be used for missing FAIRe or MIOP terms.

### Authors

- All authors known to have contributed to the preparation of this protocol, including those who filled in the template.
- Visit https://orcid.org/ to register for an ORCID.
- Date is the date the author first worked on the protocol.

| PREPARED BY  | AFFILIATION  | ORCID        | DATE       |
| ------------ | ------------ | ------------ | ---------- |
| Jacoby Baker | MBARI | 0000-0002-0673-7535 | 2023-11-07 |
| N. Kobun Truelove | MBARI | 0000-0002-2236-1849 | 2023-11-07 |
| Kathleen J. Pitz | MBARI | 0000-0002-4931-8592 | 2023-11-07 |

### Related Protocols

- This section contains protocols that should be known to users of this protocol.
- Include the link to each protocol.
- Include the version number and release date (if available).
- Internal/External: "Internal" are derivative or altered protocols, or other protocols in this workflow. "External" are protcols from manufacturers or other groups.

| PROTOCOL NAME | LINK         | VERSION      | RELEASE DATE | INTERNAL/EXTERNAL |
| ------------- | ------------ | ------------ | ------------ | ----------------- |
| 18S V9 PCR V.2  | dx.doi.org/10.17504/protocols.io.36wgq3d8olk5/v2 | 2 | 2023-09-26   | Internal      |
| NOAA/AOML PCR Protocol 18S rRNA V9 amaralzettler  | https://github.com/aomlomics/protocol-pcr-ssu18sv9-amaralzettler | 1 | 2024-08-22   | External      |

### Protocol Revision Record

- Version numbers start at 1.0.0 when the protocol is first completed and will increase when changes that impact the outcome of the procedure are made (patches: 1.0.1; minor changes: 1.1.0; major changes: 2.0.0).
- Release date is the date when a given protocol version was finalised.
- Description of revisions includes a brief description of what was changed relative to the previous version.

| VERSION | RELEASE DATE | DESCRIPTION OF REVISIONS |
| ------------- | ------------- | ------------- |
| 1.0.0 | yyyy-mm-dd | Initial release |

### Acronyms and Abbreviations

| ACRONYM / ABBREVIATION | DEFINITION |
| ------------- | ------------- |
| MBARI  | Monterey Bay Aquarium Research Institute  |
| NTC  | No template control  |
| PCR  | Polymerase chain reaction  |
| eDNA  | environmental DNA |
| EtOH  | Ethanol  |

### Glossary

| SPECIALISED TERM | DEFINITION |
| ------------- | ------------- |
| No Template Control  | A type of negative control during PCR to confirm there is no contamination during the PCR process. Normally nuclease-free water is run in place of DNA on a PCR.  |
| Content Cell  | Content Cell  |

## BACKGROUND

### Summary

This protocol is aimed at amplifying the 18S rRNA hypervariable region 9 (18S V9) in eukaryotes with a focus on microbial eukaryotes. Amplicons generated using this protocol can then be sequenced using the Illumina platform. The primers (1391F, EukBr) utilized in this protocol are based on the primer utilized in Amaral-Zettler et al. (2009), Stoek et al. (2010), and the Earth Microbiome Project (EMP).

This work was supported by NASA grant NNX14AP62A ‘National Marine Sanctuaries as Sentinel Sites for a Demonstration Marine Biodiversity Observation Network (MBON)’ funded under the National Ocean Partnership Program (NOPP RFP NOAA-NOS-IOOS-2014-2003803 in partnership between NOAA, BOEM, and NASA), and the U.S. Integrated Ocean Observing System (IOOS) Program Office.


### Method Description and Rationale

This method is applied because of its ability to amplify the target region (18S V9) across many different groups of organisms, the target region’s ability to discriminate between different taxa, and the common research application of this primer set allowing the data to be compared to a reference database and other published environmental datasets.

### Spatial Coverage and Environment(s) of Relevance

This protocol can be used to amplify the 18S rRNA marker gene region of any eDNA sample.

## PERSONNEL REQUIRED

One person with molecular biology experience.

### Safety

There are no hazardous chemicals or materials involved in this protocol. Standard lab safety techniques should still be used such as wearing PPE to avoid skin or eye contact.

### Training Requirements

Basic molecular biology training is sufficient for this protocol including sterile technique, pipetting small volumes and programming/running PCR thermal cyclers.

### Time Needed to Execute the Procedure

Protocol takes about 4 hours (240 minutes) including thermal cycler run time.

## EQUIPMENT

For 96-well Plate:

| DESCRIPTION | PRODUCT NAME AND MODEL | MANUFACTURER | QUANTITY | REMARK |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| **Durable equipment** |
| 100-1000 ul Pipette | Pipet-Lite™ XLS+ manual single-channel Adjustable-Volume Pipette | RAININ | 1 | Can be substituted with any accurate pipette |
| 10-100 ul Pipette | Pipet-Lite™ XLS+ manual single-channel Adjustable-Volume Pipette | RAININ | 1 | Can be substituted with any accurate pipette |
| 0.1-2.5 ul Pipette | Pipet-Lite™ XLS+ manual single-channel Adjustable-Volume Pipette | RAININ | 1 | Can be substituted with any accurate pipette |
| 10-100 ul 8-Channel Pipette | Pipet-Lite™ XLS+ manual 8 Channel Pipette | RAININ | 1 | Can be substituted with any accurate pipette |
| 0.5-10 uL 8-Channel Pipette |Pipet-Lite™ XLS+ manual 8 Channel Pipette | RAININ | 1 | Can be substituted with any accurate pipette |
| Thermal cycler | T100 Thermal Cycler | BIO-RAD | 1 | Can be substituted with generic |
| Gel Illuminator | PrepOne™ Sapphire Blue LED Illuminator with Photo Hood | Embi Tec | 1 | Can be substituted with generic |
| **Consumable equipment** |
| Gloves | Nitrile Gloves, Exam Grade, Powder-free | KimTech | 1 | (box) Can be substituted with generic |
| Kim Wipes | KimWipe Delicate Task Wipers | KimTech | 1 | (box) Can be substituted with generic |
| 96-well PCR Plate | SuperPlate PCR Plate, 96-well, semi-skirted AB2400 | Thermo Scientific | 1 | |
| PCR Plate Seal | PCR Plate Heat Seal, foil, peelable #1814045 | BIO-RAD | 1 | Can be substituted with generic, can use tightly-fitted strip caps in place of seal |
| 1000 µL Filter Tips | Pipette Tips RT LTS 1000µL | RAININ | 1 | (box) Can be substituted with generic |
| 200 µL Filter Tips | Pipette Tips RT LTS 200µL | RAININ | 2 | (boxes) Can be substituted with generic |
| 20 µL Filter tips | Pipette Tips RT LTS 20µL | RAININ | 2 | (boxes) Can be substituted with generic |
| AmpliTaq Gold PCR Mix | AmpliTaq Gold™ Fast PCR Master Mix 4390941 | Applied Biosystems | 3960 | (µL) for 96 samples plus a 10% volume buffer |
| Molecular water | DNase/RNase-Free Water | Zymo | 3009.6 | (µL) for 96 samples plus a 10% volume buffer |
| Forward Primer - 1391F | 18S 1391F Fluidigm Primer | IDT | 316.8 | (ul (10µM) for 96 samples plus a 10% volume buffer) Primer must be diluted from 100µM stocks to 5µM |
| Reverse Primer - EukBR | 18S EukBR Fluidigm Primer | IDT | 316.8 | (ul (10µM) for 96 samples plus a 10% volume buffer) Primer must be diluted from 100µM stocks to 5µM |
| TAE Buffer (10x) | Electrophoresis Grade TAE Buffer 10X Solution | Embi Tec | 100 | (uL) TAE buffer must be diluted from 10X to 1X concentration |
| Agarose gel 2% | 2% Agarose TAE w/ GelGreen Long Gel, 4(24+1) well | Embi Tec | 1 | Can be substituded with user cast gel |
| Gel stain loading dye | TriTrack DNA Loading Dye (6X) R1161 | Thermo Scientific | 96 | (ul per plate) |
| 100bp DNA Ladder | GeneRuler Ready-to-Use DNA Ladders | Thermo Scientific | 2 | (ul per lane on gel) |
| **Chemicals** |
| RNase AWAY | RNase AWAY Surface Decontaminant | ThermoFisher Scientific | 1 | (bottle) Used to sterilize lab surfaces and equipment |
| EtOH | Ethanol | Generic Brand | 1 | (wash bottle) Must be molecular grade ethanol |
| DI water | Deionized water | Generic | 900 | (mL) |
| **Clean-Up Protocol** |
| AMPure XP Beads | AMPure XP Bead-Based Reagent | Beckman Coulter | 1 | (kit) |
| 96-well magnetic plate | MagDTR 96-Well Magnetic Separator | Edge Biosystems Inc | 1 | Can be substituted with generic brand |
| **(OPTIONAL) Qubit** |
| Quant-iT Reagents | Quant-iT™ 1X dsDNA Assay Kits, high sensitivity (HS) Q33232 | Invitrogen | 1 | (kit) can be substituded with Qubit kit |
| Quant-iT plate reader plate | Corning™ 96-Well Solid Black Polystyrene Microplates | Corning | 1 | Can be substituted with Qubit kit and Qubit tubes |



## STANDARD OPERATING PROCEDURE

In the following SOP, please use the exact names of equipment as noted in the table above.

Provide a step-by-step description of the protocol. The identification of difficult steps in the protocol and the provision of recommendations for the execution of those steps are encouraged.

### Preparation

BEFORE STARTING
Disinfect work surfaces with 10% bleach, followed by 70% ethanol, then RNase Away and pipets with RNase Away. UV pipets, molecular grade water, and tube racks for 20 minutes prior to starting protocol.


### PCR

**Primers**: PCR primer sequences

| PCR Primer Name | Direction | Sequence (5’ -> 3’)| Sequence (5’ -> 3’) with Fluidigm Adapters | Fluidigm Adapter |
| ----- | ----- | ----- | ----- | ----- |
| Euk1391F | forward | **GTACACACCGCCCGTC** | ACACTGACGACATGGTTCTACA**GTACACACCGCCCGTC** | CS1 |
| EukBr | reverse | **TGATCCTTCTGCAGGTTCACCTAC** | TACGGTAGCAGAGACTTGGTCT**TGATCCTTCTGCAGGTTCACCTAC** | CS2 |


**Reaction Mixture**: PCR reagents, volumes, initial and final concentrations

| Reagent | Volume | Initial Concentration | final concentration|
| ----- | ----- | ----- | ----- |
| DNA extract template | 3 μl | content |content |
| Amplitaq Gold Fast PCR mastermix (Applied Biosystems) | 37.5 μl | content |content |
| forward primer | 3 μl | 5 μM |content |
| reverse primer | 3 μl | 5 μM |content |
| molecular-biology grade water | 28.5 μl | content |content |

**PCR Cycling Program**: 

| PCR Step | Temperature | Duration | Repetition |
| ----- | ----- | ----- | ----- |
| Intial Denaturation | 95° C | 10 minutes | 1 |
| Denaturation | 94° C | 45 seconds | 34x |
| Annealing | 57° C | 30 seconds | 34x |
| Extension | 68° C | 90 seconds | 34x |
| Final Extension | 72° C | 10 minutes | 1 |
| Hold | 4° C | ∞ |  |

1. PCR reactions were run in single 75ul reactions for each sample using 12-basepair Golay barcoded reverse primers (Amaral-Zettler et al. (2009), Stoek et al. (2010), Earth Microbiome Project) with Fluidigm adapters CS1 & CS2.

2. PCR reactions were run in 96-well plates with a NTC and positive control run in singleton for each plate. PCR cycling parameters use a normal ramp speed.


### Quality Control

3. After PCR amplification of the marker region, PCR products were run through an agarose gel to confirm the presence of target bands and absense of non-specific amplification across environmental samples as well as the absence of amplification in no-template controls (NTCs).



#### Positive Control

An internal positive control consisting of extracted DNA from a freshwater aquarium sample was run in singleton for each 96-well PCR plate.

#### Negative Control

A NTC consisting of nuclease-free water was run in singleton for each 96-well PCR plate.

### PCR Clean-up

4. PCR products were purified and size selected using the Agencourt AMPure XP bead system (Beckman Coulter, USA) with a bead concdntration of 1.2X. 
5. A second agarose gel was run to confirm primer removal and retention of target amplicons after purification. 
6. A subset of purified products were then quantified using Quant-It Picogreen dsDNA Assay (Life Technologies) on an fmax Molecular Devices Fluorometer with SoftMaxPro v1.3.1 

### Basic Troubleshooting Guide

- Identify known issues associated with the procedure, if any.
- Provide troubleshooting guidelines when available.

## REFERENCES

Amaral-Zettler LA, McCliment EA, Ducklow HW, Huse SM (2009) A Method for Studying Protistan Diversity Using Massively Parallel Sequencing of V9 Hypervariable Regions of Small-Subunit Ribosomal RNA Genes. PLOS ONE 4(7): e6372. https://doi.org/10.1371/journal.pone.0006372

Stoeck, T., Bass, D., Nebel, M., Christen, R., Jones, M. D. M., Breiner, H.-W., & Richards, T. A. (2010). Multiple marker parallel tag environmental DNA sequencing reveals a highly complex eukaryotic community in marine anoxic water. Molecular Ecology, 19 Suppl 1, 21–31. https://doi.org/10.1111/j.1365-294X.2009.04480.x

Caporaso, J. G., Lauber, C. L., Walters, W. A., Berg-Lyons, D., Huntley, J., Fierer, N., Owens, S. M., Betley, J., Fraser, L., Bauer, M., Gormley, N., Gilbert, J. A., Smith, G., & Knight, R. (2012). Ultra-high-throughput microbial community analysis on the Illumina HiSeq and MiSeq platforms. ISME J 6, 1621–1624. http://doi.org/10.1038/ismej.2012.8

## APPENDIX A: DATASHEETS

Link templates (e.g. preformatted spreadsheets) used to record measurements and report on the quality of the data as well as any documents such as manufacturer specifications, images, etc that support this protocol. Please include a short note describing the document's relevance.
