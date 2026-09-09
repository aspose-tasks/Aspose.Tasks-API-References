---
title: "Sınıf ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.ResourceViewColumn sınıfı. ResourceUsage görünümü ve ResourceSheet görünümünde kullanılan Projects görünüm sınıfı."
type: docs
weight: 3350
url: /tr/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

ResourceUsage görünümü ve ResourceSheet görünümünde kullanılan projenin görünüm sınıfı.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | `ResourceViewColumn` sınıfının yeni bir örneğini başlatır. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | `ResourceViewColumn` sınıfının yeni bir örneğini başlatır. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | `ResourceViewColumn` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Sütun alanı. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Sütun adını alır. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Metnin hizalamasını alır veya ayarlar ([`HorizontalStringAlignment`](../horizontalstringalignment/) enum değerlerinden biri olabilir). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Sütun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır veya ayarlar. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Sütun genişliğini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Geçerli kaynağı sütun metnine dönüştürür. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


