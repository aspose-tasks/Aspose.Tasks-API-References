---
title: "Prj.HonorConstraints"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定任务是否遵守其约束日期。"
type: docs
weight: 370
url: /zh/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

确定任务是否遵守其约束日期。

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## 示例

展示如何读取/写入 Prj.HonorConstraints 属性。

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


