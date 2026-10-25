---
title: "TaskCollection"
second_title: "Aspose.Tasks لـ Python عبر .NET مرجع API"
description: 
type: docs
weight: 1140
url: /ar/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

يمثّل مجموعة من كائنات [Task](/tasks/python-net/aspose.tasks/task/).

نوع TaskCollection يعرض الأعضاء التالية:
## الخصائص
| الاسم | الوصف |
| :- | :- |
| parent_project | يحصل على المشروع الأب لكائن TaskCollection. |
## الطرق
| الاسم | الوصف |
| :- | :- |
| add() | أضف المهمة المحددة إلى نسخة من الفئة [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) .<br/>            إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحساب الحقول التابعة مثل الفجوات، والعمل، وحقول التكلفة، والمعرفات ومستويات المخطط).<br/>            إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، مستوى المخطط وأرقام المخطط تلقائيًا.<br/>            إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا<br/>            (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، والعمل، وحقول التكلفة، ويعيد حساب المعرفات ومستويات المخطط). |
| add(task_name) | يضيف مهمة جديدة إلى مجموعة مهام الأطفال. |
| add(task_name, before_task_id) |  |
| add(parameters) | يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس مستوى المخطط. |
| to_list() | يحول كائن TaskCollection إلى قائمة من كائنات [Task](/tasks/python-net/aspose.tasks/task/). |
| get_by_uid(uid) | يعيد مهمة بالمعرف الفريد (Uid) المحدد يكون سلفها المهمة الأب لهذه المجموعة. |
| get_by_id(id) | يعيد مهمة بالمعرف (Id) المحدد يكون سلفها المهمة الأب لهذه المجموعة. |

### انظر أيضًا

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

