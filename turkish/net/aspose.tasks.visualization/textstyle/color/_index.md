---
title: "TextStyle.Color"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TextStyle özelliği. Metnin rengini alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Metnin rengini alır veya ayarlar.

```csharp
public Color Color { get; set; }
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


