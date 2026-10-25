---
title: "Prj.SpreadPercentComplete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否将完成百分比分配到状态日期"
type: docs
weight: 670
url: /zh/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

确定完成百分比是否分摊到状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## 示例

展示如何读取/写入 Prj.SpreadPercentComplete 属性。

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


