---
title: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 310
url: /ar/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

يمثل تعريف سمة موسعة مرتبطة بمشروع.

نوع ExtendedAttributeDefinition يعرض الأعضاء التالية:
## الخصائص
| الاسم | الوصف |
| :- | :- |
| field_id | يحصل أو يعيّن يتطابق مع معرف المشروع لحقل مخصص.<br/>            استخدم تمثيل السلسلة لثابت من الفئة [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) لتحديد خاصية [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | يحصل على اسم الحقل المخصص. |
| cf_type | يحصل على نوع الحقل المخصص. |
| guid | يحصل أو يعيّن الـ Guid للحقل المخصص. |
| element_type | يحصل أو يعيّن السمة الموسعة مرتبطة<br/>            بمهمة أو مورد أو تعيين. |
| max_multi_values | يحصل أو يضبط الحد الأقصى لعدد القيم التي يمكنك ضبطها في قائمة اختيار. |
| user_def | يحصل أو يضبط قيمة تشير إلى ما إذا كان الحقل المخصص معرفًا من قبل المستخدم. |
| alias | يحصل أو يضبط الاسم المستعار لحقل مخصص. |
| secondary_pid | يحصل أو يضبط معرف العملية الثانوي (PID) لحقل مخصص. |
| auto_roll_down | يحصل أو يضبط قيمة تشير إلى ما إذا كان الانخفاض التلقائي إلى التعيينات مفعلاً. |
| default_guid | يحصل أو يضبط معرف الـ Guid لمدخل جدول البحث الافتراضي. |
| lookup_uid | يحصل على معرف Guid لجدول البحث المرتبط بحقل مخصص. |
| phonetics_alias | يحصل أو يضبط النطق الصوتي للاسم المستعار لحقل مخصص. |
| rollup_type | يحصل أو يضبط طريقة حساب التجميعات. |
| calculation_type | يحصل أو يضبط نوع حساب قيمة السمة المخصصة. |
| summary_rows_calculation_type | يحصل أو يضبط نوع حساب قيمة السمة المخصصة لصفوف الملخص. |
| formula | يحصل أو يضبط الصيغة التي يستخدمها Microsoft Project لملء حقل مهمة مخصص. |
| graphical_indicator | الحصول أو تعيين معلومات مؤشرات رسومية مرتبطة بالخاصية الموسعة.<br/>            ينطبق على تنسيق MPP. |
| restrict_values | الحصول أو تعيين قيمة تشير إلى ما إذا كانت قيم الحقل المخصص مقيدة بالقيم في [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | الحصول أو تعيين طريقة فرز قوائم القيم. القيم هي: 0=تنازلي، 1=تصاعدي. |
| append_new_values | الحصول أو تعيين قيمة تشير إلى ما إذا كانت القيم الجديدة المضافة إلى المشروع تُضاف تلقائيًا إلى القائمة. |
| default | الحصول أو تعيين القيمة الافتراضية في القائمة. |
| value_list | الحصول على List<Value> ValueList. |
| secondary_guid | الحصول أو تعيين المعرف الفريد الثانوي للخاصية الموسعة. |
| parent_project | الحصول على المشروع الأب لـ [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/) المثيل. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| create_extended_attribute() | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن. |
| create_extended_attribute(text_value) | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة النصية المحددة. |
| create_extended_attribute(numeric_value) | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة الرقمية المحددة. |
| create_extended_attribute(date_time_value) | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة التاريخية المحددة. |
| create_extended_attribute(duration_value) | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة الزمنية المحددة. |
| create_extended_attribute(flag_value) | إنشاء خاصية موسعة جديدة بمعرف الحقل الذي يساوي قيمة معرف الحقل لهذا الكائن والقيمة العلم المحددة. |
| create_extended_attribute(lookup_value) | ينشئ سمة موسعة جديدة مرتبطة بالعنصر المحدد [Value](/tasks/python-net/aspose.tasks/value/). |
| create_task_definition(custom_field_type, field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يعرضها Microsoft Project كـ "None".<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [NONE](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في المهام فقط.<br/>            يلزمك تحديد |
| create_task_definition(field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يعرضها Microsoft Project كـ "None".<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [NONE](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في المهام فقط.<br/>            يلزمك تحديد |
| create_resource_definition(custom_field_type, field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يعرضها Microsoft Project كـ "None".<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [NONE](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في الموارد فقط.<br/>            يلزمك تحديد |
| create_resource_definition(field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطة، والتي يعرضها Microsoft Project كـ "None".<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [NONE](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في الموارد فقط.<br/>            يلزمك تحديد |
| create_lookup_task_definition(field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث.<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في المهام فقط.<br/>            يلزمك تحديد |
| create_lookup_task_definition(custom_field_type, field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث.<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في المهام فقط.<br/>            يلزمك تحديد |
| create_lookup_resource_definition(field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث.<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في الموارد فقط.<br/>            يلزمك تحديد |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث.<br/>            لديها [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) يساوي [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) ويمكن استخدامها في الموارد فقط.<br/>            يلزمك تحديد |
| add_lookup_value(value) | يضيف قيمة إلى قائمة البحث الداخلية. هذه طريقة مفضلة للتعامل مع [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | يزيل قيمة من قائمة البحث الداخلية. هذه طريقة مفضلة للتعامل مع [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### انظر أيضًا

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

