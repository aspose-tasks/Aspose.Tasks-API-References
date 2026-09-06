---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ResourceViewColumn. يهيئ مثيلاً جديداً من الفئة ResourceViewColumn"
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

تهيئ مثيلاً جديداً من الفئة [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| محول | ResourceToColumnTextConverter | محول بيانات المورد إلى نص العمود. |
| حقل | حقل | حقل العمود. |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

تهيئ مثيلاً جديداً من الفئة [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| محول | ResourceToColumnTextConverter | محول بيانات المورد إلى نص العمود. |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

تهيئ مثيلاً جديداً من الفئة [`ResourceViewColumn`](../).

```csharp
public ResourceViewColumn(int width, Field field)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العرض | Int32 | عرض العمود بالبكسل. |
| حقل | حقل | حقل العمود. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


