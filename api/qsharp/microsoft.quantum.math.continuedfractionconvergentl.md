---
uid: Microsoft.Quantum.Math.ContinuedFractionConvergentL
title: ContinuedFractionConvergentL function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Math
qsharp.name: ContinuedFractionConvergentL
qsharp.summary: >-
  Finds the continued fraction convergent closest to `fraction`
  with the denominator less or equal to `denominatorBound`
---

# ContinuedFractionConvergentL function

Namespace: [Microsoft.Quantum.Math](xref:Microsoft.Quantum.Math)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Finds the continued fraction convergent closest to `fraction`with the denominator less or equal to `denominatorBound`

```qsharp
function ContinuedFractionConvergentL (fraction : Microsoft.Quantum.Math.BigFraction, denominatorBound : BigInt) : Microsoft.Quantum.Math.BigFraction
```


## Input

### fraction : [BigFraction](xref:Microsoft.Quantum.Math.BigFraction)




### denominatorBound : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)





## Output : [BigFraction](xref:Microsoft.Quantum.Math.BigFraction)

Continued fraction closest to `fraction`with the denominator less or equal to `denominatorBound`