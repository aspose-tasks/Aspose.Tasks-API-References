---
title: "Project.SaveReport"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Slaat het projectoverzichtsrapport op naar de stream"
type: docs
weight: 1220
url: /nl/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Slaat het projectoverzichtsrapport op in de stream.

```csharp
public void SaveReport(Stream stream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | De stream waarin het projectrapport moet worden opgeslagen. |

## Voorbeelden

Toont hoe het projectoverzichtsrapport op te slaan als PDF-bestand.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// sla het overzichtsrapport op als PDF-bestand naar de opgegeven stream.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Slaat het projectoverzichtsrapport op in een PDF-bestand.

```csharp
public void SaveReport(string fileName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | De bestandsnaam. |

## Voorbeelden

Toont hoe het projectoverzichtsrapport op te slaan als PDF-bestand in een stream.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// men kan het overzichtsrapport opslaan als PDF-bestand naar het opgegeven pad
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Slaat het projectrapport van het opgegeven type op in de opgegeven stream.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stroom | Stroom | de opgegeven stream om het projectrapport in op te slaan. |
| reportType | ReportType | het opgegeven rapporttype.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Voorbeelden

Toont hoe het projectrapport op te slaan als PDF-bestand voor een specifiek rapporttype.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// sla het overzichtsrapport op als PDF-bestand naar de opgegeven stream.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Zie ook

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Slaat het projectrapport van het opgegeven type in PDF-indeling op op het opgegeven bestandspad.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | String | de opgegeven bestandsnaam. |
| reportType | ReportType | het opgegeven rapporttype.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Voorbeelden

Toont hoe het projectrapport op te slaan in PDF-formaat.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Zie ook

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


