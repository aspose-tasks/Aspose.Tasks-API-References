---
title: "Prj.Category"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. La categoria di un progetto"
type: docs
weight: 100
url: /it/net/aspose.tasks/prj/category/
---
## Prj.Category field

La categoria di un progetto.

```csharp
public static readonly Key<string, PrjKey> Category;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.Category.

```csharp
var project = new Project();

project.Set(Prj.Category, "Special");

Console.WriteLine("Category: " + project.Get(Prj.Category));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


