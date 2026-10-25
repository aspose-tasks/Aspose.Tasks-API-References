---
title: "Metered.GetConsumptionCredit"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Metered. يحصل على رصيد الاستهلاك"
type: docs
weight: 50
url: /ar/net/aspose.tasks/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

يحصل على رصيد الاستهلاك.

```csharp
public static decimal GetConsumptionCredit()
```

### قيمة الإرجاع

يعيد عدد نقاط الائتمان المستهلكة.

## الأمثلة

يعرض كيفية استخدام <see cref=\"Aspose.Tasks.Metered\" /> نوع الترخيص مع Aspose.Tasks.

```csharp
// لنستخدم ترخيصًا مقيسًا (انظر https://purchase.aspose.com/faqs/licensing/metered)
// تعيين ترخيص مقيس
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// العمل مع المشروع...
// ...

// يمكننا الحصول على الرصيد الحالي واستهلاك البايتات.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // تسجيل الاستثناء
}

// مؤخرًا يمكن للمستخدم إعادة تعيين الترخيص المقيس وإيقاف عدّ البايتات
metered.ResetMeteredKey();
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


