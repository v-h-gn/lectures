---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# Molecular Computing Microtalk
#### Vahagn Tovmasian, October 24 2025

---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Computational Energy Consumption

- Greenhouse gas emissions are the primary driver of global warming and climate change. 

- Datacenters are using more energy to support increasing HPC demands.

- PROBLEM: How to use less energy and still meet compute demands?

- IDEA: Do whatever nature is doing.

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# The Brain As the World's Most Energy Efficient Computer

- 100 billion neurons, 400 kcal a day energy expenditure.
- One med length GPT-5 query can use up to 40 Watt-hours [1], which is 34.4168 kcal.
- A bit under 9% of your brain's energy daily energy usage.

- But even so, we can go smaller than the neurons, on the individual operation of molecules.


<AdmonitionType title="Energy in terms of PhD Students" type="tip" width="300px" custom="text-lg" v-drag="[44,413,866,84]">
Assuming 2000 kcal a day and 10 MWh annual US household expenditure, it takes about 260 MWh to train a 24 year old PhD student. Compare that to 50 GWh for GPT-5. [2]
</AdmonitionType>


---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
image: adelman-figure.png
```
# Origins of Molecular Computing, Leonard Adelman

- Solution to directed Hamiltonian Path problem done entirely via DNA in solution
- Treat each node and edge as a separate DNA molecule. 
- Let $v_in$ be our entry node and $v_out our exit node in $G = (V,E)$
  - Generate random paths 
  - Keep only paths that begin and end at $v_in$ and $v_out$
  - Keep only paths that visit exactly |V| vertices
  - Keep only paths which only enter each vertex once.
  - If any paths remain return YES, else return NO.
---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# 
- Individual molecules can be leveraged to perform highly parallel, low energy cost computation
- 

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```


---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?



