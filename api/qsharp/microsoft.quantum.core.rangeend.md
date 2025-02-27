---
uid: Microsoft.Quantum.Core.RangeEnd
title: RangeEnd function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Core
qsharp.name: RangeEnd
qsharp.summary: >-
  Returns the defined end value of the given range,
  which is not necessarily the last element in the sequence.
---

# RangeEnd function

Namespace: [Microsoft.Quantum.Core](xref:Microsoft.Quantum.Core)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns the defined end value of the given range,which is not necessarily the last element in the sequence.

```qsharp
function RangeEnd (range : Range) : Int
```


## Input

### range : [Range](xref:microsoft.quantum.qsharp.valueliterals#range-literals)

Input range.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The defined end value of the given range.

## Remarks

A range expression's first element is `start`,its second element is `start+step`, third element is `start+step+step`, etc.,until `end` is passed.Note that the defined end value of a range can differ from the last element in the sequence specified by the range;for example, in a range 0 .. 2 .. 5 the last element is 4 but the end value is 5.