---
title: "Classe BuildVersionInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.BuildVersionInfo. Contiene la versione di build e le informazioni sul prodotto"
type: docs
weight: 160
url: /it/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Contiene la versione di build e le informazioni sul prodotto.

```csharp
public static class BuildVersionInfo
```

## Campi

| Nome | Descrizione |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Il numero di versione informativa dell'assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Versione dell'assembly. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Versione del file. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Nome del prodotto. |

## Esempi

Mostra come leggere le informazioni sulla versione di build di Aspose.Tasks.

```csharp
// leggi le informazioni comuni sulla versione corrente di Aspose.Tasks
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


