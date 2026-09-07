---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se nuove risorse o attività vengono aggiunte automaticamente a un pool di risorse o attività"
type: docs
weight: 50
url: /it/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Determina se nuove risorse o attività vengono aggiunte automaticamente a un pool di risorse o attività.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.AutoAddNewResourcesAndTasks.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


