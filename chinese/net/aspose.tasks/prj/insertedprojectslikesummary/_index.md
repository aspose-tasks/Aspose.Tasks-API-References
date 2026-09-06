---
title: "Prj.InsertedProjectsLikeSummary"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定子任务是否被计算为汇总任务"
type: docs
weight: 390
url: /zh/net/aspose.tasks/prj/insertedprojectslikesummary/
---
## Prj.InsertedProjectsLikeSummary field

确定子任务是否被计算为汇总任务。

```csharp
public static readonly Key<NullableBool, PrjKey> InsertedProjectsLikeSummary;
```

## 示例

展示如何读取/写入 Prj.InsertedProjectsLikeSummary 属性。

```csharp
var project = new Project();

project.Set(Prj.InsertedProjectsLikeSummary, true);

Console.WriteLine("Inserted Projects Like Summary: " + project.Get(Prj.InsertedProjectsLikeSummary));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


