---
title: "GraphicalIndicatorCriteria.RowType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GraphicalIndicatorCriteria 속성. 표시기가 적용되는 행을 나타내는 GraphicalIndicatorCriteriaType 열거형의 값을 가져옵니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks/graphicalindicatorcriteria/rowtype/
---
## GraphicalIndicatorCriteria.RowType property

[`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) 열거형의 값을 가져옵니다. 이 열거형은 표시기가 적용되는 행을 나타냅니다.

```csharp
public GraphicalIndicatorCriteriaType RowType { get; }
```

## 예제

그래픽 지표 정보를 검색하는 방법을 보여줍니다.

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

### 또 보기

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


