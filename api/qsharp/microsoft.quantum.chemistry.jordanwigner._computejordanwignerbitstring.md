---
uid: Microsoft.Quantum.Chemistry.JordanWigner._ComputeJordanWignerBitString
title: _ComputeJordanWignerBitString function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Chemistry.JordanWigner
qsharp.name: _ComputeJordanWignerBitString
qsharp.summary: >-
  Computes Z component of Jordan–Wigner string between
  fermion indices in a fermionic operator with an even
  number of creation / annihilation operators.
---

# _ComputeJordanWignerBitString function

Namespace: [Microsoft.Quantum.Chemistry.JordanWigner](xref:Microsoft.Quantum.Chemistry.JordanWigner)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Computes Z component of Jordan–Wigner string betweenfermion indices in a fermionic operator with an evennumber of creation / annihilation operators.

```qsharp
function _ComputeJordanWignerBitString (nFermions : Int, idxFermions : Int[]) : Bool[]
```


## Input

### nFermions : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The Number of fermions in the system.


### idxFermions : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

fermionic operator indices.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)[]

Bitstring `Bool[]` that is `true` where a `PauliZ` should be applied.

## Example

let bitString = _ComputeJordanWignerBitString(6, [0,1,2,6]) ;// bitString is [false, false, false ,true, true, true, false].