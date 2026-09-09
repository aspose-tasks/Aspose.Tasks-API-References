---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrimaveraSaveOptions özelliği. Kaynakların özet görevlerine atamalarının dışa aktarma sırasında atlanıp atlanmayacağını gösteren bir değeri alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Açıklamalar

Primavera yazılımı, kaynakların özet (WBS) görevlerine atamalarını desteklemez. Bu nedenle, bu tür atamaların dışa aktarımı Primavera modeline göre geçersiz bir dosyaya yol açabilir. True ise, özet görevlere yapılan atamalar dışa aktarım sırasında atlanır. False (varsayılan değer) ise, dışa aktarım sırasında bir özet göreve atama ile karşılaşılırsa bir istisna fırlatılır.

## Örnekler

SkipSummaryAssignments bayrağının nasıl kullanılacağını gösterir

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera, kaynakların özet görevlere atamalarını desteklemez.
// Bu tür atamaların Primavera formatına dışa aktarılması, Primavera'ya içe aktarılamayan dosyalara neden olabilir.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Ayrıca Bakınız

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


