.. _bpm_articles:

****************************
Bit Patterned Media Articles
****************************


Bit-Patterned Magnetic Recording: Theory, Media Fabrication, and Recording Performance
======================================================================================



Abstract
--------

Bit-patterned media (BPM) for magnetic recording provides a route to thermally
stable data recording at :math:`> 1 \, \frac{Tb}{in^{2}}`.
Instead of recording a bit on an ensemble of random grains, BPM comprises a
well-ordered array of lithographically patterned isolated magnetic islands,
each of which stores 1 bit.

Introduction
------------

To maintain adequate signal-to-noise ratio (SNR) to recover
recorded data with an acceptably low error rate, the grain sizes
within the magnetic film generally need to scale with the size
of the recorded bits. For a number of years, it was assumed
that the maximum achievable density for granular media would
be reached when scaling grains to smaller volume would
result in the loss of thermal stability. This understanding has
often been described as a trilemma, in which thermal stability,
media writeability, and media SNR drive mutually exclusive
objectives in media design. More recently, however, it
has become apparent that even before this long-predicted
trilemma is reached, scaling granular media properties to
achieve sufficient SNR to support an AD of $>1 Tb/in^{2}$ is
already very challenging

One concept that has been proposed to fundamentally address the shortcomings of conventional
media is bit-patterned magnetic recording (BPMR), which achieves
high SNR and thermal stability by replacing the random
grains of conventional media with lithographically patterned
magnetic islands, which are significantly larger than, and
thereby more thermally stable than, conventional media
grain.

.. figure:: _static/Img_bpm/Fig01.png
   :scale: 50 %
   :alt: granular media and BPM
   :align: center

   Comparison of a granular media (left) and BPM (right).

The grand challenge for BPMR, however, is the
high-volume low-cost manufacturing of BPM with good
magnetic properties and tight fabrication tolerances. What
makes this challenge particularly daunting is the small feature
size required—generally $<20 nm$ full pitch ($<10 nm$ feature
size) in the down-track direction, which is beyond the capa-
bilities of conventional lithographic methods as practiced by
the semiconductor industry.

BPM Data Storage Requirements
-----------------------------

On a very basic level, an HDD consists of a spinning data storage
medium (the disk), an element that reads and writes data to
the disk (the head), and a mechanical arm that moves the
head around the disk (the actuator).

### Sector Failures and Bit Error Rates

The data loss rate is usually specified as
an unrecoverable bit error rate (BER), which, for HDDs,
is typically stated as less than one error in $10^{14} – 10^{16}$ bits read
depending on the application. For the subsequent discussion,
we will assume that bits are grouped into 4 kB sectors on the
disk and that not recovering a single bit is equivalent to losing
the whole sector. We will use the midrange unrecoverable
sector failure rate (SFR) of $10^{-11}$ or one bad sector for every
400 TB written.

The read channel employs error correcting codes (ECCs) that can correct erroneous bits at
the expense of additional storage overhead.

Unrecoverable sector failures stem from four main sources:

1. mis-synchronization  
2. adjacent track erasure  
3. defects  
4. thermally activated reversal.  

### BPM Recording Theory and Concepts

*Effective Bit Position Jitter and Bit Error Rates*


*Thermal Stability*

The thermally activated reversal rate depends on the bit volume $V$, the anisotropy energy density
$K_{U}$, Boltzmann’s constant $k_{B}$ , and the drive temperature $T$. The typical way to estimate
the rate is to use the Arrhenius switching model in which the reversal rate is given by $R = f_{0} \exp(-K_{U} V /k_{B} T)$.
Using the BER criteria of $10^{-2}$, in a SFR of $<10^{-11}$ will be
maintained after 10 years if the $K_{U} V /k_{B} T > 52$. However, a population of islands will have
a distribution of volumes and anisotropy. The thermally activated reversal rate is accelerated by
adjacent track writing due to the presence of the residual write fields on the adjacent track.
Residual write fields are temporary but will accumulate near tracks that are written frequently.
Dipolar fields can also accelerate thermal decay, especially for islands in the areas of
uniform magnetization.

