---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "GraphicalIndicatorCriteria プロパティ。インジケーターが適用される行を示す GraphicalIndicatorCriteriaType 列挙体の値を取得します。"
type: docs
weight: 30
url: /ja/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

[`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 列挙体の値を取得します。この列挙体はインジケーターが適用される行を示します。

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## 例

グラフィカルインジケータ情報の取得方法を示します。

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

### 関連項目

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


