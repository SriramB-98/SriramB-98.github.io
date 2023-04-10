---
layout: page
title: An exposition on quantum interactive proofs with a classical verifier
description: Course project
img: assets/img/quantum_pic.png
html: assets/pdf/quantum_project_report.pdf
importance: 2
category: work
---

<a href="/assets/pdf/quantum_project_report.pdf" class="btn btn-sm z-depth-1" role="button">Link to report</a>  

Quantum interactive proofs are the quantum analogue of interactive proofs, in which a
powerful but untrusted prover attempts to convince a less powerful verifier of the correctness
of its computation. In quantum interactive proofs, we consider the case when either (or both)
the prover and verifier have quantum capabilities. In practice, we are concerned with the case
where the prover is a realistic quantum computer (BQP machine) trying to efficiently convince a
classical verifier (a BPP machine), which corresponds to the question: Can quantum computers
(efficiently) convince a classical verifier that its computations are correct over a polynomial
number of interactions? Recently, this question was settled in the affirmative, with the
assumption that the BQP prover cannot efficiently solve the learning with errors problem (LWE).
In this expository paper, I go over some key results in this field of quantum interactive proofs,
with a special focus on the landmark paper by Urmila Mahadev.