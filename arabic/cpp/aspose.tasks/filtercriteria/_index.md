---
title: "فئة Aspose::Tasks::FilterCriteria"
linktitle: "FilterCriteria"
articleTitle: "FilterCriteria"
second_title: "Aspose.Tasks لـ C++"
description: "يحدد المعايير التي يجب أن تفي بها المهام أو الموارد لتُعرض في عرض MSP."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/filtercriteria/
---

## FilterCriteria class

يحدد المعايير التي يجب أن تفي بها المهام أو الموارد لتُعرض في عرض MSP.

## الطرق

| الاسم | الوصف |
| --- | --- |
| [get_CriteriaRows](./get_criteriarows/) | يسترجع قائمة صفوف FilterCriteria الفرعية. إذا كان الفلتر يحتوي على أكثر من صف معيار واحد، فإن تأثير عامل And هو أن المعايير لكلا الصفين يجب أن تتحقق لكي تُعرض المهمة أو المورد نتيجة لهذا الفلتر. تأثير عامل Or هو أن المعايير لصف واحد أو الآخر يجب أن تتحقق. |
| [get_Field](./get_field/) | يسترجع حقلًا لتغييره. |
| [get_Operation](./get_operation/) | يسترجع المعيار المحدد بـ FieldName و Test و Value ويُظهر علاقته بالمعايير الأخرى في الفلتر. |
| [get_Test](./get_test/) | يحصل على نوع المقارنة التي تتم بين FieldName و Value والتي تعمل كمعايير اختيار للمرشح. FilterComparisonType |
| [get_Values](./get_values/) | يحصل على قيم الكائن للمقارنة مع قيمة الحقل المحدد بـ FieldName. |
| [IsFieldValue](./isfieldvalue/) | يحصل على ما إذا كانت القيمة اليمنى لـ FilterCriteria إشارة إلى حقل، وليس قيمة ثابتة. |
| [set_Field](./set_field/) | يضبط حقلًا للتغيير. |
| [set_Operation](./set_operation/) | يضبط المعيار المحدد بـ FieldName و Test و Value ويتعلق بمعايير أخرى في المرشح. |
| [set_Test](./set_test/) | يضبط نوع المقارنة التي تتم بين FieldName و Value والتي تعمل كمعايير اختيار للمرشح. FilterComparisonType |
| [SetValueField](./setvaluefield/) | يضبط الحقل الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName. |
| [ToString](./tostring/) | يرجع تمثيلًا نصيًا لنسخة من فئة FilterCriteria. |

