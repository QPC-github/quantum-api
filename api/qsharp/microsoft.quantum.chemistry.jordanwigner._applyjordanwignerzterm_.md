---
uid: Microsoft.Quantum.Chemistry.JordanWigner._ApplyJordanWignerZTerm_
title: _ApplyJordanWignerZTerm_ operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Chemistry.JordanWigner
qsharp.name: _ApplyJordanWignerZTerm_
qsharp.summary: Applies time-evolution by a Z term described by a `GeneratorIndex`.
---

# _ApplyJordanWignerZTerm_ operation

Namespace: [Microsoft.Quantum.Chemistry.JordanWigner](xref:Microsoft.Quantum.Chemistry.JordanWigner)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Applies time-evolution by a Z term described by a `GeneratorIndex`.

```qsharp
operation _ApplyJordanWignerZTerm_ (term : Microsoft.Quantum.Simulation.GeneratorIndex, stepSize : Double, qubits : Qubit[]) : Unit is Adj + Ctl
```


## Input

### term : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

`GeneratorIndex` representing a Z term.


### stepSize : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Duration of time-evolution.


### qubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Qubits of Hamiltonian.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

