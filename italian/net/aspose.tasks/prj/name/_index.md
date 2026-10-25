---
title: "Prj.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il nome del progetto"
type: docs
weight: 540
url: /it/net/aspose.tasks/prj/name/
---
## Prj.Name field

Il nome del progetto.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Esempi

Mostra come leggere/scrivere il nome del progetto.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


