---
title: "Prj.NewTasksEstimated"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se una durata stimata è mostrata per impostazione predefinita"
type: docs
weight: 570
url: /it/net/aspose.tasks/prj/newtasksestimated/
---
## Prj.NewTasksEstimated field

Determina se una durata stimata viene mostrata per impostazione predefinita.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEstimated;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.NewTasksEstimated.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEstimated, true);

Console.WriteLine("New Tasks Estimated: " + project.Get(Prj.NewTasksEstimated));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


