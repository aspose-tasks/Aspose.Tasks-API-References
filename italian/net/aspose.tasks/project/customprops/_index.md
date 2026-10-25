---
title: "Project.CustomProps"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene la raccolta delle proprietà personalizzate del progetto"
type: docs
weight: 260
url: /it/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Ottiene la collezione delle proprietà personalizzate del progetto.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## Esempi

Mostra come leggere le meta proprietà del progetto (API obsoleta).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// le proprietà personalizzate sono disponibili tramite la collezione tipizzata
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Le proprietà integrate sono disponibili direttamente
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// oppure come elemento della raccolta delle proprietà integrate
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Vedi anche

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


