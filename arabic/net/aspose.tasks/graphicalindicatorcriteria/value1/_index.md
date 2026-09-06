---
title: "GraphicalIndicatorCriteria.Value1"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GraphicalIndicatorCriteria. تحصل على القيمة المستخدمة لاختبار قيمة السمات الموسعة"
type: docs
weight: 50
url: /ar/net/aspose.tasks/graphicalindicatorcriteria/value1/
---
## GraphicalIndicatorCriteria.Value1 property

يحصل على القيمة المستخدمة لاختبار قيمة السمة الموسعة.

```csharp
public GraphicalIndicatorCriteriaValue Value1 { get; }
```

## الأمثلة

يوضح كيفية استرجاع معلومات المؤشرات الرسومية.

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

### انظر أيضًا

* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


