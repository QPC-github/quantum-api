---
uid: Microsoft.Quantum.AmplitudeAmplification.StandardAmplitudeAmplification
title: StandardAmplitudeAmplification function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.AmplitudeAmplification
qsharp.name: StandardAmplitudeAmplification
qsharp.summary: Standard Amplitude Amplification algorithm
---

# StandardAmplitudeAmplification function

Namespace: [Microsoft.Quantum.AmplitudeAmplification](xref:Microsoft.Quantum.AmplitudeAmplification)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Standard Amplitude Amplification algorithm

```qsharp
function StandardAmplitudeAmplification (nIterations : Int, stateOracle : Microsoft.Quantum.Oracles.StateOracle, idxFlagQubit : Int) : (Qubit[] => Unit is Adj + Ctl)
```


## Input

### nIterations : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Number of iterations $n$ of amplitude amplification


### stateOracle : [StateOracle](xref:Microsoft.Quantum.Oracles.StateOracle)

Unitary oracle $A$ that prepares start state


### idxFlagQubit : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Index to flag qubit



## Output : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj + Ctl

An operation that implements the standard amplitude amplification quantum algorithm

## Remarks

This is the standard amplitude amplification algorithm obtained by a choice of reflection phases computed by `StandardReflectionPhases`Assuming that\begin{align}A\ket{0}\_{f}\ket{0}\_s= \lambda\ket{1}\_f\ket{\text{target}}\_s + \sqrt{1-|\lambda|^2}\ket{0}\_f\cdots,\end{align}this operation prepares the state\begin{align}\operatorname{StandardAmplitudeAmplification}\ket{0}\_{f}\ket{0}\_s= \sin((2n+1)\sin^{-1}(\lambda))\ket{1}\_f\ket{\text{target}}\_s + \cdots\ket{0}\_f\end{align}In most cases, `flagQubit` and `auxiliaryRegister` is initialized in the state $\ket{0}\_f\ket{0}\_a$.

## References

- [ *G. Brassard, P. Hoyer, M. Mosca, A. Tapp* ](https://arxiv.org/abs/quant-ph/0005055)