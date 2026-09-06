---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraReadOptions 属性。获取或设置一个标志，指定是否应保留实体的原始唯一标识符。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

获取或设置一个标志，指定是否应保留实体的原始唯一标识符。

```csharp
public bool PreserveUids { get; set; }
```

## 示例

展示如何使用 &lt;see cref=\"LoadOptions\" /&gt; 加载具有指定 Id 的 Primavera 项目。

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// 设置 Primavera 读取选项
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// 处理项目...
```

### 另见

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


