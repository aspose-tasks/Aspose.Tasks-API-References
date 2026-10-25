---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ImageSaveOptions özelliği. Proje düzenini ayrı dosyalara kaydederken kaydedilecek sayfa numaralarının bir listesini alır veya ayarlar. Bu liste boşsa tüm sayfalar kaydedilir."
type: docs
weight: 50
url: /tr/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini alır veya ayarlar. Liste boşsa tüm sayfalar kaydedilir.

```csharp
public List<int> Pages { get; set; }
```

## Örnekler

Seçilen sayfaları görüntü olarak kaydetmenin nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


