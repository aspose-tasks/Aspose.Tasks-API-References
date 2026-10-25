---
title: "Project.SaveReport"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Salva il report di riepilogo del progetto nello stream."
type: docs
weight: 1220
url: /it/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Salva il report di panoramica del progetto nello stream.

```csharp
public void SaveReport(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Lo stream in cui salvare il report del progetto. |

## Esempi

Mostra come salvare il report di riepilogo del progetto in un file PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// salva il report di riepilogo in un file PDF nello stream specificato.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Salva il report di panoramica del progetto in un file PDF.

```csharp
public void SaveReport(string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | Stringa | Il nome del file. |

## Esempi

Mostra come salvare il report di riepilogo del progetto in un file PDF in uno stream.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// è possibile salvare il report di riepilogo in un file PDF nel percorso specificato
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Salva il report del progetto del tipo specificato nello stream specificato.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | lo stream specificato in cui salvare il report del progetto. |
| reportType | ReportType | il tipo di report specificato.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Esempi

Mostra come salvare il report del progetto in un file PDF per un tipo di report specifico.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// salva il report di riepilogo in un file PDF nello stream specificato.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Vedi anche

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Salva il report del progetto del tipo specificato in formato PDF nel percorso file specificato.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | Stringa | il nome del file specificato. |
| reportType | ReportType | il tipo di report specificato.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Esempi

Mostra come salvare il report del progetto in formato PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Vedi anche

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


