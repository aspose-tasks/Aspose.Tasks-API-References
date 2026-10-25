---
title: "类 PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.PrimaveraReadOptions 类。允许在读取 Primavera Xml 或 Primavera Xer 文件时指定其他选项。"
type: docs
weight: 1370
url: /zh/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

允许在读取 Primavera Xml 或 Primavera Xer 文件时指定附加选项。

```csharp
public class PrimaveraReadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | 初始化 `PrimaveraReadOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | 获取或设置一个标志，指定是否应保留实体的原始唯一标识符。 |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | 获取或设置要从包含多个项目的文件中读取的项目 UID。 |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | 获取或设置一个标志，指定是否应加载基线项目。默认值为 true。 |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | 指定用于处理从 XER 格式读取的具有未定义约束的任务的行为。 |

## 示例

展示如何从包含多个项目的 Primavera XML 或 Primavera XER 文件中读取项目。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// 返回具有特殊 UID 的项目
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


