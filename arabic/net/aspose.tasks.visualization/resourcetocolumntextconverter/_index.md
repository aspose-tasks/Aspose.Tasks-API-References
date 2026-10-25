---
title: "المندوب ResourceToColumnTextConverter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "محول بيانات الموارد إلى سلسلة الأعمدة"
type: docs
weight: 3340
url: /ar/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

محول بيانات المورد إلى سلسلة العمود.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المورد | المورد | المورد الحالي. |

### قيمة الإرجاع

بيانات السلسلة للعمود.

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

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


