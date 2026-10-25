---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GraphicalIndicatorCriteria 属性。获取 GraphicalIndicatorCriteriaType 枚举的值，该枚举指示指示器适用于哪些行。"
type: docs
weight: 30
url: /zh/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

获取 [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 枚举的值，该枚举指示指示器适用于哪些行。

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## 示例

展示如何检索图形指示器信息。

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

### 另见

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


