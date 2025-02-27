---
uid: Microsoft.Quantum.Arrays.Enumerated
title: Enumerated function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Enumerated
qsharp.summary: >-
  Given an array, returns a new array containing elements of the original
  array along with the indices of each element.
---

# Enumerated function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an array, returns a new array containing elements of the originalarray along with the indices of each element.

```qsharp
function Enumerated<'TElement> (array : 'TElement[]) : (Int, 'TElement)[]
```


## Input

### array : 'TElement[]

An array whose elements are to be enumerated.



## Output : ([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),'TElement)[]

A new array containing elements of the original array along with theirindices.

## Type Parameters

### 'TElement

The type of elements of the array.

## Example

The following `for` loops are equivalent:```qsharpfor (idx in IndexRange(array)) {    let element = array[idx];    ...}for ((idx, element) in Enumerated(array)) { ... }```