---
uid: Microsoft.Quantum.Math.ExpModL
title: ExpModL function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Math
qsharp.name: ExpModL
qsharp.summary: >-
  Returns an integer raised to a given power, with respect to a given
  modulus.
---

# ExpModL function

Namespace: [Microsoft.Quantum.Math](xref:Microsoft.Quantum.Math)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns an integer raised to a given power, with respect to a givenmodulus.

```qsharp
function ExpModL (expBase : BigInt, power : BigInt, modulus : BigInt) : BigInt
```


## Description

Let us denote expBase by $x$, power by $p$ and modulus by $N$.The function returns $x^p \operatorname{mod} N$.We assume that $N$, $x$ are positive and power is non-negative.

## Input

### expBase : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)




### power : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)




### modulus : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)





## Output : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)



## Remarks

Takes time proportional to the number of bits in `power`, not the `power` itself.