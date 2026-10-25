---
title: "Project.Print"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Project method. Mencetak proyek ke printer default dengan pengaturan printer default menggunakan kontroler cetak standar tanpa Antarmuka Pengguna"
type: docs
weight: 1140
url: /id/net/aspose.tasks/project/print/
---
## Print() {#print}

Mencetak proyek ke printer default dengan pengaturan printer default menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print()
```

## Contoh

Menampilkan cara mencetak proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Print();
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrintOptions) {#print_1}

Mencetak proyek ke printer default dengan pengaturan printer default dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(PrintOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| options | PrintOptions | instance yang ditentukan dari kelas [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) |

## Contoh

Menampilkan cara mencetak proyek dengan menggunakan opsi cetak.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.ThirdsOfMonths
};
if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
{
    project.Print(options);
}
```

### Lihat Juga

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(string) {#print_6}

Mencetak proyek ke printer yang ditentukan dengan pengaturan printer default menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(string printerName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | String | Nama printer yang ditentukan. |

## Contoh

Menampilkan cara mencetak proyek pada printer yang dipilih.

```csharp
var project = new Project(DataDir + "Project2.mpp");

foreach (string printer in PrinterSettings.InstalledPrinters)
{
    if (!printer.ToUpperInvariant().Contains("Microsoft Print to PDF".ToUpperInvariant()))
    {
        continue;
    }

    project.Print(printer);
    break;
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings) {#print_2}

Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(PrinterSettings printerSettings)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerSettings | PrinterSettings | instance yang ditentukan dari kelas PrinterSettings. |

## Contoh

Menampilkan cara menggunakan pengaturan printer untuk mencetak proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Cetak dua halaman pertama
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, string) {#print_5}

Mencetak proyek sesuai dengan pengaturan printer yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(PrinterSettings printerSettings, string documentName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerSettings | PrinterSettings | instance yang ditentukan dari kelas PrinterSettings. |
| documentName | String | nama dokumen yang akan ditampilkan (misalnya, dalam kotak dialog status cetak atau antrian printer). |

## Contoh

Menampilkan cara menggunakan pengaturan printer dan nama dokumen untuk mencetak proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Cetak dua halaman pertama
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, "Document #1");
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions) {#print_3}

Mencetak proyek sesuai dengan pengaturan printer yang ditentukan dan opsi penyimpanan khusus menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerSettings | PrinterSettings | instance yang ditentukan dari kelas PrinterSettings. |
| options | PrintOptions | instance yang ditentukan dari kelas [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) |

## Contoh

Menampilkan cara menggunakan opsi printer dan pengaturan untuk mencetak proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Cetak dua halaman pertama
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options);
```

### Lihat Juga

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Print(PrinterSettings, PrintOptions, string) {#print_4}

Mencetak proyek sesuai dengan pengaturan printer yang ditentukan, opsi penyimpanan khusus, dan nama dokumen yang ditentukan menggunakan kontroler cetak standar (tanpa Antarmuka Pengguna).

```csharp
public void Print(PrinterSettings printerSettings, PrintOptions options, string documentName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerSettings | PrinterSettings | instance yang ditentukan dari kelas PrinterSettings. |
| options | PrintOptions | instance yang ditentukan dari kelas [`PrintOptions`](../../../aspose.tasks.saving/printoptions/) |
| documentName | String | nama dokumen yang akan ditampilkan (misalnya, dalam kotak dialog status cetak atau antrian printer). |

## Contoh

Menampilkan cara menggunakan opsi printer, pengaturan printer, dan nama dokumen untuk mencetak proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var options = new PrintOptions
{
    Timescale = Timescale.Months
};

// Cetak dua halaman pertama
var settings = new PrinterSettings
{
    PrintRange = PrintRange.SomePages,
    FromPage = 1,
    ToPage = 2
};

project.Print(settings, options, "My project name");
```

### Lihat Juga

* class [PrintOptions](../../../aspose.tasks.saving/printoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


