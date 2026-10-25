---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。用于显示进度或计算挣值总计的状态日期。状态日期与当前日期（今天的日期）相同，除非指定了不同的状态日期"
type: docs
weight: 690
url: /zh/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

用于显示进度或计算挣值总计的状态日期。除非指定了其他状态日期，否则状态日期与当前日期（今天的日期）相同。

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## 示例

展示如何读取/写入 Prj.StatusDate 属性。

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


