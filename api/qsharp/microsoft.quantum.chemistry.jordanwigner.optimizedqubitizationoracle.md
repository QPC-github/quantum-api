---
uid: Microsoft.Quantum.Chemistry.JordanWigner.OptimizedQubitizationOracle
title: OptimizedQubitizationOracle function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Chemistry.JordanWigner
qsharp.name: OptimizedQubitizationOracle
qsharp.summary: >-
  Returns T-count optimized Qubitization operation
  and the parameters necessary to run it.
---

# OptimizedQubitizationOracle function

Namespace: [Microsoft.Quantum.Chemistry.JordanWigner](xref:Microsoft.Quantum.Chemistry.JordanWigner)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Returns T-count optimized Qubitization operationand the parameters necessary to run it.

```qsharp
function OptimizedQubitizationOracle (qSharpData : Microsoft.Quantum.Chemistry.JordanWigner.JordanWignerEncodingData, targetError : Double) : (Int, (Double, (Qubit[] => Unit is Adj + Ctl)))
```


## Input

### qSharpData : [JordanWignerEncodingData](xref:Microsoft.Quantum.Chemistry.JordanWigner.JordanWignerEncodingData)

Hamiltonian described by `JordanWignerEncodingData` format.


### targetError : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Error of auxillary state preparation step.



## Output : ([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),([Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals),[Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj + Ctl))

A tuple where: `Int` is the number of qubits allocated,`Double` is the one-norm of Hamiltonian coefficients, and the operationis the Quantum walk created by Qubitization.