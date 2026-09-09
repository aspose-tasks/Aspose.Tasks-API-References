---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MPPSaveOptions özelliği. Bir projeyi MPP formatında kaydederken mevcut VBA makro verilerinin kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar."
type: docs
weight: 20
url: /tr/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Projeyi MPP formatında kaydederken mevcut VBA makro verilerini kaldırıp kaldırmayacağını belirten bir değeri alır veya ayarlar.

```csharp
public bool ClearVba { get; set; }
```

## Örnekler

MPP dosyasından VBA makrolarını nasıl kaldıracağınızı gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Ayrıca Bakınız

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


