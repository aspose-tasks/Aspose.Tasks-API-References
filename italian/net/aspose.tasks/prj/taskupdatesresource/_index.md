---
title: "Prj.TaskUpdatesResource"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. Determina se gli aggiornamenti alle attività aggiornano le risorse"
type: docs
weight: 710
url: /it/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

Determina se gli aggiornamenti alle attività aggiornano le risorse.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.TaskUpdatesResource.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


