---
title: "类 ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.ResourceViewColumn 类。项目视图类，用于 ResourceUsage 视图和 ResourceSheet 视图。"
type: docs
weight: 3350
url: /zh/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

在 ResourceUsage 视图和 ResourceSheet 视图中使用的项目视图类。

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | 初始化 `ResourceViewColumn` 类的新实例。 |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | 初始化 `ResourceViewColumn` 类的新实例。 |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | 初始化 `ResourceViewColumn` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | 列字段。[`Field`](./field/)。 |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 获取列名。 |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 获取或设置文本的对齐方式（可以是 [`HorizontalStringAlignment`](../horizontalstringalignment/) 枚举的其中一个值）。 |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 获取或设置回调，可用于自定义列单元格的外观。 |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 获取列宽。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | 将当前资源转换为列文本。 |

## 示例

展示如何添加要导出的资源视图列。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// 遍历列
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### 另见

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


