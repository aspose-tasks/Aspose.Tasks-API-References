---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。计算挣值的默认方法"
type: docs
weight: 310
url: /zh/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

计算挣值的默认方法。

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## 示例

展示如何读取/写入 Prj.EarnedValueMethod 属性。

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


