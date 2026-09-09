---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Proje görünümünün render edilmesi sırasında uygulanan metin stillerinin listesini alır veya ayarlar."
type: docs
weight: 190
url: /tr/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Bir proje görünümünün renderlanması sırasında uygulanan metin stillerinin listesini alır veya ayarlar.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Açıklamalar

Bu stiller, GanttCharView.TextStyles içinde tanımlanan stillerin üzerine yazar.

## Örnekler

Bir projedeki farklı **metin** öğelerini biçimlendirmek için kaydetme seçeneklerinin metin stillerinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ayrıca Bakınız

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


