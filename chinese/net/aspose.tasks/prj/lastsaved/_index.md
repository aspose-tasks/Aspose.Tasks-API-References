---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目上次保存的日期。以 UTC 格式保存在 mpp 文件中。DateTime 类型"
type: docs
weight: 440
url: /zh/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

项目上次保存的日期。以 UTC 格式保存在 mpp 文件中。DateTime 类型。

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


