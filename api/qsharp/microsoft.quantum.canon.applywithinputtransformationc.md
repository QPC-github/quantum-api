---
uid: Microsoft.Quantum.Canon.ApplyWithInputTransformationC
title: ApplyWithInputTransformationC operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyWithInputTransformationC
qsharp.summary: >-
  Given an operation that accepts some input, a function that
  returns an output compatible with that operation, and an input to that
  function, applies the operation using the function to transform the
  input to a form expected by the operation.
---

# ApplyWithInputTransformationC operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an operation that accepts some input, a function thatreturns an output compatible with that operation, and an input to thatfunction, applies the operation using the function to transform theinput to a form expected by the operation.

```qsharp
operation ApplyWithInputTransformationC<'T, 'U> (fn : ('U -> 'T), op : ('T => Unit is Ctl), input : 'U) : Unit is Ctl
```


## Input

### fn : 'U -> 'T

A function that transforms the given input into a form expected by theoperation.


### op : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

The operation to be applied.


### input : 'U

An input to the function.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T


### 'U



## Example

The following call uses@"Microsoft.Quantum.Arithmetic.LittleEndianAsBigEndian" to applyan operation designed for@"Microsoft.Quantum.Arithmetic.BigEndian" inputs to an input of type@"Microsoft.Quantum.Arithmetic.LittleEndian":```qsharpApplyWithInputTransformation(LittleEndianAsBigEndian, ApplyXorInPlaceBE, LittleEndian(qubits));```

## See Also

- [Microsoft.Quantum.Canon.ApplyWithInputTransformation](xref:Microsoft.Quantum.Canon.ApplyWithInputTransformation)
- [Microsoft.Quantum.Canon.ApplyWithInputTransformationA](xref:Microsoft.Quantum.Canon.ApplyWithInputTransformationA)
- [Microsoft.Quantum.Canon.ApplyWithInputTransformationCA](xref:Microsoft.Quantum.Canon.ApplyWithInputTransformationCA)
- [Microsoft.Quantum.Canon.TransformedOperation](xref:Microsoft.Quantum.Canon.TransformedOperation)