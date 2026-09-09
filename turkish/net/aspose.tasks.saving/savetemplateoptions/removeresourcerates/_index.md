---
title: "SaveTemplateOptions.RemoveResourceRates"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveTemplateOptions özelliği. Bir proje şablonundaki kaynak oranlarının kaldırılıp kaldırılmayacağını belirten bir değeri alır veya ayarlar"
type: docs
weight: 50
url: /tr/net/aspose.tasks.saving/savetemplateoptions/removeresourcerates/
---
## SaveTemplateOptions.RemoveResourceRates property

Bir proje şablonundaki kaynak oranlarının kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar.

```csharp
public bool RemoveResourceRates { get; set; }
```

## Örnekler

Seçenekleri kullanarak projeyi şablon olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// şablon kaydetme seçenekleri oluştur
// ve özelliklerini ayarla
var options = new SaveTemplateOptions
{
    // bir proje şablonundaki tüm sabit maliyetlerin kaldırılıp kaldırılmayacağını gösteren bir değeri ayarla
    RemoveFixedCosts = true,

    // bir proje şablonundaki tüm gerçek değerlerin kaldırılıp kaldırılmayacağını gösteren bir değeri ayarla
    RemoveActualValues = true,

    // bir proje şablonundaki kaynak oranlarının kaldırılıp kaldırılmayacağını gösteren bir değeri ayarla
    RemoveResourceRates = true,

    // bir proje şablonundaki tüm temel değerlerin kaldırılıp kaldırılmayacağını gösteren bir değeri ayarla
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Ayrıca Bakınız

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


