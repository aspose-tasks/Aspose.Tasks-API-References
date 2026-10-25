---
title: "الفئة Metered"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Metered. توفر طرقًا لتعيين المفتاح القابل للقياس"
type: docs
weight: 1020
url: /ar/net/aspose.tasks/metered/
---
## Metered class

يوفر طرقًا لتعيين المفتاح المقيس.

```csharp
public class Metered
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Metered](metered/)() | المنشئ الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | يتحقق مما إذا كان المنتج مرخصًا بنجاح باستخدام ترخيص Metered. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | يزيل الترخيص الذي تم إعداده مسبقًا. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | يحدد المفاتيح العامة والخاصة القابلة للقياس. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | يحصل على رصيد الاستهلاك. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | يحصل على حجم ملف الاستهلاك. |

## الأمثلة

في هذا المثال، سيتم محاولة تعيين المفتاح العام والخاص القابل للقياس

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

ملف jar المكوّن:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


