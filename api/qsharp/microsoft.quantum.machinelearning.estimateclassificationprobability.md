---
uid: Microsoft.Quantum.MachineLearning.EstimateClassificationProbability
title: EstimateClassificationProbability operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.MachineLearning
qsharp.name: EstimateClassificationProbability
qsharp.summary: >-
  Given a sample and a sequential classifier, estimates the
  classification probability for that sample by repeatedly measuring
  the output of the classifier on the given sample.
---

# EstimateClassificationProbability operation

Namespace: [Microsoft.Quantum.MachineLearning](xref:Microsoft.Quantum.MachineLearning)

Package: [Microsoft.Quantum.MachineLearning](https://nuget.org/packages/Microsoft.Quantum.MachineLearning)


Given a sample and a sequential classifier, estimates theclassification probability for that sample by repeatedly measuringthe output of the classifier on the given sample.

```qsharp
operation EstimateClassificationProbability (tolerance : Double, model : Microsoft.Quantum.MachineLearning.SequentialModel, sample : Double[], nMeasurements : Int) : Double
```


## Input

### tolerance : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The tolerance to allow in encoding the sample into a state preparationoperation.


### model : [SequentialModel](xref:Microsoft.Quantum.MachineLearning.SequentialModel)

The sequential model to be used to estimate the classificationprobability for the given sample.


### sample : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)[]

The feature vector for the sample to be classified.


### nMeasurements : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of measurements to use in estimating the classificationprobability.



## Output : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

An estimate of the classification probability for the given sample.