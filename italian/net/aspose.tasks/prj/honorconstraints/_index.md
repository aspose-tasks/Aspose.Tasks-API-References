---
title: "Prj.HonorConstraints"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se le attività rispettano le loro date di vincolo."
type: docs
weight: 370
url: /it/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

Determina se le attività rispettano le loro date vincolanti.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.HonorConstraints.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


