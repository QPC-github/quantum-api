---
uid: Microsoft.Quantum.Random.DrawRandomInt
title: DrawRandomInt operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Random
qsharp.name: DrawRandomInt
qsharp.summary: Draws a random integer in a given inclusive range.
---

# DrawRandomInt operation

Namespace: [Microsoft.Quantum.Random](xref:Microsoft.Quantum.Random)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Draws a random integer in a given inclusive range.

```qsharp
operation DrawRandomInt (min : Int, max : Int) : Int
```


## Input

### min : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The smallest integer to be drawn.


### max : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The largest integer to be drawn.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

An integer in the inclusive range from `min` to `max` with uniformprobability.

## Example

The following Q# snippet randomly rolls a six-sided die:```qsharplet roll = DrawRandomInt(1, 6);```

## Remarks

Fails if `max < min`.

## See Also

- [Microsoft.Quantum.DiscreteUniformDistribution](xref:Microsoft.Quantum.DiscreteUniformDistribution)