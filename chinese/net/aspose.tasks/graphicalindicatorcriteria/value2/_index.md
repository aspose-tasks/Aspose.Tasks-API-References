---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks for .NET API 参考"
description: "GraphicalIndicatorCriteria 属性。获取在 IsWithin 和 IsNotWithin 比较类型情况下用于测试扩展属性值的第二个值"
type: docs
weight: 60
url: /zh/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

获取在 'IsWithin' 和 'IsNotWithin' 比较类型情况下用于测试扩展属性值的第二个值。

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


