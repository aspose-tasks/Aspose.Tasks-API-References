---
title: "Project.SetBaseline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة المشروع. حفظ حقول الخط الأساسي إلى الخط الأساسي المحدد لكامل المشروع"
type: docs
weight: 1250
url: /ar/net/aspose.tasks/project/setbaseline/
---
## SetBaseline(BaselineType) {#setbaseline}

يحفظ حقول الخط الأساسي إلى الخط الأساسي المحدد لكامل المشروع.

```csharp
public void SetBaseline(BaselineType baselineType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| baselineType | BaselineType | نوع الخط الأساسي لحفظ بيانات الخط الأساسي إليه. |

## الأمثلة

يعرض كيفية إنشاء خطوط أساسية لمشروع كامل.

```csharp
var project = new Project();

// إضافة مهام
project.RootTask.Children.Add("Task");
project.RootTask.Children.Add("Task2");

// تعيين خط أساسي للمهام المحددة
project.SetBaseline(BaselineType.Baseline);
```

### انظر أيضًا

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SetBaseline(BaselineType, IEnumerable&lt;Task&gt;) {#setbaseline_1}

يحفظ حقول الخط الأساسي إلى الخط الأساسي المحدد للمهام المحددة.

```csharp
public void SetBaseline(BaselineType baselineType, IEnumerable<Task> taskCollection)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| baselineType | BaselineType | نوع الخط الأساسي لحفظ بيانات الخط الأساسي إليه. |
| taskCollection | IEnumerable`1 | قائمة المهام لحفظ بيانات الخط الأساسي لها. |

## الأمثلة

يعرض كيفية إنشاء خطوط أساسية محددة لمهام معينة.

```csharp
var project = new Project();

// إضافة مهام
var task = project.RootTask.Children.Add("Task");
var task2 = project.RootTask.Children.Add("Task2");

// تعيين خط أساسي للمهام المحددة
project.SetBaseline(BaselineType.Baseline, new[] { task, task2 });
```

### انظر أيضًا

* enum [BaselineType](../../baselinetype/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


