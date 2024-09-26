---
title: Class BuildVersionInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BuildVersionInfo class. Contains build version and product information
type: docs
weight: 160
url: /net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Contains build version and product information.

```csharp
public static class BuildVersionInfo
```

## Fields

| Name | Description |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | The informational version number of the assembly. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Assembly version. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | File version. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Product name. |

## Examples

Shows how to read build version info of Aspose.Tasks.

```csharp
// read common info about the current Aspose.Tasks version
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