*Data Track Writing Architecture*

Data can be written to the disk by

1. Centered track recording  
    In centered track recording, the write head writes a single track in a single pass, without
    overwriting the adjacent tracks. Centered track recording requires a match between the physical
    dimensions of the writer and the TP.

2. Shingled magnetic recording  
    In SMR, the writer spans several tracks and each track is written sequentially like overlapping
    shingles.

3. Hypertrack recording  
    In HTMR, two tracks are written simultaneously using a writer than spans two tracks.

*BAR considerations*

---

## Magnetic Material for BPM

### Prepatterned Substrates Versus Etching Continuous Films

The initial approach for BPM fabrication was to prepattern the substrate with pillar features, upon
which magnetic films with perpendicular anisotropy were deposited.

As lithographic and patterning techniques improved, the
order of fabrication steps was reversed and a continuous film
of magnetic material was deposited prior to the patterning
steps. This greatly expanded the variety of magnetic materials
that could be used.

Regardless of which fabrication strategy is pursued, it is
essential to include a continuous (not patterned) soft magnetic
underlayer below the magnetic seed layer structure in order to
close the magnetic flux from the write head and to keep the
magnetic flux lines at the recording point more perpendicular
to the layer structure in a manner similar to conventional
perpendicular recording.

### Magnetic Properties and Switching Field Distribution

To create etched BPM, the initial films must be continuous,
uniform, and smooth in order to be patterned into highly
uniform magnetic islands.

In practice, there can be significant
differences in physical structure and materials properties from
island to island, which cause variations in the switching field
of the islands.

