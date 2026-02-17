---
title: Project.SaveReport
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Saves the project overview report to the stream
type: docs
weight: 1230
url: /net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Saves the project overview report to the stream.

```csharp
public void SaveReport(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream to save project report to. |

## Examples

Shows how to save the project overview report to PDF file.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// save the overview report to PDF file to the specified stream.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Saves the project overview report to PDF file.

```csharp
public void SaveReport(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The file name. |

## Examples

Shows how to save the project overview report to PDF file into a stream.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// one can save the overview report to PDF file to the specified path
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Saves the project report of the specified type to the specified stream.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the specified stream to save project report to. |
| reportType | ReportType | the specified report type.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Examples

Shows how to save the project report to PDF file for specific report type.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// save the overview report to PDF file to the specified stream.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### See Also

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Saves the project report of the specified type in PDF format to the specified file path.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | the specified file name. |
| reportType | ReportType | the specified report type.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Examples

Shows how to save the project project report in PDF format.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### See Also

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


