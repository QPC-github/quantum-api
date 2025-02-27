---
uid: Microsoft.Quantum.Characterization.RobustPhaseEstimation
title: RobustPhaseEstimation operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Characterization
qsharp.name: RobustPhaseEstimation
qsharp.summary: >-
  Performs the robust non-iterative quantum phase estimation algorithm for a given oracle `U` and eigenstate,
  and provides a single real-valued estimate of the phase with variance scaling at the Heisenberg limit.
---

# RobustPhaseEstimation operation

Namespace: [Microsoft.Quantum.Characterization](xref:Microsoft.Quantum.Characterization)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Performs the robust non-iterative quantum phase estimation algorithm for a given oracle `U` and eigenstate,and provides a single real-valued estimate of the phase with variance scaling at the Heisenberg limit.

```qsharp
operation RobustPhaseEstimation (bitsPrecision : Int, oracle : Microsoft.Quantum.Oracles.DiscreteOracle, targetState : Qubit[]) : Double
```


## Input

### bitsPrecision : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

This provides an estimate of $\phi$ with standard deviation$\sigma \le 2\pi / 2^\text{bitsPrecision}$ using a number of queries scaling like $\sigma \le 10.7 \pi / \text{# of queries}$.


### oracle : [DiscreteOracle](xref:Microsoft.Quantum.Oracles.DiscreteOracle)

An operation implementing $U^m$ for given integer powers $m$.


### targetState : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A quantum register that $U$ acts on. If it stores an eigenstate$\ket{\phi}$ of $U$, then $U\ket{\phi} = e^{i\phi} \ket{\phi}$for $\phi\in(-\pi,\pi]$ an unknown phase.



## Output : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)



## Remarks

In the limit of a large number of queries, Cramer-Rao lower boundsfor the standard deviation of the estimate of $\phi$ satisfy$\sigma \ge 2 \pi / \text{# of queries}$.

## References

- Robust Calibration of a Universal Single-Qubit Gate-Set via Robust Phase Estimation  Shelby Kimmel, Guang Hao Low, Theodore J. Yoder  https://arxiv.org/abs/1502.02677