Two distinct components
contribute to the SFD. First, the iSFD, which is caused by
the variations in the materials properties and microstructure
(such as defects, grain boundaries, crystallite misorientation,
and also different degrees of island edge damage due to
patterning. Second, the dipolar contribution, which
is an additional broadening that originates from different dipolar fields at each island arising from the specific magnetic state
of nearby islands. In order to ensure that an island being
addressed by the writer properly reverses without disturbing
the state of its neighbors, it is important that the iSFD be kept
as small as possible.

In order to evaluate and compare the reversal properties
of different BPM systems, which can have different average
island coercivity (i.e., average island switching field), it is
useful to consider iSFD normalized to the coercivity,
i.e., $iSFD/H_{C}$, as a figure of merit.
With prepatterned substrates and
Co/Pt or Co/Pd multilayers, $SFD/H_{C}$ increases from a ~3%
for large micrometer-sized islands to 12%–18% for diameters
of 30 nm or less. This trend arises from the fact that as islands
become smaller, properties are averaged over less magnetic
material.
In order to lower $SFD/H_{C}$, alternative magnetic structures
were investigated, including exchange spring and exchange-
coupled composite magnetic multilayer systems. such heterogeneous magnetic structures decreased
$SFD/H_{C}$ from >11% to 7.5%.


### Magnetic Materials for High Areal Density

For ADs beyond $1.2 Td/in^{2}$, additional media layer improvements
were implemented to keep $iSFD/H_{C}$ below 10%.

$H_{C}$ decreases and iSFD
broadens with decreasing film thickness, leading to unaccept-
able $iSFD/H_{C}$ values of ~20% for 4 nm thick
layers. The thermal stability ratio decreases from 150 for 8 nm
media down to 50 at 4 nm. In order to compensate for the loss
in magnetic volume and the decrease of the perpendicular
anisotropy density with thinner recording layers, a natural
approach is to vary the alloy composition and, in particular,
employ alloys with higher Pt content and therefore higher
$K_{U}$. However, BPM made of such alloys usually exhibits
broader iSFD, which may be caused by an increase in stacking fault density and other defects in
high-Pt-content cobalt
alloys.

A magnetic stack combining a hard magnetic layer and a
softer magnetic layer that are strongly exchange coupled was
also evaluated.
In this composite system, the hard magnetic layer provides an
increase of the overall perpendicular anisotropy density, while
the softer magnetic layer keeps the effective iSFD value
low. A study of $H_{C}$ and iSFD as a function of
the thickness ratio of the hard and soft magnetic layers, where
the total magnetic layer thickness was kept constant,
showed a linear increase of $H_{C}$ with the thickness ratio.

### Magnetic Materials for Templated Growth

Templated growth (TG) provides an alternative means to
generate ultrahigh-density BPM. In TG BPM, nucleation sites
with the desired pattern are generated by nanolithographic
patterning. A sequence of underlayers, magnetic layers, and
overcoat layers are then deposited on the nucleation features.

The magnetic layers can consist of cosputtered magnetic alloy
and oxide segregants to obtain a periodic array of magnetic
islands in a matrix of oxides

In order for TG BPM to obtain the best recording media
properties, it is desirable to start with nucleation features
with consistent size, shape, and surface conformation.

![Templated Growth](Img/Fig02.png)
*(a) TEM cross section TG BPR media (b) Plan-view SEM image*

Rather than choosing to grow on an amorphous nucleation
feature, if a nucleation feature with a preferred crystallographic
orientation is used, better orientation of grains (with
correspondingly better structural and magnetic properties) can
be obtained.

Because TG BPM generally has a higher
fill factor than etched media, we find that eTG media can
have a higher coercivity and thermal stability factor. So far,
TG BPM has a wider SFD than conventional etched BPM,
possibly due to variations in the nucleation features that are
reflected in magnetic variations from island to island. As a
consequence, recording performance of TG BPR media is
not as good as etched media, and further optimization of
the nucleation features, growth conditions, layer structure, and
materials composition are needed in order to achieve the full
potential of eTG media.

![Hysteresis TG](Img/Fig03.png)
*Magnetic hysteresis loop of an epitaxial grown TG BPM with a density of $1 Td/in^2$*

TG BPM has the potential of reaching much higher AD
without facing the scaling challenges associated with etching.
Therefore, TG BPM is a promising candidate for ultrahigh
density bit-patterned recording media.

---

## Media Fabrication

Fabrication of BPM diverges significantly from nanofabri-
cation processes practiced by the semiconductor industry for
multiple reasons.
1) The sizes of BPM features (generally $<20 nm$ full pitch
in the down-track direction) are beyond the capability
of conventional lithographic methods.
2) BPM requires single-shot full-disk lithography to avoid
stitching errors.
3) BPM patterns are circular in nature and are highly
periodic.
4) Cost targets are much lower and total area to be
patterned is much larger than for semiconductors.
5) BPMR can tolerate a relatively high defect rate
($~10^{-3}$ defective islands).

![Fabrication](Img/Fig04.png)
*(a) Process flow for fabrication of the master template, working templates, and BPM disks. (b) Two-generation nanoimprint strategy for duplicating the pattern from a single master template via replicated working templates to a large number of disks*

![Pattern](Img/Fig05.png)
*(c) Complete master pattern is formed by intersecting (a) zoned radial line pattern and (b) circumferential track pattern.*

### Rotary-Stage e-Beam Litography

In order to be able to generate complicated patterns, such
as bit patterns or HDD servo areas, a rotary EBL tool incor-
porates a formatting unit. The formatter generates deflection
and blanking signals for the beam within each written band.
The parameter data for each sector in a band are sent to the
formatter in real time, and therefore there is no need to store
massive amounts of pattern data as it would be the case for
an X–Y EBL system.

### Directed Self-Assembly of Block Copolymers

1. Introduction to Self-Assembly for BPM:
    Because sub-10 nm lithography  
is not available by any conventional lithographic technique,
BCP lithography has evolved as an organic part of the
BPM patterning solution not only because of the ability of
BCPs to form sublithographic features, but also because of
their flexibility to comply with other important BPM design
requirements such as conforming to zoned periodic features
on circular tracks at constant angular pitch.

2. Patterning With PS-PMMA From 41 to 22 nm Pitch:
    To do ...

3. Patterning Below 22 nm Pitch (BCP+SADP):  
    To do ...

4. Patterning Below 22 nm Pitch (Higher $chi$ BCPs):  
    To do ...

