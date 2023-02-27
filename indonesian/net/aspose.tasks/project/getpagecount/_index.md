---
title: GetPageCount
second_title: Aspose.Tasks untuk Referensi .NET API
description: Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikanSaveOptionsaspose.tasks.saving/saveoptions/ .
type: docs
weight: 1080
url: /id/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikan[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| saveOptions | SaveOptions | Opsi simpan untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

jumlah halaman yang akan dirender.

### Contoh

Dalam contoh contoh HtmlSaveOptions ini dan jumlah halaman dalam HTML yang dihasilkan ditulis ke konsol.

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

### Lihat juga

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan default[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Hari).

```csharp
public int GetPageCount()
```

### Nilai Pengembalian

Jumlah halaman yang akan dirender.

### Lihat juga

* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikan[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| scale | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

Jumlah halaman yang akan dirender.

### Lihat juga

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan default[`Timescale`](../../../aspose.tasks.visualization/timescale/) (hari) dan diberikan[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| format | PresentationFormat | Format untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

Jumlah halaman yang akan dirender.

### Lihat juga

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikan[`Timescale`](../../../aspose.tasks.visualization/timescale/) Dan[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| format | PresentationFormat | Format untuk mendapatkan jumlah halaman. |
| scale | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

jumlah halaman yang akan dirender.

### Lihat juga

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikan[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) dan rentang tanggal.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageSize | PageSize | Ukuran untuk mendapatkan jumlah halaman. |
| scale | Timescale | Skala untuk mendapatkan jumlah halaman. |
| startDate | DateTime | Tanggal mulai untuk mendapatkan jumlah halaman. |
| endDate | DateTime | Tanggal akhir untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

Jumlah halaman yang akan dirender.

### Lihat juga

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan yang diberikan[`Timescale`](../../../aspose.tasks.visualization/timescale/) Dan[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageSize | PageSize | Ukuran untuk mendapatkan jumlah halaman. |
| scale | Timescale | Skala untuk mendapatkan jumlah halaman. |

### Nilai Pengembalian

Jumlah halaman yang akan dirender.

### Lihat juga

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ruang nama [Aspose.Tasks](../../project/)
* perakitan [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
