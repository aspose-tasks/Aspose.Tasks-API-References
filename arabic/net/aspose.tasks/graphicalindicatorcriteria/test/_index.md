---
title: "GraphicalIndicatorCriteria.Test"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GraphicalIndicatorCriteria. تحصل على نوع المقارنة التي تُجرى بين قيمة السمات الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي. FilterComparisonType"
type: docs
weight: 40
url: /ar/net/aspose.tasks/graphicalindicatorcriteria/test/
---
## GraphicalIndicatorCriteria.Test property

تحصل على نوع المقارنة التي تُجرى بين قيمة السمة الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي. [`FilterComparisonType`](../../filtercomparisontype/)

```csharp
public FilterComparisonType Test { get; }
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

* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


