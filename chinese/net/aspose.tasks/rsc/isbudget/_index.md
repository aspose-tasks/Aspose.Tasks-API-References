---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。确定工作材料或成本资源是否为预算资源"
type: docs
weight: 380
url: /zh/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

确定工作、材料或成本资源是否为预算资源。

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## 示例

展示如何读取/写入 Rsc.IsBudget 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