5. Design Requirements for Self-Assembled Patterns:  
    To do ...
    - Pitch flexibility
    - Defect density
    - Skew angle
    - Compatibility with servo patterns
    - Line roughness
    - Pattern Transfer of BCP DSA Patterns

### Self-Aligned Double Patterning (SADP)

SADP is a technique used by the semiconductor industry
to double the density of an existing prepattern.

There are three major unique features in our SADP for BPM:
1. our prepattern is created using DSA of BCP.

2. SADP is performed on circumferential or radial line arrays instead of
straight lines.

3. SADP is used to pattern a nanoimprint template instead of active devices.

![SADP](Img/Fig06.png)
*Line doubling process flow with DSA. (a) DSA BCP lines. (b) Etched carbon lines with line width control. (c) Conformal spacer deposition. (d) Anisotropic spacer etch back. (e) Mandrel removal. (f) Transfer into substrate.*

### Integration of Servo Patterns

When a disk drive reads or writes data on a recording
medium (including BPM), it needs position information in
both the disk radial and circumferential directions. This is
provided by servo patterns on the disk.
Servo patterns consist of several
magnetic sequences, including track number, sector number,
and subtrack position reference pattern (usually called a burst
pattern).
BPM offers the possibility of eliminating conventional
servowriting by creating physical servo patterns of magnetic
islands along with data islands. One way to accomplish this
is to fabricate a master template that contains both servo and
data patterns, and imprint this on each disk.

![Servo/data-integration process](Img/Fig07.png)
*Servo/data-integration process. (a) Circumferential submaster after
protective layer $1$ deposition. (b) Data area protected with photoresist.
(c) Servo patterns exposed using wet etch. (d) Alumina deposition by ALD.
(e) Alumina etched to produce tone-reversed servo pattern. (f) Servo pattern
etched into silicon. (g) Deposition of protective layer $2$. (h) Data area
DSA guiding patterns retrieved by liftoff and wet etch.*

### Pattern Transfer in Fabrication of Imprint Templates

High-volume manufacturing of BPM via nanoimprint
lithography requires robust master or submaster templates that
can be used thousands of times without degradation while
withstanding occasional cleaning to remove built-up organic
residues or contaminants. One route to achieving this is to
transfer patterns directly into the substrate onto which the
patterns are primarily formed. This is, however, a formidable
challenge at the dimensions required for BPM, especially in
the case of SADP.

Our nanoimprint template fabrication strategy has under-
gone two major transitions

1. hexagonal island arrays to rectangular, or high BAR arrays.

2. hole-tone to pillar tone.

After the fabrication of a BPM master template, it needs to
be replicated to multiple working templates for high-volume
manufacturing of disks using nanoimprinting. The template
replication is done by imprinting the master template pattern
into nanoimprint resist on working template substrates.

### Nanoimprint Litography

Nanoimprint lithography is the preferred technology for low-cost high-volume replication
of BPM patterns,
because of its extendibility to single-digit nanometer-scale
feature size and its ability to replicate full disk patterns without
stitching. Nanoimprinting was first developed specifically as a
solution for fabrication of BPM.

1. UV Cure Ink Jet Dispense Nanoimprinting Process:  
    
    ![UV-cure](Img/Fig08.png)
    *UV-cure nanoimprinting process steps. (a) Resist dispensing.
(b) Conformal contact of the disk and template, resist spreading, and
UV curing. (c) Separation of the disk and template.*

2. Normal Tone Versus Reverse Tone Imprinting:
    Nanoimprinting is similar to a molding process in that the topographic
pattern in the resist is a negative tone image of the template
pattern. To make use of the resist image for pattern transfer
to another layer (such as the magnetic layer of BPM), there
are two choices:
    - a normal tone process, in which the resist
itself is used as an etch mask and
    - a reverse tone process, in which depressions in the resist are backfilled with another
material that serves as the etch mask for pattern transfer
    ![NormalTone/ReverseTone](Img/Fig09.png)
    Although the terminology can be confusing, it is
