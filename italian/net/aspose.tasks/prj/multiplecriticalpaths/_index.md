---
title: "Prj.MultipleCriticalPaths"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se vengono calcolati più percorsi critici"
type: docs
weight: 530
url: /it/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

Determina se vengono calcolati percorsi critici multipli.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MultipleCriticalPaths.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


