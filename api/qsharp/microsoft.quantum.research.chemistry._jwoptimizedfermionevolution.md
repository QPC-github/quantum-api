---
uid: Microsoft.Quantum.Research.Chemistry._JWOptimizedFermionEvolution
title: _JWOptimizedFermionEvolution operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Research.Chemistry
qsharp.name: _JWOptimizedFermionEvolution
qsharp.summary: >-
  Represents a dynamical generator as a set of simulatable gates and an
  expansion in the JWOptimized basis.

  See [Dynamical Generator Modeling](xref:microsoft.quantum.libraries.overview.data-structures#dynamical-generator-modeling)
  for more details.
---

# _JWOptimizedFermionEvolution operation

Namespace: [Microsoft.Quantum.Research.Chemistry](xref:Microsoft.Quantum.Research.Chemistry)

Package: [Microsoft.Quantum.Research.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Research.Chemistry)


Represents a dynamical generator as a set of simulatable gates and anexpansion in the JWOptimized basis.See [Dynamical Generator Modeling](xref:microsoft.quantum.libraries.overview.data-structures#dynamical-generator-modeling)for more details.

```qsharp
operation _JWOptimizedFermionEvolution (generatorIndex : Microsoft.Quantum.Simulation.GeneratorIndex, stepSize : Double, parityQubit : Qubit, qubits : Qubit[]) : Unit is Adj + Ctl
```


## Input

### generatorIndex : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

A generator index to be represented as unitary evolution in the JWOptimizedbasis.


### stepSize : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

A multiplier on the duration of time-evolution by the term referencedin `generatorIndex`.


### parityQubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit that determines the sign of time-evolution.


### qubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Register acted upon by time-evolution operator.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

