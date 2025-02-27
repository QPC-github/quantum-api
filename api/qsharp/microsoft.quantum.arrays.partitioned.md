---
uid: Microsoft.Quantum.Arrays.Partitioned
title: Partitioned function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Partitioned
qsharp.summary: Splits an array into multiple parts.
---

# Partitioned function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Splits an array into multiple parts.

```qsharp
function Partitioned<'T> (nElements : Int[], arr : 'T[]) : 'T[][]
```


## Input

### nElements : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

Number of elements in each part of array


### arr : 'T[]

Input array to be split.



## Output : 'T[][]

Multiple arrays where the first array is the first `nElements[0]` of `arr`and the second array are the next `nElements[1]` of `arr` etc. The last arraywill contain all remaining elements. If the array is split exactly, thelast array will be the empty array, indicating there are no remaining elements.In other words, `Tail(Partitioned(...))` will always return the remainingelements, while `Most(Partitioned(...))` will always return the completepartitions of the array.

## Type Parameters

### 'T



## Example

```qsharp// The following returns [[1, 5], [3], [7]];let split = Partitioned([2,1], [1,5,3,7]);// The following returns [[1, 5], [3, 7], []];let split = Partitioned([2,2], [1,5,3,7]);```