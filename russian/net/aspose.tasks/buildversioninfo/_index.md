---
title: "Класс BuildVersionInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.BuildVersionInfo. Содержит информацию о версии сборки и продукте."
type: docs
weight: 160
url: /ru/net/aspose.tasks/buildversioninfo/
---
## BuildVersionInfo class

Содержит информацию о версии сборки и продукте.

```csharp
public static class BuildVersionInfo
```

## Поля

| Имя | Описание |
| --- | --- |
| static readonly [AssemblyInformationalVersion](../../aspose.tasks/buildversioninfo/assemblyinformationalversion/) | Информационный номер версии сборки. |
| static readonly [AssemblyVersion](../../aspose.tasks/buildversioninfo/assemblyversion/) | Версия сборки. |
| static readonly [FileVersion](../../aspose.tasks/buildversioninfo/fileversion/) | Версия файла. |
| static readonly [Product](../../aspose.tasks/buildversioninfo/product/) | Название продукта. |

## Примеры

Показывает, как читать информацию о версии сборки Aspose.Tasks.

```csharp
// чтение общей информации о текущей версии Aspose.Tasks
Console.WriteLine("Product: " + BuildVersionInfo.Product);
Console.WriteLine("File Version: " + BuildVersionInfo.FileVersion);
Console.WriteLine("Assembly Version: " + BuildVersionInfo.AssemblyVersion);
Console.WriteLine("Assembly Informational Version: " + BuildVersionInfo.AssemblyInformationalVersion);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


