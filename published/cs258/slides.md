---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
presenter: true
---

# MolGym: A Gymnasium Compatible Environment Suite for applying RL to biochemical applications.
## 12/06/2025 

---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Motivation

There are lots of relevant problems in biochemistry which can be represented as Markov Decision Process (MDPs).

We'll focus on **retrosynthesis** and **antimicrobial peptide design.**

<img src = "https://alevelchemistry.co.uk/wp-content/uploads/2018/11/organic-synthesis-3.jpg" v-drag>

---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::

# Retrosynthesis

Problem: Find the best sequence of reactions to generate a target molecule.

Very important in industrial scale chemistry => even well known reactions are not necessarily optimal w.r.t the cost of raw ingredients

Furthermore, certain synthesis pathways have increased harm to the environment via byproducts.

Ex. Hydrogen gas can be generated with electricity + H2O, more commonly generated heating methane and water together, producing CO2


::right::

# MDP Formulation

## States
Target molecule, usually given as a SMILES string Ex. `C([C@@H]1[C@H]([C@@H]([C@H]([C@H](O1)O)O)O)O)O`

## Actions
The set of all reactions which contain the target molecule as a product

## Rewards
User defined weighted combination of the cost of the reaction (buying chemicals), time, complexity, negative weighting of undesired byproducts

## Transition Model
$P(s_{t+1} | s_t, a_t) = 1$, i.e, there is little stochasticity involved.


---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::

# Antimicrobial Peptide Design

Problem: Using antibiotics develops antibiotic resistance, how to design newer and more effective antibiotics?

One candidate is using **anti-microbial peptides** (AMPs). 

Peptides can be neatly represented as strings with an alphabet, and then defined as a probablistic context free grammar.

The problem then becomes a search across the PCFG space for a candidate with the highest proposed antimicrobial potency.

::right::

# MDP Formulation

## States
The set of all valid sentences defined by our AMP PCFG

## Actions
The set of all valid words which can be arranged in our sentence

## Rewards
Weighted combination of structural similarity (AlphaFold), genomic similarity (PDB, GenBank, etc), and environmental impacts (toxicity, synthesizability, etc)

## Transition Model
Probabilities of a particular word being in the sentence as defined by our PCFG.


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# AMP PCFG Environment Episode Example

User passes in a defined structure for a sentence (a target protein) 

`<VARIABLE_START> <KNOWN_CHAIN>`

Agent then uses PCFG grammar rules to perform an action, which results in.

```
"""
S -> VARIABLE_START KNOWN_CHAIN [1.0]
KNOWN_CHAIN -> 'ACIAGERRYGTCIYQGRLWAFCC' [1.0]
VARIABLE_START -> 'A' VARIABLE_MID [0.5] | 'G' VARIABLE_MID [0.5]
VARIABLE_MID -> 'C' VARIABLE_END [0.5] | 'D' VARIABLE_END [0.5]
VARIABLE_END -> 'E' [1.0]
"""
```

`<VARIABLE_START> ACIAGERRYGTCIYQGRLWAFCC`

Agent keeps performing actions until an episode end is reached, giving a candidate as well as a reward

```
G <VARIABLE_MID> ACIAGERRYGTCIYQGRLWAFCC
G C <VARIABLE_END> ACIAGERRYGTCIYQGRLWAFCC
G C E ACIAGERRYGTCIYQGRLWAFCC
Total reward: 0.8113705638880109
Final sentence: GCEACIAGERRYGTCIYQGRLWAFCC
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Evaluation

- Scale of problems beyond timeline for class (existing works report taking millions of CPU hours to train decent results)

- Use smaller constrained scenarios to test the environment for class, eventually test actual stuff

- Retrosynthesis: Hemoglobin Synthesis

- Generating defensin analogues. (type of antibiotic protein humans produce)


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Code/API

- All environments follow Gymnasium API, will be backwards compatible with Gym

- AMP generation leverages NLTK and user defined grammar -> eventually grammar will be automatically generated based on database.

- Environments internally decide whether to use GPU or CPU based on available hardware



---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Future Work

## Now Until Deadline
1. Get dssp (secondary structure annotation) for generating grammar as internal software only works on Linux, 
2. Actually train a model.

## Beyond This Class
1. HPC optimizations
2. Database integration 
3. Set up GCP and spend UCR's money.