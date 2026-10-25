---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceViewColumn yapıcı. ResourceViewColumn sınıfının yeni bir örneğini başlatır"
type: docs
weight: 10
url: /tr/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

[`ResourceViewColumn`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Sütunun adı. |
| genişlik | Int32 | Sütunun piksel cinsinden genişliği. |
| dönüştürücü | ResourceToColumnTextConverter | Kaynak verilerini sütun metnine dönüştüren dönüştürücü. |
| alan | Alan | Sütun alanı. |

## Örnekler

Dışa aktarılacak kaynak görünüm sütunlarını nasıl ekleyeceğinizi gösterir.

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

// sütunlar üzerinde yinele
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

### Ayrıca Bakınız

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

[`ResourceViewColumn`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | Dize | Sütunun adı. |
| genişlik | Int32 | Sütunun piksel cinsinden genişliği. |
| dönüştürücü | ResourceToColumnTextConverter | Kaynak verilerini sütun metnine dönüştüren dönüştürücü. |

## Örnekler

Dışa aktarılacak kaynak görünüm sütunlarını nasıl ekleyeceğinizi gösterir.

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

// sütunlar üzerinde yinele
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

### Ayrıca Bakınız

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

[`ResourceViewColumn`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public ResourceViewColumn(int width, Field field)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| genişlik | Int32 | Sütun genişliği piksel cinsinden. |
| alan | Alan | Sütun alanı. |

## Örnekler

Dışa aktarılacak kaynak görünüm sütunlarını nasıl ekleyeceğinizi gösterir.

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

// sütunlar üzerinde yinele
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

### Ayrıca Bakınız

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


