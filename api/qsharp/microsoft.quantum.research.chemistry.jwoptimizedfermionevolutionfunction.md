---
uid: Microsoft.Quantum.Research.Chemistry.JWOptimizedFermionEvolutionFunction
title: JWOptimizedFermionEvolutionFunction function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Research.Chemistry
qsharp.name: JWOptimizedFermionEvolutionFunction
qsharp.summary: >-
  Represents a dynamical generator as a set of simulatable gates and an
  expansion in the JWOptimized basis.
---

# JWOptimizedFermionEvolutionFunction function

Namespace: [Microsoft.Quantum.Research.Chemistry](xref:Microsoft.Quantum.Research.Chemistry)

Package: [Microsoft.Quantum.Research.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Research.Chemistry)


Represents a dynamical generator as a set of simulatable gates and anexpansion in the JWOptimized basis.

```qsharp
function JWOptimizedFermionEvolutionFunction (generatorIndex : Microsoft.Quantum.Simulation.GeneratorIndex, parityQubit : Qubit) : Microsoft.Quantum.Simulation.EvolutionUnitary
```


## Input

### generatorIndex : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

A generator index to be represented as unitary evolution in the JWOptimizedbasis.


### parityQubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit that determines the sign of time-evolution.



## Output : [EvolutionUnitary](xref:Microsoft.Quantum.Simulation.EvolutionUnitary)

An `EvolutionUnitary` representing time-evolution by the termreferenced in `generatorIndex.