---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "GraphicalIndicatorCriteria プロパティ。IsWithin および IsNotWithin の比較タイプの場合に、拡張属性の値をテストするために使用される第2の値を取得します。"
type: docs
weight: 60
url: /ja/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

'IsWithin' および 'IsNotWithin' の比較タイプの場合に、拡張属性の値をテストするために使用される第2の値を取得します。

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


