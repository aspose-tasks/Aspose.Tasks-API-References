---
title: "ResourceViewColumn.GetColumnText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceViewColumn. تحول المورد الحالي إلى نص العمود"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

يحوّل المورد الحالي إلى نص العمود.

```csharp
public string GetColumnText(Resource resource)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| المورد | المورد | المورد الحالي. |

### قيمة الإرجاع

نص العمود.

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


