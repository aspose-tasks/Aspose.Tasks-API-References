---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "Aspose.Tasks for .NET API 참조"
description: "GraphicalIndicatorCriteria 속성. IsWithin 및 IsNotWithin 비교 유형의 경우 확장 속성 값을 테스트하는 데 사용되는 두 번째 값을 가져옵니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

'IsWithin' 및 'IsNotWithin' 비교 유형의 경우 확장 속성 값을 테스트하는 데 사용되는 두 번째 값을 가져옵니다.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


