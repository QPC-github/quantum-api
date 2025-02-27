---
uid: Microsoft.Quantum.Canon.MultiplexPauli
title: MultiplexPauli operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: MultiplexPauli
qsharp.summary: Applies a Pauli rotation conditioned on an array of qubits.
---

# MultiplexPauli operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a Pauli rotation conditioned on an array of qubits.

```qsharp
operation MultiplexPauli (coefficients : Double[], pauli : Pauli, control : Microsoft.Quantum.Arithmetic.LittleEndian, target : Qubit) : Unit is Adj + Ctl
```


## Description

This applies a multiply controlled unitary operation that performsrotations by angle $\theta_j$ about single-qubit Pauli operator $P$when controlled by the $n$-qubit number state $\ket{j}$.In particular, the action of this operation is represented by theunitary$$\begin{align}U = \sum^{2^n - 1}_{j=0} \ket{j}\bra{j} \otimes e^{i P \theta_j}.\end{align}$$

## Input

### coefficients : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)[]

Array of up to $2^n$ coefficients $\theta_j$. The $j$th coefficientindexes the number state $\ket{j}$ encoded in little-endian format.


### pauli : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)

Pauli operator $P$ that determines axis of rotation.


### control : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

$n$-qubit control register that encodes number states $\ket{j}$ inlittle-endian format.


### target : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Single qubit register that is rotated by $e^{i P \theta_j}$.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

`coefficients` will be padded with elements $\theta_j = 0.0$ iffewer than $2^n$ are specified.

## See Also

- [Microsoft.Quantum.Canon.ApproximatelyMultiplexPauli](xref:Microsoft.Quantum.Canon.ApproximatelyMultiplexPauli)