---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "VbaModuleCollection メソッド。コレクション オブジェクトを VbaModule オブジェクトのリストに変換します"
type: docs
weight: 100
url: /ja/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

コレクション オブジェクトを [`VbaModule`](../../vbamodule/) オブジェクトのリストに変換します。

```csharp
public List<VbaModule> ToList()
```

### 戻り値

オブジェクトのリストです。

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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


