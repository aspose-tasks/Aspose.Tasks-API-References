---
title: "Project.SaveReport"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Project. Menyimpan laporan ikhtisar proyek ke stream"
type: docs
weight: 1220
url: /id/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Menyimpan laporan ikhtisar proyek ke aliran.

```csharp
public void SaveReport(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran untuk menyimpan laporan proyek. |

## Contoh

Menampilkan cara menyimpan laporan ikhtisar proyek ke file PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// simpan laporan ikhtisar ke file PDF ke aliran yang ditentukan.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Menyimpan laporan ikhtisar proyek ke file PDF.

```csharp
public void SaveReport(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file. |

## Contoh

Menampilkan cara menyimpan laporan ikhtisar proyek ke file PDF ke dalam aliran.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// seseorang dapat menyimpan laporan ikhtisar ke file PDF ke jalur yang ditentukan
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Lihat Juga

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Menyimpan laporan proyek tipe yang ditentukan ke aliran yang ditentukan.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | aliran yang ditentukan untuk menyimpan laporan proyek. |
| reportType | ReportType | tipe laporan yang ditentukan.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Contoh

Menampilkan cara menyimpan laporan proyek ke file PDF untuk tipe laporan tertentu.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// simpan laporan ikhtisar ke file PDF ke aliran yang ditentukan.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Lihat Juga

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Menyimpan laporan proyek tipe yang ditentukan dalam format PDF ke jalur file yang ditentukan.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | nama file yang ditentukan. |
| reportType | ReportType | tipe laporan yang ditentukan.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Contoh

Menampilkan cara menyimpan laporan proyek proyek dalam format PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Lihat Juga

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


