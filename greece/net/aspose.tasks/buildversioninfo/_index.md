---
title: "Κλάση BuildVersionInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.BuildVersionInfo. Περιέχει την έκδοση κατασκευής και πληροφορίες προϊόντος."
type: docs
weight: 160
url: /el/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Περιέχει την έκδοση κατασκευής και πληροφορίες προϊόντος.

```csharp
public static class BuildVersionInfo
```

## Πεδία

| Όνομα | Περιγραφή |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Ο αριθμός έκδοσης πληροφοριών του assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Έκδοση assembly. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Έκδοση αρχείου. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Όνομα προϊόντος. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις πληροφορίες έκδοσης κατασκευής του Aspose.Tasks.

```csharp
// διαβάστε κοινές πληροφορίες σχετικά με την τρέχουσα έκδοση του Aspose.Tasks
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