important to note that normal tone produces a negative image
of the template features, and reverse tone produces a positive
image.

3. Defects in Nanoimprinting

    ![Typical defects](Img/Fig10.png)
    *Typical defects in nanoimprinting. (a) Nonfilled features in a
    $300 Gd/in^{2}$ pattern with a hole tone template. (b) Nonfilled features in
    a $300 Gd/in^{2}$ pattern with a pillar-tone template. (c) Fractured pillars.
    (d) Fractured pillars lodged in $300 Gd/in^{2}$ template holes. (e) Full disk view
    with a large centimeter-size tent defect caused by large airborne particle.
    (f) Tent defect with particle visible at center of tent.*

### Media Pattern Transfer

1. Media Etch Mask Preparation

2. Magnetic Dot Pattern Transfer by Etching

3. Vacuum Planarization

### Alternative Patterne Transfer: Templated Growth

### Alternative Patterne Transfer: Ion Implantation

---

## Recording System Integration

Many components work in tandem in the drive to store and
retrieve data with high fidelity. On the component side, there
are the read/write head and the media components. Closely
tied to these is the HDI. On the system side, there are the
servo/mechanical, read channel, write synchronization, front
end electronics subsystems, data architecture, and firmware.
The integration of all of these systems into a functioning
drive requires a careful awareness of the specifications of each
system and the interactions between the various systems in
order to arrive at a detailed balance that can meet customer
requirements

### Head-Disk Interface

Some of the tribological challenges expected to be aggravated by the rougher BPM surface include the following:

1. higher disk defect and asperity densities;  
2. poorer contact detection and clearance control for  recording heads flying over the disk surface;  
3. higher average flying heights and spacing modulations
of the recording head;  
4. poorer robustness of the BPM islands toward head-disk
contacts;  
5. increased tendency for corrosion.  

A potential way to solve the problems associated with
the patterned topography of BPM is to planarize the BPM
disk surface

The impacts and tribological challenges that using unplanarized and partially planarized BPM disks can have on the performance of the HDI can be 

1. Head-Media Spacing (HMS)
2. Contact Detection on BPM
    * Unplanarized media
    * Partially planarized media
3. Flying Height and Modulation of HMS

### Servo and Servo Patterns

1. Self-Registered Servo
2. Nonregistered Servo

### Write Synchronization

1. Zoning and Frequency RRO
2. Write Clock PLL

### Recording System Modeling

### Effect of Servo Fluctuations

---

## BPM Recording Experiments at $1.6 \frac{Td}{in^{2}}$

---

## Extendibility

### Extendibility Assesment Framework

### Island Tolerances and AD

### Thermal Stability and Writeability Limits


---

## Abbreviations

AD -> areal density  

AE -> acoustic emission 

ALD -> atomic layer deposition  

BCP -> block copolymer  
BAR -> bit aspect ratio  
BER -> bit error rate  
BPM -> bit-patterned media  
BPR -> ?  
BPMR -> bit-patterned magnetic recording  
DSA -> directed self-assembly  
EBL -> electron-beam lithography  
ECC -> error correcting code  
FM -> fill mask  
HAMR -> heat-assited magnetic recording  
HDD -> hard disk drive  
HDI -> head-disk interface  
HMS -> head-media spacing  
HTMR -> hypertrack magnetic recording (Two or more tracks are read/writen in one pass)   
ICP -> inductively  coupled plasma   
IBE -> ion beam etching 
LER -> line edge roughness  
MWW -> magnetic write width  
PES -> position error signal  
PLL -> phase looked loop  
PMR -> perpendicular magnetic recording  
ROO -> repetitive runout  
RIE -> reactive ion etching  
SADP -> self-aligned double patterning  
SFD -> switching field distribution  
iSFD -> intrinsec SFD  
SFR -> sector failure rate  
SMR -> shingled magnetic recording  
SNR -> signal-to-noise ratio  
TFC -> thermal flying height control 
TG -> templated growth  
eTG -> epitaxial TG  
TMR -> track misregistration  
TP -> track pitch (Separation between the centers of two adjacent tracks ~20nm)  
