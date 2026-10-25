---
title: "Prj.Manager"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的经理"
type: docs
weight: 450
url: /zh/net/aspose.tasks/prj/manager/
---
## Prj.Manager field

项目的经理。

```csharp
public static readonly Key<string, PrjKey> Manager;
```

## 示例

展示如何读取/写入 Prj.Manager 属性。

```csharp
var project = new Project();

project.Set(Prj.Manager, "Steve");

Console.WriteLine("Manager: " + project.Get(Prj.Manager));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


