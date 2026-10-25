---
title: "Tsk.EarnedValueMethod"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se il campo Complete o Physical Complete deve essere usato per calcolare il costo preventivato del lavoro eseguito (BCWP)"
type: docs
weight: 350
url: /it/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Determina se il campo % Completato o % Completato fisico deve essere usato per calcolare il costo preventivato del lavoro eseguito (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


