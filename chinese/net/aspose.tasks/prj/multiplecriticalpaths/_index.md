---
title: "Prj.MultipleCriticalPaths"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否计算多个关键路径"
type: docs
weight: 530
url: /zh/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

确定是否计算多条关键路径。

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## 示例

展示如何读取/写入 Prj.MultipleCriticalPaths 属性。

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


