---
uid: Microsoft.Quantum.Canon.ApplyFermionicSWAP
title: ApplyFermionicSWAP operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyFermionicSWAP
qsharp.summary: Applies the Fermionic SWAP.
---

# ApplyFermionicSWAP operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies the Fermionic SWAP.

```qsharp
operation ApplyFermionicSWAP (qubit1 : Qubit, qubit2 : Qubit) : Unit is Adj + Ctl
```


## Description

This essentially swaps the qubits while applying a global phase of -1if both qubits are 1s. Preserves anti-symmetrization of orbitals.See  for more information.This operation is represented by the unitary operator\begin{align}f_{swap} \mathrel{:=}\begin{bmatrix}1 & 0 & 0 & 0 \\\\0 & 0 & 1 & 0 \\\\0 & 1 & 0 & 0 \\\\0 & 0 & 0 & -1 \\\\\end{bmatrix}.\end{align}

## Input

### qubit1 : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

The first qubit to be swapped.


### qubit2 : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

The second qubit to be swapped.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## References

- [ *Ryan Babbush, Nathan Wiebe, Jarrod McClean, James McClain,  Hartmut Neven, Garnet Kin-Lic Chan*,  arXiv:1706.00023 ](https://arxiv.org/pdf/1706.00023.pdf)

## See Also

- [Microsoft.Quantum.Intrinsic.SWAP](xref:Microsoft.Quantum.Intrinsic.SWAP)