---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of het veld Complete of Physical Complete gebruikt moet worden om de begrote kostprijs van uitgevoerd werk (BCWP) te berekenen"
type: docs
weight: 350
url: /nl/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Bepaalt of het veld % Voltooid of Fysiek % Voltooid moet worden gebruikt om de begrote kosten van uitgevoerd werk (BCWP) te berekenen.

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Voorbeelden

Toont hoe de Tsk.EarnedValueMethod-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


