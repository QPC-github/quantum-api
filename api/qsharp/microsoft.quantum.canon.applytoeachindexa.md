---
uid: Microsoft.Quantum.Canon.ApplyToEachIndexA
title: ApplyToEachIndexA operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyToEachIndexA
qsharp.summary: >-
  Applies a single-qubit operation to each indexed element in a register.
  The modifier `A` indicates that the single-qubit operation is adjointable.
---

# ApplyToEachIndexA operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a single-qubit operation to each indexed element in a register.The modifier `A` indicates that the single-qubit operation is adjointable.

```qsharp
operation ApplyToEachIndexA<'T> (singleElementOperation : ((Int, 'T) => Unit is Adj), register : 'T[]) : Unit is Adj
```


## Input

### singleElementOperation : ([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),'T) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

Operation to apply to each qubit.


### register : 'T[]

Array of qubits on which to apply the given operation.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The target on which each of the operations acts.

## See Also

- [Microsoft.Quantum.Canon.ApplyToEachIndex](xref:Microsoft.Quantum.Canon.ApplyToEachIndex)