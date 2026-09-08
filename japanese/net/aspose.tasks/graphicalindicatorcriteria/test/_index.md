---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "GraphicalIndicatorCriteria プロパティ。拡張属性の値と Values の比較タイプを取得します。これはグラフィカルインジケーターの適用基準として機能します。FilterComparisonType"
type: docs
weight: 40
url: /ja/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

拡張属性の値と Values の比較タイプを取得します。これはグラフィカルインジケーターの適用基準として機能します。[`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


