---
title: "Classe BuildVersionInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.BuildVersionInfo. Contient les informations de version de construction et du produit"
type: docs
weight: 160
url: /fr/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Contient la version de build et les informations du produit.

```csharp
public static class BuildVersionInfo
```

## Champs

| Nom | Description |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Le numéro de version informationnelle de l'assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Version de l'assembly. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Version du fichier. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Nom du produit. |

## Exemples

Montre comment lire les informations de version de construction d'Aspose.Tasks.

```csharp
// lire les informations communes sur la version actuelle d'Aspose.Tasks
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


