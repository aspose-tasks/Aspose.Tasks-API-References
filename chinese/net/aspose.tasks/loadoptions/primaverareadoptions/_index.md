---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LoadOptions 属性。获取或设置 PrimaveraReadOptions 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为"
type: docs
weight: 60
url: /zh/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

获取或设置 [`PrimaveraReadOptions`](../../primaverareadoptions/) 类的指定实例，可用于自定义加载 Primavera 格式（Primavera P6 XER 或 Primavera P6 Xml）的行为。

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


