---
title: "Prj.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De naam van het project"
type: docs
weight: 540
url: /nl/net/aspose.tasks/prj/name/
---
## Prj.Name field

De naam van het project.

```csharp
public static readonly Key<string, PrjKey> Name;
```

## Voorbeelden

Toont hoe de projectnaam te lezen/schrijven.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

project.Set(Prj.Name, "Custom Project Name");

Console.WriteLine("Project name: " + project.Get(Prj.Name));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


