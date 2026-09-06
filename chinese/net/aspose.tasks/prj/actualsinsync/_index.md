---
title: "Prj.ActualsInSync"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否已将所有实际工作与项目同步"
type: docs
weight: 10
url: /zh/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

确定是否已将所有实际工作与项目同步。

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## 示例

展示如何读取/写入 Prj.ActualsInSync 属性。

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


