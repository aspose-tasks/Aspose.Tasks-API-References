---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks لمرجع .NET API
description: TaskLink ملكية. الحصول على مدة التأخير أو تعيينها  اعتمادًا على تنسيق LagFormat .
type: docs
weight: 50
url: /ar/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

الحصول على مدة التأخير أو تعيينها ، اعتمادًا على تنسيق LagFormat .

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | عند محاولة تعيين قيمة TaskLinks حيث يكون LagFormat هو TimeUnitType.Percent. |

### ملاحظات

يمكن أن يكون تأخر الارتباط قيمة النسبة المئوية (تنسيق LagFormat هو TimeUnitType.Percent) . في هذه الحالة يتم احتساب المدة كنسبة مئوية من مدة PredTask . وإلا فإن الطريقة تُرجع قيمة TimeSpan التي تمثل تأخر TaskLink.

### أنظر أيضا

* class [TaskLink](../)
* مساحة الاسم [Aspose.Tasks](../../tasklink/)
* المجسم [Aspose.Tasks](../../../)


