---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MPPSaveOptions özelliği. Bir projeyi MPP formatında kaydederken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Görünüm verileri Project.Views Filters ve Tables koleksiyonlarını içerir."
type: docs
weight: 80
url: /tr/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Projeyi MPP formatında kaydederken görünüm verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Görünüm verileri Project.Views, Filters ve Tables koleksiyonlarını içerir.

```csharp
public bool WriteViewData { get; set; }
```

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


