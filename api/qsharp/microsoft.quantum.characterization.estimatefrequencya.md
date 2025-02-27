---
uid: Microsoft.Quantum.Characterization.EstimateFrequencyA
title: EstimateFrequencyA operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Characterization
qsharp.name: EstimateFrequencyA
qsharp.summary: >-
  Given a preparation that is adjointable and measurement, estimates the frequency
  with which that measurement succeeds (returns `Zero`) by
  performing a given number of trials.
---

# EstimateFrequencyA operation

Namespace: [Microsoft.Quantum.Characterization](xref:Microsoft.Quantum.Characterization)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given a preparation that is adjointable and measurement, estimates the frequencywith which that measurement succeeds (returns `Zero`) byperforming a given number of trials.

```qsharp
operation EstimateFrequencyA (preparation : (Qubit[] => Unit is Adj), measurement : (Qubit[] => Result), nQubits : Int, nMeasurements : Int) : Double
```


## Input

### preparation : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

An adjointable operation $P$ that prepares a given state $\rho$ onits input register.


### measurement : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal) 

An operation $M$ representing the measurement of interest.


### nQubits : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of qubits on which the preparation and measurementeach act.


### nMeasurements : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of times that the measurement should be performedin order to estimate the frequency of interest.



## Output : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

An estimate $\hat{p}$ of the frequency with which$M(P(\ket{00 \cdots 0}\bra{00 \cdots 0}))$ returns `Zero`,obtained using the unbiased binomial estimator $\hat{p} =n\_{\uparrow} / n\_{\text{measurements}}$, where $n\_{\uparrow}$ isthe number of `Zero` results observed.

## Remarks

For adjointable operations, certain assumptions can be made such likecalling the operation will prepare the qubits to exactly the same state,which allow target machines to make some performance optimizations.