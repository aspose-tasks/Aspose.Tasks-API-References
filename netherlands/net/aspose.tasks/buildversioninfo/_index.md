---
title: "Klasse BuildVersionInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BuildVersionInfo-klasse. Bevat buildversie en productinformatie"
type: docs
weight: 160
url: /nl/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Bevat de buildversie en productinformatie.

```csharp
public static class BuildVersionInfo
```

## Velden

| Naam | Beschrijving |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Het informatieve versienummer van de assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Assembly-versie. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Bestandsversie. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Productnaam. |

## Voorbeelden

Toont hoe de buildversie‑info van Aspose.Tasks te lezen.

```csharp
// lees algemene informatie over de huidige Aspose.Tasks‑versie
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


