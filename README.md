<div align="center">

# Mechanosynthetic Build Sequences for Semiconductor Materials with Three Degree of Freedom Nanopositioners

Philip Turner

December 7, 2024

<i>Virginia Tech, NANO 3114</i>

</div>

## Abstract

Atomically precise manufacturing procedures were studied for various materials, with the restriction to 3DOF actuators. GFN2-xTB enabled vastly greater simulation speeds than previous studies, while retaining qualitative accuracy in properties besides energy. A large combinatorial space of tooltip types and product materials was explored. Build sequence design relied heavily on automated caching and retrieval of simulation results. While diamond could not be built, aromatic and amorphous carbon could. Silicon mechanosynthesis expanded on previous theoretical studies and established an alternative method of completing the silicon unit cell. Silicon carbide was found to be a more thermodynamically viable material, with similar affinity for 6-membered ring formation. Finally, a silicon carbide tooltip was designed which could perform assisted replication. The study garnered several insights into experimentally accessible methods for building atomically precise products.

## Introduction

The ultimate goal of manufacturing is to build products with atomic precision. As of 2024, the dominant technique for manufacturing small objects is photolithography. Large, intricate chips are manufactured with ~50 nm transistor size (some details within the transistor have ~10 nm resolution). Although marketed as exponentially decreasing with time ("3 nm" and "2 nm" nodes), transistor density is no longer scaling exponentially. For example, the transistor count in four generations of Apple M-series chips increased linearly with time. Moore's Law has ended and we are still nowhere near the atomic level.

Since the 1990s, scanning probe microscopes have repeatedly built atomic-scale structures out of inert feedstocks (Xe, CO, Cl<sup>-</sup>). Electronics have been manufactured by ripping individual hydrogen atoms off a Si(100) surface, then subjecting the atomically precise pattern to CVD precursor gasses[^1]. To date, no scanning probe has been reported to manufacture 3D structures with a repeating crystal unit cell. The lack of 3D structures stems from the limitations of "conventional mode" atom placement. The scanning probe nudges an atom along a metallic surface, then releases it at the intended destination. To build a 3D structure like a pyramid, the probe would detach the atom from the surface and move upwards in the Z direction. Two chemical reactions must occur reliably&mdash;the atom separates from the surface and binds to the probe, then it migrates from the probe to the build site.

Merkle and Freitas, with investment from Canadian Bank Note, developed an alternative called "inverted mode". Atomically precise nano-tips, about 30 atoms in size, are synthesized with organic chemistry[^2]. Each tip is already charged with a weakly bound feedstock, such as a hydrogen atom. It also contains three linkers that bind to a surface in a tripod configuration. The sample surface is covered with thousands or millions of these nano-tips. Next, a single nano-tip is used to build a single atom onto the scanning probe. Inverted mode simplifies the construction of 3D structures, as only a single chemical reaction is performed to translocate an atom in the Z direction. It also allows the use of reactive feedstocks such as free radicals, which are needed to form covalent bonds.

Before doing experimental research, Merkle and Freitas published a large volume of theoretical research on diamond mechanosynthesis. The largest project was the Minimal Toolset paper[^3]. It proposed 65 reaction sequences that could build both diamond unit cells and replicas of the tools that carried out the reactions. One problem encountered was the formation of 5-membered rings, which disrupt the diamond lattice structure. To circumvent 5-membered ring formation, some critical reactions relied on multiple nanopositioners and/or six degrees of freedom. Existing scanning probes only have a three degree-of-freedom (3DOF) actuator. This experimental limitation brings into question whether diamond can ever be built.

In addition to diamond, there was a body of theoretical literature on silicon mechanosynthesis. In 1997, Herman published a paper about the affinity of silicon for sp<sup>3</sup> orbital geometry, and a set of reactions that could build infinite silicon lattices[^4]. This research was promising, as the difficulty building diamond stemmed from carbon's preference for sp<sup>2</sup> geometry (e.g. graphite is more stable than diamond). In addition, the unique orbital preferences of silicon allowed the silicon diradical to break apart 5-membered rings. Subsequent papers disclosed reaction sequences that could build silicon unit cells in all crystallographic orientations, and both cubic and hexagonal packing. Nothing of the sort had been published for diamond mechanosynthesis. The content of the papers strongly supported Herman's claim that silicon was ideal for near-term mechanosynthesis with scanning probes.

A limitation of the silicon mechanosynthesis literature was the choice of feedstocks. For example, one feedstock was a bare silicon atom with four dangling bonds. Such a feedstock would likely form a covalent bond with the tooltip presenting it, reducing it to a three-fold radical. One objective of the current paper was adapting Herman's work to feedstocks readily available on tripod nano-tips. To expand the design space for tripods, the designs based on adamantane cages would be generalized to atranes[^5]. The end result would be a refined protocol for building silicon, and highly amenable to experimental validation with existing technology.

TODO: Materials and Methods + References in the next commit.