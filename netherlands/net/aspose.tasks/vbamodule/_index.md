---
title: "Klasse VbaModule"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.VbaModule klasse. Vertegenwoordigt een VBA-module"
type: docs
weight: 2810
url: /nl/net/aspose.tasks/vbamodule/
---
## VbaModule class

Stelt een VBA-module voor.

```csharp
public sealed class VbaModule
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Haalt een verzameling van de attributen van de module op. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Haalt een naam van de VBA-module op |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Haalt de broncode van de VBA-module op of stelt deze in |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Haalt het type van de module op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Maakt een instantie van `VbaModule` met het type VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Maakt een instantie van `VbaModule` met het type VbaModuleType.ProceduralModule. |

## Voorbeelden

Toont hoe modules van een VBA-project gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


