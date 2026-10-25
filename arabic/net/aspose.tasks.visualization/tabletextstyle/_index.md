---
title: "الفئة TableTextStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.TableTextStyle. تمثل نمط نص في جدول العرض"
type: docs
weight: 3370
url: /ar/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

يمثل نمط النص في جدول العرض.

```csharp
public class TableTextStyle : TextStyle
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | ينشئ مثيلاً جديداً للفئة `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | ينشئ مثيلاً جديداً للفئة `TableTextStyle` باستخدام الخط المحدد. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | ينشئ مثيلاً جديداً للفئة `TableTextStyle` بإعدادات الخط الافتراضية والنمط المحدد للخط. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | ينشئ مثيلاً جديداً للفئة `TableTextStyle` بحجم الخط المحدد والنمط المحدد للخط. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | يحصل أو يعيّن لون الخلفية لنمط النص. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | يحصل أو يعيّن نمط الخلفية لنمط النص. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | يحصل أو يعيّن لون النص. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | يحصل أو يعيّن الحقل الذي سيُطبق عليه النمط. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | يحصل أو يعيّن خط نمط النص. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | يرجع قيمة من تعداد [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | يحصل على معرف فريد للصف. يُرجع -1 إذا كان النمط سيُطبق على جميع صفوف العرض. |

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

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


