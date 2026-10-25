---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。保存项目文件时所使用的 Microsoft Office Project 版本"
type: docs
weight: 620
url: /zh/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

保存项目文件时使用的 Microsoft Office Project 版本。

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## 示例

展示如何检查项目的保存版本和保存日期。

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// 显示项目版本
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


