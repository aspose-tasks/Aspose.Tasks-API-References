---
title: "Enum BackgroundPattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.BackgroundPattern. Menentukan pola latar belakang"
type: docs
weight: 100
url: /id/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Menentukan pola latar belakang.

```csharp
public enum BackgroundPattern
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Menunjukkan pola latar belakang diagonal kiri gelap. |
| DarkDiagonalRight | `8` | Menunjukkan pola latar belakang diagonal kanan gelap. |
| DarkDither | `13` | Menunjukkan pola latar belakang dither gelap. |
| DarkFill | `4` | Menunjukkan pola latar belakang isi gelap. |
| DiagonalLeft | `5` | Menunjukkan pola latar belakang diagonal kiri. |
| DiagonalRight | `6` | Menunjukkan pola latar belakang diagonal kanan. |
| Hollow | `0` | Menunjukkan pola latar belakang berongga. |
| LightDither | `11` | Menunjukkan pola latar belakang dither ringan. |
| LightFill | `2` | Menunjukkan pola latar belakang isi ringan. |
| MediumDither | `12` | Menunjukkan pola latar belakang dither sedang. |
| MediumFill | `3` | Menunjukkan pola latar belakang isi sedang. |
| MediumVerticalStripe | `10` | Menunjukkan pola latar belakang garis vertikal sedang. |
| SolidFill | `1` | Menunjukkan pola latar belakang isi padat. |
| ThinVerticalStripe | `9` | Menunjukkan pola latar belakang garis vertikal tipis. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


