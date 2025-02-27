---
uid: Microsoft.Quantum.Preparation.PrepareUniformSuperposition
title: PrepareUniformSuperposition operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Preparation
qsharp.name: PrepareUniformSuperposition
qsharp.summary: Creates a uniform superposition over states that encode 0 through `nIndices - 1`.
---

# PrepareUniformSuperposition operation

Namespace: [Microsoft.Quantum.Preparation](xref:Microsoft.Quantum.Preparation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Creates a uniform superposition over states that encode 0 through `nIndices - 1`.

```qsharp
operation PrepareUniformSuperposition (nIndices : Int, indexRegister : Microsoft.Quantum.Arithmetic.LittleEndian) : Unit is Adj + Ctl
```


## Description

This operation can be described by a unitary matrix $U$ that createsa uniform superposition over all number states$0$ to $M-1$, given an input state $\ket{0\cdots 0}$. In other words,$$\begin{align}U \ket{0} = \frac{1}{\sqrt{M}} \sum_{j=0}^{M - 1} \ket{j}.\end{align}$$.

## Input

### nIndices : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The desired number of states $M$ in the uniform superposition.


### indexRegister : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

The qubit register that stores the number states in `LittleEndian` format.This register must be able to store the number $M-1$, and is assumed to beinitialized in the state $\ket{0\cdots 0}$.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

The following example prepares the state $\frac{1}{\sqrt{6}}\sum_{j=0}^{5}\ket{j}$on $3$ qubits.```Q#let nIndices = 6;using(indexRegister = Qubit[3]) {    PrepareUniformSuperposition(nIndices, LittleEndian(indexRegister));    // ...}```

## Remarks

The operation is adjointable, but requires that `indexRegister` is in a uniformsuperposition over the first `nIndices` basis states in that case.