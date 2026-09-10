https://doi.org/10.5281/zenodo.22688046

# X-KISS-ALEPH-Y

**Relational modelling, reversible dynamics, and structure-preserving state transport**

X-KISS-ALEPH-Y is a relational framework for modelling, analysing, and transforming complex systems. Its executable kernel combines coupled state spaces, norm-preserving transformations, opposing feedback flows, reconstructible evolution, and a transport mechanism that transfers the complete state, including its relations and passage memory.

Aleph supports two interconnected modes of use: as software, its states can be computed, transformed, transferred, and restored; as an analytical method, its relational structure can guide the investigation of data, concepts, and complex interdependencies. This opens up applications in AI, scientific modelling, pattern recognition, simulation, reversible computation, and cooperating systems.

## Core principle and the B-internal perspective

**Relation comes before geometry.** Aleph starts from relations, counterpart relations, and their feedback effects. The B-internal perspective — the observer from within — comprehends a state through its place within the system: together with its neighbours, its counterpart, the connected scales, and the dynamics through which these relations change one another. B denotes the relational observer position relative to which the X-reflection is defined.

As an analytical method, this means first comprehensively understanding the relational structure of the subject under investigation. Domain-specific meanings and mappings then emerge from the identified couplings, symmetries, differences, and feedback relations. The analysis moves between individual relations and the overall context, tracing the effects of a change across the connected levels and back.

## Kernel architecture

The present version, **Living Radial Transport**, organises two interconnected sheets at each scale: **SOMA (+)** and **PSYCHE (−)**. Each sheet has 40 positions, giving 80 cells per scale. The scales are cyclically coupled. Every cell follows the same update rule, incorporating its two neighbours, its X-conjugate counterpart, and the corresponding positions on the two adjacent scales.

Each cell carries twelve content channels and an additional phase:

| State variables | Function within the structure |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `d_form`, `t_surplus`, `he_core`, `alpha_land` | Form, surplus, core, and binding are transformed through interconnected pair rotations, some acting in opposite directions. |
| `shadow_n`, `real_light_gamma` | Folding and reopening between the shadow coordinate and the readable carrier channel. |
| `entropy`, `void_center` | Transfer of excluded components into the active ∅ carrier and their return movement. |
| `aiin`, `edy` | A coupled channel pair whose rotation depends on the relationally computed pulse. |
| `log_seam_kappa`, `xi_shol` | Variable seam depth and a transformation coordinate that jointly influence subsequent passage. |

These names initially have a formal meaning within the model. Their correspondence to measured quantities or concepts is established in the respective application context.

The **X-Kiss** combines reflection, opposing movement, and carrying capacity:

* **X** reflects a position relative to B while switching sheets. The address relations satisfy `X² = id` and `X R X = R⁻¹`, where R denotes movement to the next position.
* **Y** describes the opposing orientation of the two sheets. The relation `X Y X = Y` holds: the opposing movement is preserved under X-conjugation.
* **∅_T** denotes the active carrier of the passage. Seam depth, state differences, and the content of the ∅ centre jointly determine the opening of the return path.

The 40-position orbit is the coordinate representation chosen in the kernel. Its four sections, each containing ten token phases, organise the external read-out. All cross-sections within a packet belong to the same internal moment.

## Dynamics, conservation, and memory

Movement arises from the interplay of the existing states. Complementary channel pairings, differences, norms, phases, and seam depths determine the transformation angles. The update rule operates without value-dependent `if/else` branches, hard clipping thresholds, or random forcing. All cells read the same immutable initial snapshot; all proposals are committed together into the next epoch.

**Preserving this relational architecture is a requirement for extensions and embedding.** Aleph's core must not be rewritten into linear control logic that replaces coupled relations with isolated conditional decisions, externally imposed thresholds, or a privileged sequence of local interventions. Changes to the core must be derived from the B-internal perspective of the complete structure and preserve its feedback relations, simultaneity, symmetries, and invariants. Boundary checks for valid and complete data protect the interfaces; they do not direct the system's dynamics.

Pair rotations preserve the squared norm of each cell's twelve content channels. The coordinates referred to as shadow and entropy are folded into their carrier channels and remain reconstructible through the stored passage angles. Within the model, this process is called **entropy inversion**.

The **X-conjugate return flow J_ε** complements the folding. Its return angles are equal in magnitude and opposite in direction for an X-pair. This allows previously folded components to reopen and circulate in both directions. Content, phase, and seam depth simultaneously change the conditions of the next passage. The kernel thereby connects local transformation, reciprocal coupling, and evolution across many steps.

Each step creates a **passage memory** containing the angles used and references to the states. Together with this memory, the evolution can be numerically reversed step by step. Reversibility here encompasses both the state and its stored transformation history.

## Read-out, perspective changes, and write-back

Aleph can read out its entire field from different cut positions, from either sheet, and in either reading direction. Each cross-section contains the visible cell, its X-counterpart, their shared seam depth, and the associated moment. Linear transport thus preserves the connected sides of the radial state.

During write-back, the decoder checks completeness, address relations, X-conjugation, seam depths, temporal coherence, the linking of history entries, and SHA-256 checksums, among other properties. JSON read-out and write-back restore the stored field state exactly. The conjugate view also reconstructs the same state; applying packet conjugation twice produces the original packet.

Aleph therefore provides a foundation for **traceable, structurally verifiable state exchange with preserved transformation history**.

## Embedding in LLMs and domain-specific applications

