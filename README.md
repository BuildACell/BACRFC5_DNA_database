# BAC RFC #5 - Database of DNA Components
This distribution represents a draft of a DNA parts repository. We propose that the Build a Cell community shares DNA designs following this structure. 

This distribution was shared with the BAC community on 2023.11.14 (Austin, TX, USA) and is available under the MIT License (BAC Tools Group: 2023).

## Contents
This distribution is broken into five (5) categories: promoters, RBS sites, CDSes, terminators, and vectors.

### Level-matched T7 promoters
The level-matched T7 promoters are a set of 10 pT7 promoter variants, selected to allow for transcriptional control across two orders of magnitude, along the same lines as the Anderson Collection promoters for *E. coli*. The promoters are useful for implementing basic control in a synthetic cell, reducing the expression of toxic genes, and matching the stoichiometries of different proteins within multigene DNA constructs and synthetic cell modules.

Each promoter appears as a MoClo Level 0 ‘P’ part, while also driving expression of efasGFP for immediate use and measurement within PURE or cells containing the T7 RNA polymerase.

### RBSes
Also included are two 5’ untranslated regions, UTR1 and the reference RBS from Elowitz (1999). The UTR parts are designed as MoClo level 0 ‘U’ and ‘T’ modules, respectively.

UTR1 is based on the T7 *g10* leader sequence and results in highly efficient translation efficiency and consequent high expression levels in systems containing the *E. coli* ribosome. The Elowitz RBS is the reference RBS used to define RBS efficiency in Elowitz (1999) and by the iGEM community.

### CDSes
We've included two (2) types of coding sequence in this example distribution: fluorescent and colormetric **reporters**, and antibiotic **resistance markers**.

### Terminators
The T7 terminator tT7 is the consensus terminator derived from T7 *g1*, commonly used in protein production and recommended for use in the PURE system. T7hyb6 and T7hyb10 are efficient synthetic terminators developed by Calvopina-Chavez, *et al.* (2022) that have been shown to provide high termination efficiencies against T7 RNA polyermerase *in vivo* and *in vitro* as well as terminate transcription from the native *E. coli* RNA polymerase. The T7hyb6 terminator consists of a single termination domain while the more effective and longer T7hyb10 terminator consists of two termination domains linked by two pause sites.

### Vectors
The pOpen-MoClo-L1-1 vector is a modification of the FreeGenes pOpenv3 vector making it suitable as a MoClo level 1 destination plasmid. The vector contains an insert encoding J23103-UTR1-cjBlue, allowing for blue-white selection of correct assemblies.

## How do I use this distribution?
T7 promoters are included on plasmids (AmpR) with intact transcriptional units expressing a green fluorescent reporter. In other words, you can drop these plasmids directly into a T7 expression system (e.g., *in vitro* in PURE, *in vivo* in BL21(DE3) *E. coli* strains) and observe green fluorescence (ex: ~ 485 nm / em: ~ 520 nm).

MoClo parts follow the MoClo assembly standard (see Ref1 for details).

## References
1. MoClo Paper - https://doi.org/10.1371/journal.pone.0016765
