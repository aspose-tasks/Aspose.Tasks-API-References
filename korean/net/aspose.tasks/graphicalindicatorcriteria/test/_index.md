---
title: "GraphicalIndicatorCriteria.Test"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GraphicalIndicatorCriteria 속성. 확장 속성 값과 값 사이의 비교 유형을 가져옵니다. 이 비교는 그래픽 표시기의 적용 기준으로 작동합니다. FilterComparisonType"
type: docs
weight: 40
url: /ko/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

확장 속성 값과 값 사이의 비교 유형을 가져옵니다. 이 비교는 그래픽 표시기의 적용 기준으로 작동합니다. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


