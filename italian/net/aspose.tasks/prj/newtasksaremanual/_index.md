---
title: "Prj.NewTasksAreManual"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se i nuovi compiti sono creati come manuali"
type: docs
weight: 550
url: /it/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Determina se le nuove attività vengono create come manuali.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


