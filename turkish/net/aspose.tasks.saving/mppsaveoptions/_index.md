---
title: "Sınıf MPPSaveOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.MPPSaveOptions sınıfı. Proje verilerini MPP'ye kaydederken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 2050
url: /tr/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Proje verilerini MPP'ye kaydederken ek seçenekleri belirtmeye izin verir.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Yeni bir `MPPSaveOptions` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Projeyi MPP formatında kaydederken mevcut VBA makro verilerini kaldırıp kaldırmayacağını belirten bir değeri alır veya ayarlar. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Oluşturulan MPP dosyasını korumak için kullanılan bir parolayı alır veya ayarlar. Şu anda MS Project 2010 ve daha yeni formatlar için desteklenmektedir. Null değeri, proje dosyasının korunmadığını gösterir. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | MPP'ye kaydederken geçersiz kaynak atamalarını kaldırıp kaldırmayacağını gösteren bir değeri alır veya ayarlar. MS Project her görev için boş bir kaynak ataması oluşturur. Kaydetme sırasında bunları kaldırmak için bu bayrağı true olarak ayarlayın. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği biçimi alır veya ayarlar. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır veya ayarlar. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında renderlanan görevleri filtrelemek için kullanılan koşulu alır veya ayarlar. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Projeyi MPP formatında kaydederken filtre verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Filtre verileri Project.TaskFilters ve Project.ResourceFilters koleksiyonlarını içerir. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Projeyi MPP formatında kaydederken grup verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Grup verileri Project.TaskGroups ve Project.ResourceGroups koleksiyonlarını içerir. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | MPP dosyasındaki mevcut VBA makro verilerini güncelleyip güncellemeyeceğini gösteren bir değeri alır veya ayarlar. Şu anda VbaModule.SourceCode yazımı desteklenmektedir. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Projeyi MPP formatında kaydederken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Görünüm verileri Project.Views, Filters ve Tables koleksiyonlarını içerir. |

## Örnekler

Projeyi bir akışa MPP dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // kaydetme seçenekleri oluştur
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // MPP'ye kaydederken geçersiz kaynak atamalarını kaldırıp kaldırmayacağını gösteren bir değeri ayarlar
        RemoveInvalidAssignments = true
    };

    // seçeneklerle MPP kaydet
    project.Save(stream, options);
}
```

### Ayrıca Bakınız

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


