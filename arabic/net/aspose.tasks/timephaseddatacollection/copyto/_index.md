---
title: TimephasedDataCollection.CopyTo
second_title: Aspose.Tasks لمرجع .NET API
description: TimephasedDataCollection طريقة. ينسخ عناصر ملفTimephasedDataCollection إلىArray  بدءًا من ملفArray الفهرس .
type: docs
weight: 90
url: /ar/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

ينسخ عناصر ملف[`TimephasedDataCollection`](../) إلىArray ، بدءًا من ملفArray الفهرس .

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| array | TimephasedData[] | أحادي البعدArray هذه هي وجهة العناصر المنسوخة من[`TimephasedDataCollection`](../) . ملفArray يجب أن يكون الفهرسة الصفرية. |
| arrayIndex | Int32 | المؤشر الصفري في*array* عنده يبدأ النسخ. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *array* باطل. |
| ArgumentOutOfRangeException | *arrayIndex* أقل من 0. |
| ArgumentException | عدد العناصر في المصدر[`TimephasedDataCollection`](../) أكبر من المساحة المتوفرة من*arrayIndex* إلى نهاية الوجهة*array* . |

### أنظر أيضا

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* مساحة الاسم [Aspose.Tasks](../../timephaseddatacollection/)
* المجسم [Aspose.Tasks](../../../)


