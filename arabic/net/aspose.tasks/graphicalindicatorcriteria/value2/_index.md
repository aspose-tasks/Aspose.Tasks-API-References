---
title: "GraphicalIndicatorCriteria.Value2"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GraphicalIndicatorCriteria. تحصل على القيمة الثانية المستخدمة لاختبار قيمة السمات الموسعة في حالة أنواع المقارنة IsWithin و IsNotWithin"
type: docs
weight: 60
url: /ar/net/aspose.tasks/graphicalindicatorcriteria/value2/
---
## GraphicalIndicatorCriteria.Value2 property

يحصل على القيمة الثانية المستخدمة لاختبار قيمة السمة الموسعة في حالة أنواع المقارنة 'IsWithin' و 'IsNotWithin'.

```csharp
public GraphicalIndicatorCriteriaValue Value2 { get; }
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


