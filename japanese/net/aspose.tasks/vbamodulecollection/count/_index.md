---
title: "VbaModuleCollection.Count"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "VbaModuleCollection プロパティ。"
type: docs
weight: 10
url: /ja/net/aspose.tasks/vbamodulecollection/count/
---
## VbaModuleCollection.Count property

```csharp
public int Count { get; }
```

## 例

VBA モジュールの反復方法を示します。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### 関連項目

* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


