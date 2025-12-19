# Higher Regularity for Quantum Graphs

This repository contains the computational framework supporting the article  
**“Higher Regularity for Quantum Graphs”**.

The code provides an explicit algebraic and numerical implementation of quantum graphs modeled via finite-dimensional C*-algebras, with a focus on higher-order regularity conditions, Schur idempotency, and spectral verification for both classical and genuinely quantum examples.

The implementation is designed to serve both as:
- a verification tool for structural properties appearing in the paper, and
- an exploratory environment for constructing and testing new quantum graph examples.

---

## Mathematical Scope

The framework is based on the viewpoint that a quantum graph is encoded by:
- a finite-dimensional C*-algebra  
  A ≅ ⊕ᵢ Mₙᵢ(ℂ),
- equipped with a distinguished state (trace),
- together with adjacency-type operators satisfying algebraic regularity conditions.

The code implements:
- Schur products and Schur idempotency,
- higher-order regularity constraints,
- spectral properties of quantum adjacency operators,
- examples arising from quantum strongly regular graphs, including cases with no classical analog.

---

## Repository Structure

The main content is provided as a research notebook:

Higher_regularity_for_quantum_graphs.ipynb

The notebook is structured as follows:

1. Definition of the Algebra Framework  
   - Algebra class implementing finite-dimensional C*-algebras  
   - Combinatorial utilities  
   - Definition of states (tracial functionals)

2. Verifiers  
   - Schur idempotency tests  
   - Higher regularity verifiers

3. Examples  
   - Explicit quantum graph constructions

4. Quantum Graph Constructions  
   - The 9-Paley quantum graph  
   - A quantum strongly regular graph with no classical counterpart  
   - The 16-Clebsch graph  
   - The Shrikhande graph

5. Higher Regularity Verification  
   - Systematic validation of higher-order conditions

6. Spectral Analysis  
   - Eigenvalue computations  
   - Spectral invariants

7. Self-Duality and Association Schemes  
   - Star–triangle (Reidemeister III) verifiers  
   - Kauffman exchange relations  
   - Association scheme data for quantum graphs (e.g. A₃, G₃)

---

## Key Features

- Explicit implementation of finite-dimensional C*-algebras
- Schur product and idempotency checks
- Automated verification of higher regularity conditions
- Spectral computation for quantum adjacency operators
- Construction and validation of:
  - Paley-type quantum graphs
  - Clebsch-type quantum graphs
  - Strongly regular quantum graphs without classical analogs
- Tools for exploring self-duality and association schemes

---

## Requirements

The code is written in Python and requires:

- Python ≥ 3.9
- NumPy
- SciPy
- Matplotlib

Recommended environment:

conda create -n quantum-graphs python=3.10 numpy scipy matplotlib  
conda activate quantum-graphs

---

## Usage

The primary entry point is the Jupyter notebook:

jupyter notebook Higher_regularity_for_quantum_graphs.ipynb

The notebook is designed to be read sequentially, as it mirrors the logical development of the constructions and verifications appearing in the article.

Individual sections can be executed independently for experimentation with specific quantum graph examples.

---

## Relation to the Article

This code accompanies the paper:

**Quantum graphs and spin models**

Specifically, the notebook:
- provides explicit realizations of the examples discussed in the paper,
- verifies higher regularity conditions appearing in the main results,
- supports claims regarding spectral properties and self-duality.

The code is not intended as a general-purpose library, but as a transparent and reproducible computational companion to the theoretical results.

---

## Limitations

- The implementation is restricted to finite-dimensional algebras.
- Optimization and large-scale performance were not priorities.
- The focus is on correctness and mathematical transparency rather than API stability.

---

## Citation

If you use this code in academic work, please cite the associated article.  
A BibTeX entry will be added upon publication.

---

## Authors

Roberto Hernández Palomares - University of Waterloo
Néstor Fabián Bravo Hernández - Centro de Investigación en Matemáticas (CIMAT)
Fabio Viales Solís - Universidad de Costa Rica (UCR)
---

