---
title: "Project.SaveReport"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Proje özet raporunu akışa kaydeder."
type: docs
weight: 1220
url: /tr/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Proje genel bakış raporunu akışa kaydeder.

```csharp
public void SaveReport(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Proje raporunun kaydedileceği akış. |

## Örnekler

Proje özet raporunu PDF dosyasına nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Özet raporu belirtilen akışa PDF dosyası olarak kaydedin.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Proje genel bakış raporunu PDF dosyasına kaydeder.

```csharp
public void SaveReport(string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | Dize | Dosya adı. |

## Örnekler

Proje özet raporunu bir akışa PDF dosyası olarak nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Özet raporu belirtilen yola PDF dosyası olarak kaydedebilirsiniz.
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Belirtilen türdeki proje raporunu belirtilen akışa kaydeder.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Akış | Proje raporunun kaydedileceği belirtilen akış. |
| reportType | ReportType | belirtilen rapor türü.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Örnekler

Belirli rapor türü için proje raporunu PDF dosyasına nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Özet raporu belirtilen akışa PDF dosyası olarak kaydedin.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Ayrıca Bakınız

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Belirtilen türdeki proje raporunu PDF formatında belirtilen dosya yoluna kaydeder.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | Dize | Belirtilen dosya adı. |
| reportType | ReportType | belirtilen rapor türü.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Örnekler

Proje raporunu PDF formatında nasıl kaydedeceğinizi gösterir.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Ayrıca Bakınız

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


