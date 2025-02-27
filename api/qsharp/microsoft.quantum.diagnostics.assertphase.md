---
uid: Microsoft.Quantum.Diagnostics.AssertPhase
title: AssertPhase operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: AssertPhase
qsharp.summary: Asserts that the phase of an equal superposition state has the expected value.
---

# AssertPhase operation

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Asserts that the phase of an equal superposition state has the expected value.

```qsharp
operation AssertPhase (expected : Double, qubit : Qubit, tolerance : Double) : Unit
```


## Description

This operation asserts that the phase $\phi$ of a quantum statethat may be expressed as$\frac{e^{i t}}{\sqrt{2}}(e^{i\phi}\ket{0} + e^{-i\phi}\ket{1})$for some arbitrary real $t$ has the expected value.

## Input

### expected : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The expected value of $\phi \in (-\pi,\pi]$.


### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

The qubit that stores the expected state.


### tolerance : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Absolute tolerance on the difference between actual and expected.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

The following assert succeeds:`qubit` is in state $\ket{\psi}=e^{i 0.5}\sqrt{1/2}\ket{0}+e^{i 0.5}\sqrt{1/2}\ket{1}$;- `AssertPhase(0.0, qubit, 10e-10);``qubit` is in state $\ket{\psi}=e^{i 0.5}\sqrt{1/2}\ket{0}+e^{-i 0.5}\sqrt{1/2}\ket{1}$;- `AssertPhase(0.5, qubit, 10e-10);``qubit` is in state $\ket{\psi}=e^{-i 2.2}\sqrt{1/2}\ket{0}+e^{i 0.2}\sqrt{1/2}\ket{1}$;- `AssertPhase(-1.2, qubit, 10e-10);`