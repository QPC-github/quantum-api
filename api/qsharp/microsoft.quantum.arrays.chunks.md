---
uid: Microsoft.Quantum.Arrays.Chunks
title: Chunks function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Chunks
qsharp.summary: Splits an array into multiple parts of equal length.
---

# Chunks function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Splits an array into multiple parts of equal length.

```qsharp
function Chunks<'T> (nElements : Int, arr : 'T[]) : 'T[][]
```


## Input

### nElements : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The length of each chunk. Must be positive.


### arr : 'T[]

The array to be split.



## Output : 'T[][]

A array containing each chunk of the original array.

## Type Parameters

### 'T



## Remarks

Note that the last element of the output may be shorterthan `nElements` if `Length(arr)` is not divisible by `nElements`.