---
title: "Project.SaveReport"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Project. Guarda el informe de visión general del proyecto en el flujo."
type: docs
weight: 1220
url: /es/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Guarda el informe de visión general del proyecto en el flujo.

```csharp
public void SaveReport(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo donde guardar el informe del proyecto. |

## Ejemplos

Muestra cómo guardar el informe de visión general del proyecto en un archivo PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// guarda el informe de visión general en un archivo PDF en el flujo especificado.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Guarda el informe de visión general del proyecto en un archivo PDF.

```csharp
public void SaveReport(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | Cadena | El nombre del archivo. |

## Ejemplos

Muestra cómo guardar el informe de visión general del proyecto en un archivo PDF dentro de un flujo.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// se puede guardar el informe de visión general en un archivo PDF en la ruta especificada
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Ver también

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Guarda el informe del proyecto del tipo especificado en el flujo especificado.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | el flujo especificado donde guardar el informe del proyecto. |
| reportType | ReportType | el tipo de informe especificado.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Ejemplos

Muestra cómo guardar el informe del proyecto en un archivo PDF para un tipo de informe específico.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// guarda el informe de visión general en un archivo PDF en el flujo especificado.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Ver también

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Guarda el informe del proyecto del tipo especificado en formato PDF en la ruta de archivo especificada.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | Cadena | el nombre de archivo especificado. |
| reportType | ReportType | el tipo de informe especificado.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Ejemplos

Muestra cómo guardar el informe del proyecto en formato PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Ver también

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


