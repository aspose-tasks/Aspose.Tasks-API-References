---
title: "MPPSaveOptions.WriteFilters"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلاتر عند حفظ مشروع بتنسيق MPP. تشمل بيانات الفلاتر مجموعات Project.TaskFilters و Project.ResourceFilters."
type: docs
weight: 50
url: /ar/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب كتابة بيانات الفلاتر عند حفظ المشروع إلى تنسيق MPP. تشمل بيانات الفلاتر مجموعات Project.TaskFilters و Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## ملاحظات

مدعوم حاليًا لتنسيقات MSP 2010 أو الأحدث.

## الأمثلة

يوضح كيفية إضافة وحفظ فلتر مهمة جديد إلى مشروع MPP.

```csharp
Project project = new Project();

project.TaskFilters.Clear();
project.ResourceFilters.Clear();

var filter = new Filter();
filter.Name = "New Task Filter";
filter.FilterType = ItemType.TaskItem;
filter.ShowInMenu = true;
filter.ShowRelatedSummaryRows = true;

filter.Criteria = new FilterCriteria();

var criteria1 = new FilterCriteria();
criteria1.Field = Field.TaskNumber13;
criteria1.Test = FilterComparisonType.IsLessThan;
criteria1.Values[0] = 34.3D;

filter.Criteria.CriteriaRows.Add(criteria1);
project.TaskFilters.Add(filter);

SimpleSaveOptions options = new MPPSaveOptions() { WriteFilters = true };
project.Save(OutDir + "output_new_filter.mpp", options);
```

### انظر أيضًا

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


