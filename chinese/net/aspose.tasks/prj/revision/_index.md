---
title: "Prj.Revision"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目保存的次数"
type: docs
weight: 610
url: /zh/net/aspose.tasks/prj/revision/
---
## Prj.Revision field

项目保存的次数。

```csharp
public static readonly Key<int, PrjKey> Revision;
```

## 示例

展示如何设置项目元信息。

```csharp
var project = new Project(DataDir + "WriteProjectInfo.mpp");

// 设置项目信息
project.Set(Prj.Author, "Author");
project.Set(Prj.LastAuthor, "Last Author");
project.Set(Prj.Revision, 15);
project.Set(Prj.Keywords, "MSP Aspose");
project.Set(Prj.Comments, "Comments");

Console.WriteLine(project.Get(Prj.Author));
Console.WriteLine(project.Get(Prj.LastAuthor));
Console.WriteLine(project.Get(Prj.Revision));
Console.WriteLine(project.Get(Prj.Keywords));
Console.WriteLine(project.Get(Prj.Comments));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


