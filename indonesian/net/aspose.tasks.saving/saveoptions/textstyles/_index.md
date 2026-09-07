---
title: "SaveOptions.TextStyles"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur daftar gaya teks yang diterapkan selama perenderan tampilan proyek"
type: docs
weight: 190
url: /id/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Mendapatkan atau mengatur daftar gaya teks yang diterapkan selama rendering tampilan proyek.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Catatan

Gaya ini menggantikan gaya yang didefinisikan dalam GanttCharView.TextStyles.

## Contoh

Menampilkan cara menggunakan gaya teks opsi penyimpanan yang digunakan untuk menata berbagai item **text** dalam sebuah proyek.

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

### Lihat Juga

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


