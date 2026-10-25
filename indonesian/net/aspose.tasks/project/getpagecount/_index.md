---
title: "Project.GetPageCount"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan SaveOptions yang diberikan"
type: docs
weight: 1110
url: /id/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| saveOptions | SaveOptions | Opsi penyimpanan untuk mendapatkan jumlah halaman. |

### Nilai Kembali

jumlah halaman yang akan dirender.

## Contoh

Dalam contoh ini, instance HtmlSaveOptions dan jumlah halaman dalam HTML yang dihasilkan ditulis ke konsol.

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

Menampilkan cara mendapatkan jumlah halaman untuk opsi penyimpanan tertentu.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var options = new HtmlSaveOptions
                  {
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A4,
                      Timescale = Timescale.Days,
                      StartDate = project.Get(Prj.StartDate).Date,
                      EndDate = project.Get(Prj.FinishDate).Date
                  };

Console.WriteLine(project.GetPageCount(options));
```

### Lihat Juga

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan default [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Hari).

```csharp
public int GetPageCount()
```

### Nilai Kembali

Jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman untuk skala waktu yang berbeda.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Dapatkan jumlah halaman, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../../aspose.tasks.visualization/timescale/) yang diberikan.

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| skala | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Kembali

Jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman untuk skala waktu yang berbeda.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Dapatkan jumlah halaman, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Lihat Juga

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan default [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Hari) dan [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) yang diberikan.

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| format | PresentationFormat | Format untuk mendapatkan jumlah halaman. |

### Nilai Kembali

Jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman berdasarkan format presentasi dan skala waktu.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Dapatkan jumlah halaman untuk Hari (default), Bulan, dan ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Lihat Juga

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../../aspose.tasks.visualization/timescale/) dan [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) yang diberikan.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| format | PresentationFormat | Format untuk mendapatkan jumlah halaman. |
| skala | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Kembali

jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman berdasarkan format presentasi dan skala waktu.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Dapatkan jumlah halaman untuk Hari (default), Bulan, dan ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Lihat Juga

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) dan rentang tanggal yang diberikan.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pageSize | PageSize | Ukuran untuk mendapatkan jumlah halaman. |
| skala | Timescale | Skala untuk mendapatkan jumlah halaman. |
| startDate | DateTime | Tanggal mulai untuk mendapatkan jumlah halaman. |
| endDate | DateTime | Tanggal akhir untuk mendapatkan jumlah halaman. |

### Nilai Kembali

Jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman berdasarkan ukuran halaman, skala waktu, tanggal mulai, dan tanggal selesai.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Lihat Juga

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan [`Timescale`](../../../aspose.tasks.visualization/timescale/) dan [`PageSize`](../../../aspose.tasks.visualization/pagesize/) yang diberikan.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pageSize | PageSize | Ukuran untuk mendapatkan jumlah halaman. |
| skala | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Kembali

Jumlah halaman yang akan dirender.

## Contoh

Menampilkan cara mendapatkan jumlah halaman berdasarkan ukuran halaman dan skala waktu.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Lihat Juga

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


