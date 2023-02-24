---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Aspose.Tasks لمرجع .NET API
description: ExtendedAttributeDefinition طريقة. إضافة قيمة إلى قائمة البحث الداخلي. هذه طريقة مفضلة للتلاعب بامتدادValueList .
type: docs
weight: 290
url: /ar/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

إضافة قيمة إلى قائمة البحث الداخلي. هذه طريقة مفضلة للتلاعب بامتداد[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| value | Value | القيمة المراد إضافتها إلى البحث. |

### ملاحظات

تعمل هذه الطريقة فقط مع ملفات[`ExtendedAttributeDefinition`](../) الحالات التي لها[`CalculationType`](../calculationtype/) يساويLookup .

### أمثلة

استخدم هذا الرمز لإضافة قيمة جديدة إلى قائمة البحث:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### أنظر أيضا

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* مساحة الاسم [Aspose.Tasks](../../extendedattributedefinition/)
* المجسم [Aspose.Tasks](../../../)


