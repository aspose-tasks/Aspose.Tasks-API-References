---
title: "فئة Aspose::Tasks::Metered"
linktitle: "مقاسة"
articleTitle: "مقاسة"
second_title: "Aspose.Tasks لـ C++"
description: "يوفر طرقًا لتعيين المفتاح المقنن."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/metered/
---

## Metered class

يوفر طرقًا لتعيين المفتاح المقنن.

في هذا المثال، سيتم محاولة تعيين المفتاح العام والخاص المقاس <ms>

```cpp
[C#]
 
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
 
 
[Visual Basic]
 
Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

</ms> <java> ملف jar للمكوّن:

```cpp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

</java>

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetConsumptionCredit](./getconsumptioncredit/) | يحصل على رصيد الاستهلاك. |
| [GetConsumptionQuantity](./getconsumptionquantity/) | يحصل على حجم ملف الاستهلاك. |
| [IsLicensed](./islicensed/) | يتحقق مما إذا كان المنتج مرخصًا بنجاح باستخدام ترخيص Metered. |
| [ResetMeteredKey](./resetmeteredkey/) | يزيل الترخيص المُعد مسبقًا. |
| [SetMeteredKey](./setmeteredkey/) | يضبط المفاتيح العامة والخاصة المقاسة. |

