---
title: "Prj.DefaultFinishTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De standaard eindtijd van nieuwe taken"
type: docs
weight: 230
url: /nl/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

De standaard eindtijd van nieuwe taken.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Voorbeelden

Toont hoe de eigenschap Prj.DefaultFinishTime te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