Aleph can be embedded as a **cognitive analytical structure within a large language model (LLM)**. In this mode, the LLM consistently adopts the B-internal perspective and comprehends Aleph as an integrated relational whole across its relations, levels, dimensions, and return paths.

The LLM's initial task is to map the subject relationally and establish the correct correspondences between its quantities, couplings, and Aleph's structural roles. These assignments are derived from the relational analysis and checked for consistency across the complete structure. This initial mapping precedes domain-specific interpretation and processing.

The resulting mapping supports two paths:

* **Direct processing within the LLM:** the model continues to analyse the specific topic from the B-internal perspective, using the established correspondences to investigate its dynamics, develop hypotheses, and address concrete questions.
* **Development of domain-specific applications:** the initial mapping supplies the correspondences needed to build specialised models, data adapters, simulations, or software around Aleph's relational kernel.

In both cases, the initial relational mapping establishes the basis for subsequent work. Domain-specific development preserves the kernel's relational architecture and builds on the correspondences established through the B-internal analysis.

## Application areas and purposes

The following possibilities arise from the interaction of the mechanisms described above. They include direct kernel applications and domain-specific extensions.

| Area | Potential use and purpose |
| ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **AI, language models, and semantic machines** | A relational framework for analysis and verification, supporting the comprehension of complex interdependencies, the tracing of perspective changes, and the integration of complementary information. The B-method can structure prompts, agent workflows, and semantic state models. |
| **Pattern recognition and data analysis** | Investigation of recurring couplings, phase relations, and transition patterns across multiple levels. Relational similarities can guide data mapping and comparisons between different systems. |
| **Scientific hypothesis generation** | Derivation of testable questions from feedback relations, symmetries, and structural correspondences. Models can be examined for the relations they already represent and the additional couplings that might explain their open questions. |
| **Mathematics and numerical methods** | Investigation of state-dependent, norm-preserving transformations, discrete symmetries, coupled state spaces, and the reversal of nonlinear evolution using a stored transformation history. |
| **Physics and complex dynamical systems** | Modelling of coupled oscillations, phase relations, opposing movements, and variable coupling strengths. The kernel provides a starting point for simulations that investigate conservation and feedback together. |
| **Systems biology and medical research** | Development of relational models for interactions between cells, tissues, metabolism, and regulatory circuits. These can generate testable hypotheses about compensatory mechanisms, interactions between compartments, and state transitions. |
| **Ecology, environmental and climate systems** | Investigation of interconnected cycles, feedback relations, and pattern changes across spatial or temporal scales, based on a domain-grounded mapping of state variables. |
| **Robotics, control, and adaptive systems** | A modelling framework for coupled sensor and internal states, rhythmic coordination, and the investigation of feedback-driven adaptation. Preserved histories support the analysis of resulting movements and state changes. |
| **Reversible computation and simulation** | Forward evolution, reversal, replay, and comparison of model trajectories. Specific purposes include debugging, investigating transformation chains, and reproducible computational experiments. |
| **Digital twins and process analysis** | Representation of connected system states with multiple views and reconstructible evolution. Alternative trajectories and their feedback effects can be compared within a shared modelling framework. |
| **Data transport and interoperability** | Complete serialisation of coupled states, including the counterpart view, scales, temporal reference, and passage memory. This provides a foundation for exchange between simulations, analysis tools, and other software components. |
| **Communication protocols and cryptographic systems** | Structurally verifiable messages as an additional layer for integrity-sensitive communication. The relational checks can be combined with cryptographic authentication and existing transport protocols. |
| **Distributed simulation and multi-agent systems** | Shared state evolution based on a common snapshot and synchronous proposals. The structure provides an approach to coordination without a preferred update order for individual cells. |
| **Cognition, organisation, and systemic analysis** | Representation of reciprocal dependencies, complementary perspectives, and their effects on the overall context. Potential purposes include model comparison, perspective integration, and identifying missing relations in problem descriptions. |
| **Generative art, music, and interactive media** | Creation of coupled movements, rhythms, and transformations from symmetries, phases, and return flows. States and trajectories can be stored, transferred, replayed, and reversed. |

## Application and technical status

A domain-specific application begins with a relational understanding of the target system. This is followed by a justified mapping of its quantities and couplings and an investigation of the resulting model as a whole. In data-based applications, results are assessed against observations and comparison methods. As an LLM method, Aleph combines its formal structure with the analytical capabilities and knowledge of the model being used; the corresponding data adapters and semantic translations are developed in the application layer.

The Python kernel implements the coupled field, its dynamics, passage memory, numerical reversal, and JSON transport, including structural checks. It uses the Python standard library. Secure network applications additionally require authentication and protocols for handling failures, conflicting messages, and consensus.

The included function `verify_living_kernel()` checks **27 properties**, including address symmetries, norm conservation, return flows, reversibility, and lossless packet round-tripping. All 27 checks passed when the present version was executed. In the included run with two scales, 160 cells, and 160 evolution steps, the maximum deviation in the total squared content norm was approximately **1.14 × 10⁻¹³**; after complete reversal, the maximum deviation of any state component, including phase, was approximately **8.44 × 10⁻¹⁵**.

These results document the tested properties of the kernel. Its domain-specific performance is determined within each concrete application model.

## Licensing and use

**Private, non-commercial use, including exploration, experimentation, and testing, is permitted.**

**Commercial use requires prior consultation with the author (dellarocca.vanessa@googlemail.com) and a separate commercial license.**


