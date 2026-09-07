---
title: "TextStyle.TextStyle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor TextStyle. Menginisialisasi instance baru dari kelas TextStyle dengan pengaturan default"
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Menginisialisasi instance baru dari kelas [`TextStyle`](../) dengan pengaturan default.

```csharp
public TextStyle()
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

---

## TextStyle(float, FontStyles) {#constructor_3}

Menginisialisasi instance baru dari kelas [`TextStyle`](../) dengan font default dan ukuran serta gaya font yang ditentukan.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontSize | Single | Ukuran font dari TextStyle. |
| fontStyle | FontStyles | Gaya font dari TextStyle. |

### Lihat Juga

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Menginisialisasi instance baru dari kelas [`TextStyle`](../) dengan font default dan gaya font yang ditentukan.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontStyle | FontStyles | Gaya font yang diterapkan pada font default. |

### Lihat Juga

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Menginisialisasi instance baru dari kelas [`TextStyle`](../) dengan pengaturan font yang ditentukan.

```csharp
public TextStyle(FontDescriptor font)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| font | FontDescriptor | Font dari TextStyle. |

### Lihat Juga

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


