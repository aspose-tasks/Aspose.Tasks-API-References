---
title: "Prj.Manager"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il responsabile di un progetto"
type: docs
weight: 450
url: /it/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

Il responsabile di un progetto.

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.Manager.

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


