---
title: "Class SaveTemplateOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Saving.SaveTemplateOptions sınıfı. Bir projeyi şablon olarak kaydederken ek seçenekler belirtmeye olanak tanır"
type: docs
weight: 2200
url: /tr/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Projeyi şablon olarak kaydederken ek seçenekleri belirtmeye izin verir.

```csharp
public class SaveTemplateOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Bir proje şablonundaki tüm gerçek değerlerin kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Bir proje şablonundaki tüm temel değerlerin kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Bir proje şablonundaki tüm sabit maliyetlerin kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Bir proje şablonundaki kaynak oranlarının kaldırılıp kaldırılmayacağını gösteren bir değeri alır veya ayarlar. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


