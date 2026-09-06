---
title: "Prj.BaselineForEarnedValue"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。用于计算方差值的特定基准"
type: docs
weight: 80
url: /zh/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

用于计算差异值的特定基线。

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## 示例

展示如何读取/写入 Prj.BaselineForEarnedValue 属性。

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


