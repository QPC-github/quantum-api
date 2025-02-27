---
uid: Microsoft.Quantum.Simulation.GeneratorSystem
title: GeneratorSystem user defined type
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.Simulation
qsharp.name: GeneratorSystem
qsharp.summary: >-
  Represents a collection of `GeneratorIndex`es.

  We iterate over this
  collection using a single-index integer, and the size of the
  collection is assumed to be known.
---

# GeneratorSystem user defined type

Namespace: [Microsoft.Quantum.Simulation](xref:Microsoft.Quantum.Simulation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Represents a collection of `GeneratorIndex`es.We iterate over thiscollection using a single-index integer, and the size of thecollection is assumed to be known.

```qsharp

newtype GeneratorSystem = (Int, (Int -> Microsoft.Quantum.Simulation.GeneratorIndex));
```



## Remarks

Instances of `GeneratorSystem` can be defined easily using the<xref:Microsoft.Quantum.Arrays.LookupFunction> function.

## See Also

- [Microsoft.Quantum.Arrays.LookupFunction](xref:Microsoft.Quantum.Arrays.LookupFunction)