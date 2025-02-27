---
uid: Microsoft.Quantum.Synthesis.ApplyPermutationUsingDecomposition
title: ApplyPermutationUsingDecomposition operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Synthesis
qsharp.name: ApplyPermutationUsingDecomposition
qsharp.summary: >-
  Permutes the amplitudes in a quantum state given a permutation
  using decomposition-based synthesis.
---

# ApplyPermutationUsingDecomposition operation

Namespace: [Microsoft.Quantum.Synthesis](xref:Microsoft.Quantum.Synthesis)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Permutes the amplitudes in a quantum state given a permutationusing decomposition-based synthesis.

```qsharp
operation ApplyPermutationUsingDecomposition (perm : Int[], qubits : Microsoft.Quantum.Arithmetic.LittleEndian) : Unit is Adj + Ctl
```


## Description

This procedure implements the decomposition basedsynthesis approach.  The input is a permutation $\pi$ over $2^n$ elements$\{0, \dots, 2^n-1\}$, which represents an $n$-variable reversible Boolean function.The algorithm iteratively performs the following steps for each variableindex $i$:1. Compute $((\pi_l, \pi_r), \pi')$ such that the images   of $\pi_l$ and $\pi_r$ do not change bits in their elements at indexes other   than $i$ and images of $\pi'$ do not change bit $i$ in their elements.2. Set $\pi \leftarrow \pi'$, and derive truth tables from $\pi_l$ and $\pi_r$   based on elements that are not fixed-points.After applying these steps for all variable indexes, the remainingpermutation $\pi$ will be the identity, and based on the collected truthtables and indexes, one can apply truth-table controlled @"Microsoft.Quantum.Intrinsic.X"operations using the @"Microsoft.Quantum.Synthesis.ApplyXControlledOnTruthTable" operation.The variable order is $0, \dots, n - 1$.  A custom variable order can be specifiedin the operation @"Microsoft.Quantum.Synthesis.ApplyPermutationUsingDecompositionWithVariableOrder".

## Input

### perm : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

A permutation of $2^n$ elements starting from 0.


### qubits : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

A list of $n$ qubits to which the permutation is applied to.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

To synthesize a `SWAP` operation:```qsharpusing (qubits = Qubit[2]) {  ApplyPermutationUsingDecomposition([0, 2, 1, 3], LittleEndian(qubits));}```

## References

- [*Alexis De Vos*, *Yvan Van Rentergem*,  Adv. in Math. of Comm. 2(2), 2008, pp. 183--200](http://www.aimsciences.org/article/doi/10.3934/amc.2008.2.183)- [*Mathias Soeken*, *Laura Tague*, *Gerhard W. Dueck*, *Rolf Drechsler*,  Journal of Symbolic Computation 73 (2016), pp. 1--26](https://www.sciencedirect.com/science/article/pii/S0747717115000188?via%3Dihub)

## See Also

- [Microsoft.Quantum.Synthesis.ApplyPermutationUsingDecompositionWithVariableOrder](xref:Microsoft.Quantum.Synthesis.ApplyPermutationUsingDecompositionWithVariableOrder)
- [Microsoft.Quantum.Synthesis.ApplyPermutationUsingTransformation](xref:Microsoft.Quantum.Synthesis.ApplyPermutationUsingTransformation)