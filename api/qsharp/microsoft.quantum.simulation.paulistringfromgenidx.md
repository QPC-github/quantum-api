---
uid: Microsoft.Quantum.Simulation.PauliStringFromGenIdx
title: PauliStringFromGenIdx function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Simulation
qsharp.name: PauliStringFromGenIdx
qsharp.summary: >-
  Extracts the Pauli string and its qubit indices of a Pauli term described
  by a `GeneratorIndex`.
---

# PauliStringFromGenIdx function

Namespace: [Microsoft.Quantum.Simulation](xref:Microsoft.Quantum.Simulation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Extracts the Pauli string and its qubit indices of a Pauli term describedby a `GeneratorIndex`.

```qsharp
function PauliStringFromGenIdx (generatorIndex : Microsoft.Quantum.Simulation.GeneratorIndex) : (Pauli[], Int[])
```


## Input

### generatorIndex : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

`GeneratorIndex` type that encodes a Pauli term.



## Output : ([Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)[],[Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[])

The Pauli string of the term described by a `GeneratorIndex`, andindices to the qubits it acts on.