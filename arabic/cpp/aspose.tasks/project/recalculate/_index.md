---
title: "Aspose::Tasks::Project::Recalculate طريقة"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks لـ C++"
description: "يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة."
type: docs
weight: 1130
url: /ar/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ البدء المبكر/المتأخر، يحسب الفجوات، حقول العمل والتكلفة مع التحقق الاختياري.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| معامل | الوصف |
| --- | --- |
| validate | إذا كان صحيحًا سيتم تنفيذ التحقق من إعادة الحساب. ما البيانات التي يتم التحقق منها: في الوقت الحالي يتم تنفيذ التحقق الأساسي فقط من نطاقات تواريخ المهمة وروابط المهمة. نطاقات تواريخ المهمة (مثل ActualStart - ActualFinish، EarlyStart - EarlyFinish، إلخ) وكذلك تواريخ روابط المهمة سيتم فحصها وفقًا لمعيار التاريخ الذي يكون فيه تاريخ البدء أقل أو يساوي تاريخ الانتهاء. إذا فشل أي من الشروط المذكورة أعلاه فسيتم رمي استثناء RecalculationValidationException. |

