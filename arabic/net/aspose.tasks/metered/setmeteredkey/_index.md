---
title: "Metered.SetMeteredKey"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Metered. تعين المفاتيح العامة والخاصة للترخيص القائم على الاستهلاك"
type: docs
weight: 40
url: /ar/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

يحدد المفاتيح العامة والخاصة القابلة للقياس.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| publicKey | سلسلة | المفتاح العام. |
| privateKey | سلسلة | المفتاح الخاص. |

## ملاحظات

إذا قمت بشراء ترخيص metered، يجب استدعاء هذه API عند بدء تشغيل التطبيق، عادةً يكون ذلك كافياً. ومع ذلك، إذا فشل metered في رفع بيانات الاستهلاك خلال فترة 24 ساعة، سيتم تعيين الترخيص إلى حالة التقييم. لتجنب هذه الحالة، يجب عليك فحص حالة الترخيص بانتظام. إذا كانت حالة التقييم، استدعِ هذه API مرة أخرى.

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


