---
title: "Delege ResourceToColumnTextConverter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Kaynak verilerini sütun dizesine dönüştüren dönüştürücü"
type: docs
weight: 3340
url: /tr/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

Kaynağın verisini sütunun dizesine dönüştüren dönüştürücü.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Kaynak | Geçerli kaynak. |

### Dönüş Değeri

Sütun için dize verisi.

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

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


