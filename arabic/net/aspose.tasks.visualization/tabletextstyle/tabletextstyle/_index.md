---
title: "TableTextStyle.TableTextStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ TableTextStyle. يهيئ نسخة جديدة من الفئة TableTextStyle"
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

يهيئ نسخة جديدة من الفئة [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowUid | Int32 | معرف فريد للصف المحدد. |

## الأمثلة

يوضح كيفية تخصيص أنماط نص الجدول التي تُستخدم لتنسيق عناصر نصية مختلفة في المشروع.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// تعيين نمط نص اسم المهمة الأولى
var style1 = new TableTextStyle(1);
// تعيين حقل سيتم تطبيق النمط عليه.
style1.Field = Field.TaskName;
// تعيين <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> لنمط النص.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// تعيين الحجم بالنقاط لخط نمط النص.

// تعيين نمط نص مدة المهمة الثانية
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // تعيين علامة تشير إلى أنه يجب كتابة بيانات العرض
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### انظر أيضًا

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`TableTextStyle`](../) باستخدام الخط المحدد.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowUid | Int32 | معرف فريد للصف المحدد. |
| font | FontDescriptor | خط يُستند إليه النمط النصي. |

### انظر أيضًا

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

يهيئ نسخة جديدة من الفئة [`TableTextStyle`](../) باستخدام حجم الخط المحدد ونمط الخط.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowUid | Int32 | معرف فريد للصف المحدد. |
| fontSize | Single | حجم الخط الذي يُستند إليه النمط النصي. |
| fontStyle | FontStyles | نمط الخط الذي يُستند إليه النمط النصي. |

### انظر أيضًا

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

يهيئ نسخة جديدة من الفئة [`TableTextStyle`](../) باستخدام إعدادات الخط الافتراضية والنمط المحدد للخط.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| rowUid | Int32 | معرف فريد للصف المحدد. |
| fontStyle | FontStyles | نمط الخط الذي يُستند إليه النمط النصي. |

### انظر أيضًا

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


