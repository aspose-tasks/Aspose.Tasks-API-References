---
title: "Prj.BaselineForEarnedValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La baseline specifica usata per calcolare i valori di varianza"
type: docs
weight: 80
url: /it/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

La baseline specifica utilizzata per calcolare i valori di varianza.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


