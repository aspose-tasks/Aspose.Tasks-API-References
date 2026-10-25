---
title: "Prj.Guid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il GUID del progetto"
type: docs
weight: 360
url: /it/net/aspose.tasks/prj/guid/
---
## Prj.Guid field

Il GUID del progetto.

```csharp
public static readonly Key<Guid, PrjKey> Guid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.Guid.

```csharp
var project = new Project();

project.Set(Prj.Guid, new Guid("efcc0d63-d8e0-4a34-9f3e-9f973f50238a"));

Console.WriteLine("Guid: " + project.Get(Prj.Guid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


