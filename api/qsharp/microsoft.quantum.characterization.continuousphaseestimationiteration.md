---
uid: Microsoft.Quantum.Characterization.ContinuousPhaseEstimationIteration
title: ContinuousPhaseEstimationIteration operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Characterization
qsharp.name: ContinuousPhaseEstimationIteration
qsharp.summary: >-
  Performs a single iteration of an iterative (classically-controlled) phase
  estimation algorithm using arbitrary real powers of a unitary oracle.
---

# ContinuousPhaseEstimationIteration operation

Namespace: [Microsoft.Quantum.Characterization](xref:Microsoft.Quantum.Characterization)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Performs a single iteration of an iterative (classically-controlled) phaseestimation algorithm using arbitrary real powers of a unitary oracle.

```qsharp
operation ContinuousPhaseEstimationIteration (oracle : Microsoft.Quantum.Oracles.ContinuousOracle, time : Double, theta : Double, targetState : Qubit[], controlQubit : Qubit) : Unit is Adj + Ctl
```


## Input

### oracle : [ContinuousOracle](xref:Microsoft.Quantum.Oracles.ContinuousOracle)

Operation acting on a double $t$ and a register,such that $U^t$ is applied to the given register, where $U$ is the unitarywhose phase is to be estimated, and where $t$ is the integer powergiven to the oracle


### time : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Number of times to apply the given unitary oracle.


### theta : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Angle by which to invert the phase on the control qubit beforeacting on the target state.


### targetState : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Register of state acted upon by the given unitary oracle.


### controlQubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)





## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

