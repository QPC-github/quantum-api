---
uid: Microsoft.Quantum.Math.Round
title: Round function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Math
qsharp.name: Round
qsharp.summary: Returns the nearest integer to the specified number.
---

# Round function

Namespace: [Microsoft.Quantum.Math](xref:Microsoft.Quantum.Math)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns the nearest integer to the specified number.

```qsharp
function Round (value : Double) : Int
```


## Input

### value : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)





## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The nearest integer to the input.

## Example

```Message($"{Round(3.1)}");   //  3Message($"{Round(3.7)}");   //  4Message($"{Round(-3.1)}");  // -3Message($"{Round(-3.7)}");  // -4```