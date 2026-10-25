---
title: "Prj.UpdateManuallyScheduledTasksWhenEditingLinks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se i compiti manuali devono essere aggiornati quando i collegamenti sono stati modificati"
type: docs
weight: 770
url: /it/net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

Determina se le attività manuali devono essere aggiornate quando i collegamenti sono stati modificati.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.UpdateManuallyScheduledTasksWhenEditingLinks.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


