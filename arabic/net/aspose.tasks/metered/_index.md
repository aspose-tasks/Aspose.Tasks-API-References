---
title: Class Metered
second_title: Aspose.Tasks لمرجع .NET API
description: Aspose.Tasks.Metered فصل. يوفر طرقًا لتعيين المفتاح المقنن .
type: docs
weight: 890
url: /ar/net/aspose.tasks/metered/
---
## Metered class

يوفر طرقًا لتعيين المفتاح المقنن .

```csharp
public class Metered
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## طُرق

| اسم | وصف |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | يزيل ترخيص الإعداد السابق . |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | مجموعات المفاتيح العامة والخاصة التي تم قياسها. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | يحصل على ائتمان الاستهلاك. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | الحصول على حجم ملف الاستهلاك. |

### أمثلة

في هذا المثال ، ستُبذل محاولة لتعيين المفتاح العام والخاص المحسوب

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

ملف جرة المكون:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks/)
* المجسم [Aspose.Tasks](../../)


