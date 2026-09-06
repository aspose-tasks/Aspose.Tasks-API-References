---
title: "GraphicalIndicatorCriteria.GraphicalIndicatorCriteria"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ GraphicalIndicatorCriteria. يخلق مثيلاً جديدًا لنوع GraphicalIndicatorCriteria"
type: docs
weight: 10
url: /ar/net/aspose.tasks/graphicalindicatorcriteria/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) {#constructor_1}

يخلق مثيلاً جديدًا للنوع [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value1, 
    GraphicalIndicatorCriteriaValue value2)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | قيمة enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) التي تحدد الصفوف التي يُطبق عليها المؤشر |
| test | FilterComparisonType | قيمة [`FilterComparisonType`](../../filtercomparisontype/) التي تشير إلى نوع المقارنة التي يجريها المعيار. |
| imageIndex | Int32 | فهرس الصورة التي تُعرض عندما يفي الحقل بالمعايير |
| value1 | GraphicalIndicatorCriteriaValue | القيم المستخدمة في فحص الشرط. |
| value2 | GraphicalIndicatorCriteriaValue | القيمة الثانية (نهاية الفاصل) المستخدمة في فحص الشرط في حالة شروط 'IsWithin' و 'IsNotWithing' |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | يُرمى عندما يتم تمرير تركيبة غير صحيحة من الوسائط إلى المنشئ. |

### انظر أيضًا

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)

---

## GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) {#constructor}

يخلق مثيلاً جديدًا للنوع [`GraphicalIndicatorCriteria`](../).

```csharp
public GraphicalIndicatorCriteria(GraphicalIndicatorCriteriaType rowType, 
    FilterComparisonType test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowType | GraphicalIndicatorCriteriaType | قيمة enum [`GraphicalIndicatorCriteriaType`](../../graphicalindicatorcriteriatype/) التي تحدد الصفوف التي يُطبق عليها المؤشر |
| test | FilterComparisonType | قيمة [`FilterComparisonType`](../../filtercomparisontype/) التي تشير إلى نوع المقارنة التي يجريها المعيار. |
| imageIndex | Int32 | فهرس الصورة التي تُعرض عندما يفي الحقل بالمعايير |
| value | GraphicalIndicatorCriteriaValue | القيمة المستخدمة في فحص الشرط. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | يُرمى عندما يتم تمرير تركيبة غير صحيحة من الوسائط إلى المنشئ. |
| ArgumentException | عند تمرير قيمة IsWithin أو IsNotWithing إلى وسيط الاختبار. |

### انظر أيضًا

* enum [GraphicalIndicatorCriteriaType](../../graphicalindicatorcriteriatype/)
* enum [FilterComparisonType](../../filtercomparisontype/)
* class [GraphicalIndicatorCriteriaValue](../../graphicalindicatorcriteriavalue/)
* class [GraphicalIndicatorCriteria](../)
* namespace [Aspose.Tasks](../../graphicalindicatorcriteria/)
* assembly [Aspose.Tasks](../../../)


