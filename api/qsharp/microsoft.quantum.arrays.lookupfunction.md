---
uid: Microsoft.Quantum.Arrays.LookupFunction
title: LookupFunction function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: LookupFunction
qsharp.summary: >-
  Given an array, returns a function which returns elements of that
  array.
---

# LookupFunction function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an array, returns a function which returns elements of thatarray.

```qsharp
function LookupFunction<'T> (array : 'T[]) : (Int -> 'T)
```


## Input

### array : 'T[]

The array to be represented as a lookup function.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals) -> 'T

A function `f` such that `f(idx) == f[idx]`.

## Type Parameters

### 'T

The type of the elements of the array being represented as a lookupfunction.

## Remarks

This function is mainly useful for interoperating with functions andoperations that take `Int -> 'T` functions as their arguments. Thisis common, for instance, in the generator representation library,where functions are used to avoid the need to record an entire arrayin memory.