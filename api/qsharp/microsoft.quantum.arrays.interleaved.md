---
uid: Microsoft.Quantum.Arrays.Interleaved
title: Interleaved function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Interleaved
qsharp.summary: Interleaves two arrays of (almost) same size.
---

# Interleaved function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Interleaves two arrays of (almost) same size.

```qsharp
function Interleaved<'T> (first : 'T[], second : 'T[]) : 'T[]
```


## Description

This function returns the interleaving of two arrays, startingwith the first element from the first array, then the firstelement from the second array, and so on.The first array must either beof the same length as the second one, or can have one more element.

## Input

### first : 'T[]

The first array to be interleaved.


### second : 'T[]

The second array to be interleaved.



## Output : 'T[]

Interleaved array

## Type Parameters

### 'T

The type of each element of `first` and `second`.

## Example

```qsharp// same as int1 = [1, -1, 2, -2, 3, -3]let int1 = Interleaved([1, 2, 3], [-1, -2, -3])// same as int2 = [false, true, false, true, false]let int2 = Interleaved(ConstantArray(3, false), ConstantArray(2, true));```