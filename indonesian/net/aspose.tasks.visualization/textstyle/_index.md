---
title: "Kelas TextStyle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.TextStyle. Ubah gaya visual teks untuk sebuah item dalam tampilan proyek"
type: docs
weight: 3420
url: /id/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Ubah gaya visual teks untuk item dalam tampilan proyek.

```csharp
public class TextStyle
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Menginisialisasi instance baru dari kelas `TextStyle` dengan pengaturan default. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Menginisialisasi instance baru dari kelas `TextStyle` dengan pengaturan font yang ditentukan. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Menginisialisasi instance baru dari kelas `TextStyle` dengan font default dan gaya font yang ditentukan. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Menginisialisasi instance baru dari kelas `TextStyle` dengan font default serta ukuran dan gaya font yang ditentukan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Mendapatkan atau mengatur warna latar belakang gaya teks. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Mendapatkan atau mengatur pola latar belakang gaya teks. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Mendapatkan atau mengatur warna teks. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Mendapatkan atau mengatur font gaya teks. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Mendapatkan atau mengatur [`TextItemType`](../textitemtype/) dari gaya teks. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


