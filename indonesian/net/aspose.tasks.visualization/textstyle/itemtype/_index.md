---
title: "TextStyle.ItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TextStyle. Mendapatkan atau mengatur TextItemType dari gaya teks"
type: docs
weight: 60
url: /id/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

Mendapatkan atau mengatur [`TextItemType`](../../textitemtype/) dari gaya teks.

```csharp
public virtual TextItemType ItemType { get; set; }
```

## Contoh

Menampilkan cara menyesuaikan gaya teks yang digunakan untuk menata berbagai item teks dalam sebuah proyek.

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

### Lihat Juga

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


