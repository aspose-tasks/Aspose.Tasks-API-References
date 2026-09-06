---
title: "类 BuildVersionInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BuildVersionInfo 类。包含构建版本和产品信息"
type: docs
weight: 160
url: /zh/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

包含构建版本和产品信息。

```csharp
public static class BuildVersionInfo
```

## 字段

| 名称 | 描述 |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | 程序集的信息版本号。 |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | 程序集版本。 |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | 文件版本。 |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | 产品名称。 |

## 示例

展示如何读取 Aspose.Tasks 的构建版本信息。

```csharp
// 读取当前 Aspose.Tasks 版本的常规信息
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


