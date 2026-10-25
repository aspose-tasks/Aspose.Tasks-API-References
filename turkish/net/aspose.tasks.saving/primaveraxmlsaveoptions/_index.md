---
title: "Sınıf PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.PrimaveraXmlSaveOptions sınıfı. Projeyi Primavera xml formatında kaydederken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 2160
url: /tr/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Projeyi Primavera xml formatına kaydederken ek seçenekleri belirtmeye izin verir.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | `PrimaveraXmlSaveOptions` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Kök görevin kaydedilip kaydedilmeyeceğini gösteren bir değeri alır veya ayarlar. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |

## Örnekler

Primavera XML dosyasına nasıl dışa aktarılacağını gösterir.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


