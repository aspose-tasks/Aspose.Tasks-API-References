---
title: "Prj.EarnedValueMethod"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il metodo predefinito per calcolare il valore guadagnato"
type: docs
weight: 310
url: /it/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

Il metodo predefinito per calcolare il valore guadagnato.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


