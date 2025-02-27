---
uid: Microsoft.Quantum.Diagnostics.AllowAtMostNQubits
title: AllowAtMostNQubits operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: AllowAtMostNQubits
qsharp.summary: >-
  Between a call to this operation and its adjoint, asserts that
  at most a given number of additional qubits are allocated with
  using statements.
---

# AllowAtMostNQubits operation

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Between a call to this operation and its adjoint, asserts thatat most a given number of additional qubits are allocated withusing statements.

```qsharp
operation AllowAtMostNQubits (nQubits : Int, message : String) : Unit is Adj
```


## Input

### nQubits : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The maximum number of qubits that may be allocated.


### message : [String](xref:microsoft.quantum.qsharp.valueliterals#string-literals)

A message to be displayed upon failure.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

The following snippet will fail when executed on machines whichsupport this diagnostic:```qsharpwithin {    AllowAtMostNQubits(3, "Too many qubits allocated.");} apply {    // Fails since this allocates four qubits.    using (register = Qubit[4]) {    }}```

## Remarks

This operation may be replaced by a no-op on targets which do notsupport it.