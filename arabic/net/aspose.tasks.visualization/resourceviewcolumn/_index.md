---
title: "الفئة ResourceViewColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Visualization.ResourceViewColumn. فئة عرض المشاريع المستخدمة في عرض ResourceUsage وعرض ResourceSheet"
type: docs
weight: 3350
url: /ar/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

فئة عرض المشروع المستخدمة في عرض ResourceUsage وعرض ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | ينشئ مثيلاً جديداً للفئة `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | ينشئ مثيلاً جديداً للفئة `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | ينشئ مثيلاً جديداً للفئة `ResourceViewColumn`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | حقل العمود. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | يحصل على اسم العمود. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | يحصل أو يعيّن محاذاة النص (يمكن أن تكون أحد قيم تعداد [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | يحصل على عرض العمود. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | يحوّل المورد الحالي إلى نص العمود. |

## الأمثلة

يوضح كيفية إضافة أعمدة عرض الموارد لتصديرها.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// التكرار عبر الأعمدة
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### انظر أيضًا

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


