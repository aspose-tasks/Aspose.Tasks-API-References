---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraReadOptions 属性。指定用于处理从 XER 格式读取的未定义约束任务的行为。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

指定用于处理从 XER 格式读取的具有未定义约束的任务的行为。

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


