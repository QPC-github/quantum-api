---
uid: Microsoft.Quantum.Arithmetic.MultiplyAndAddByModularInteger
title: MultiplyAndAddByModularInteger operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: MultiplyAndAddByModularInteger
qsharp.summary: Performs a modular multiply-and-add by integer constants on a qubit register.
---

# MultiplyAndAddByModularInteger operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Performs a modular multiply-and-add by integer constants on a qubit register.

```qsharp
operation MultiplyAndAddByModularInteger (constMultiplier : Int, modulus : Int, multiplicand : Microsoft.Quantum.Arithmetic.LittleEndian, summand : Microsoft.Quantum.Arithmetic.LittleEndian) : Unit is Adj + Ctl
```


## Description

Implements the map$$\begin{align}\ket{x} \ket{b} \mapsto \ket{x} \ket{(b + a \cdot x) \operatorname{mod} N}\end{align}$$for a given modulus $N$, constant multiplier $a$, and summand $b$.

## Input

### constMultiplier : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

An integer $a$ by which `multiplicand` is being multiplied.Must be between 0 and `modulus`-1, inclusive.


### modulus : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The modulus $N$ which addition and multiplication is taken with respect to.


### multiplicand : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

A quantum register representing an unsigned integer whose value, multiplied by `constMultiplier`, is tobe added to each basis state label of `summand`. Corresponds to theregister in state $\ket{x}$ above.


### summand : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

A quantum register representing an unsigned integer to use as the targetfor this operation. Corresponds to the register initially in $\ket{b}$ above.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

- For the circuit diagram and explanation see Figure 6 on [Page 7  of arXiv:quant-ph/0205095v3](https://arxiv.org/pdf/quant-ph/0205095v3.pdf#page=7)- This operation corresponds to CMULT(a)MOD(N) in  [arXiv:quant-ph/0205095v3](https://arxiv.org/pdf/quant-ph/0205095v3.pdf)

## See Also

- [Microsoft.Quantum.Arithmetic.MultiplyAndAddPhaseByModularInteger](xref:Microsoft.Quantum.Arithmetic.MultiplyAndAddPhaseByModularInteger)