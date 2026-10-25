---
title: "TaskLink.LinkLagTimeSpan"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskLink. تحصل أو تعين مدة التأخير حسب LagFormat"
type: docs
weight: 50
url: /ar/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

يحصل أو يعيّن مدة التأخير، اعتمادًا على LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | عند محاولة تعيين القيمة لـ TaskLinks حيث يكون LagFormat هو TimeUnitType.Percent. |

## ملاحظات

يمكن أن يكون تأخير الرابط قيمة نسبية (LagFormat هو TimeUnitType.Percent). في هذه الحالة يتم حساب المدة كنسبة مئوية من مدة PredTask. وإلا فإن الطريقة تُرجع قيمة TimeSpan تمثل تأخير TaskLink.

### انظر أيضًا

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


