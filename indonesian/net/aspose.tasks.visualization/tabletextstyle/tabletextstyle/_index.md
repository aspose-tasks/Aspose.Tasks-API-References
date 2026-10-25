---
title: "TableTextStyle.TableTextStyle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor TableTextStyle. Menginisialisasi instance baru dari kelas TableTextStyle."
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Menginisialisasi instance baru dari kelas [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | Int32 | ID unik baris yang ditentukan. |

## Contoh

Menampilkan cara menyesuaikan gaya teks tabel yang digunakan untuk memberi gaya pada berbagai item teks dalam sebuah proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// atur gaya teks nama tugas pertama
var style1 = new TableTextStyle(1);
// atur bidang yang akan diterapkan gaya.
style1.Field = Field.TaskName;
// atur <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> dari gaya teks.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// atur ukuran dalam poin dari font gaya teks.

// atur gaya teks durasi tugas kedua
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // atur bendera yang menunjukkan bahwa data tampilan harus ditulis
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Lihat Juga

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Menginisialisasi instance baru dari kelas [`TableTextStyle`](../) dengan font yang ditentukan.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | Int32 | ID unik baris yang ditentukan. |
| font | FontDescriptor | Font yang menjadi dasar gaya teks. |

### Lihat Juga

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Menginisialisasi instance baru dari kelas [`TableTextStyle`](../) dengan ukuran font dan gaya font yang ditentukan.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | Int32 | ID unik baris yang ditentukan. |
| fontSize | Single | Ukuran font yang menjadi dasar gaya teks. |
| fontStyle | FontStyles | Gaya font yang menjadi dasar gaya teks. |

### Lihat Juga

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Menginisialisasi instance baru dari kelas [`TableTextStyle`](../) dengan pengaturan font default dan gaya font yang ditentukan.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | Int32 | ID unik baris yang ditentukan. |
| fontStyle | FontStyles | Gaya font yang menjadi dasar gaya teks. |

### Lihat Juga

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


