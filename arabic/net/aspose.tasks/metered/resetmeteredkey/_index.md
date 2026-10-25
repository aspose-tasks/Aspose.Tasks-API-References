---
title: "Metered.ResetMeteredKey"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Metered. تزيل الترخيص المُعد مسبقاً"
type: docs
weight: 30
url: /ar/net/aspose.tasks/metered/resetmeteredkey/
---
## Metered.ResetMeteredKey method

يزيل الترخيص الذي تم إعداده مسبقًا.

```csharp
public void ResetMeteredKey()
```

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


