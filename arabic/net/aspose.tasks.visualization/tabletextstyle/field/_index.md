---
title: "TableTextStyle.Field"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TableTextStyle. تحصل أو تعين حقلًا يتم تطبيق النمط عليه. Field"
type: docs
weight: 20
url: /ar/net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

تحصل أو تعين حقلًا يتم تطبيق النمط عليه. `Field`.

```csharp
public Field Field { get; set; }
```

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

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


