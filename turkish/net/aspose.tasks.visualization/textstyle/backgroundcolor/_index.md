---
title: "TextStyle.BackgroundColor"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TextStyle özelliği. Metin stilinin arka plan rengini alır veya ayarlar. Color"
type: docs
weight: 20
url: /tr/net/aspose.tasks.visualization/textstyle/backgroundcolor/
---
## TextStyle.BackgroundColor property

Metin stilinin arka plan rengini alır veya ayarlar. [`Color`](../color/).

```csharp
public Color BackgroundColor { get; set; }
```

## Örnekler

Bir projedeki farklı metin öğelerini biçimlendirmek için kullanılan metin stillerinin nasıl özelleştirileceğini gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ayrıca Bakınız

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


