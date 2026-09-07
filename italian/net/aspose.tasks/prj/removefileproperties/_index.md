---
title: "Prj.RemoveFileProperties"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se tutte le proprietà dei file verranno rimosse al salvataggio"
type: docs
weight: 600
url: /it/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Determina se tutte le proprietà del file verranno rimosse al salvataggio.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


