---
title: "TextStyle.BackgroundColor"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TextStyle. Mendapatkan atau mengatur warna latar belakang dari gaya teks. Color"
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/textstyle/backgroundcolor/
---
## TextStyle.BackgroundColor property

Mendapatkan atau mengatur warna latar belakang dari gaya teks. [`Color`](../color/).

```csharp
public Color BackgroundColor { get; set; }
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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


