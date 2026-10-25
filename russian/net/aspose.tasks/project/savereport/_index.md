---
title: "Project.SaveReport"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Сохраняет обзорный отчёт проекта в поток."
type: docs
weight: 1220
url: /ru/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Сохраняет обзорный отчёт проекта в поток.

```csharp
public void SaveReport(Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | Поток, в который сохраняется отчёт проекта. |

## Примеры

Показывает, как сохранить обзорный отчёт проекта в PDF‑файл.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// сохранить обзорный отчёт в PDF‑файл в указанный поток.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Сохраняет обзорный отчёт проекта в PDF‑файл.

```csharp
public void SaveReport(string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | Строка | Имя файла. |

## Примеры

Показывает, как сохранить обзорный отчёт проекта в PDF‑файл в поток.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// можно сохранить обзорный отчёт в PDF‑файл по указанному пути
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Сохраняет отчёт проекта указанного типа в указанный поток.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Поток | указанный поток, в который сохраняется отчёт проекта. |
| reportType | ReportType | указанный тип отчёта.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Примеры

Показывает, как сохранить отчёт проекта в PDF‑файл для конкретного типа отчёта.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// сохранить обзорный отчёт в PDF‑файл в указанный поток.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### См. также

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Сохраняет отчёт проекта указанного типа в формате PDF в указанный путь к файлу.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | Строка | указанное имя файла. |
| reportType | ReportType | указанный тип отчёта.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Примеры

Показывает, как сохранить отчёт проекта в формате PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### См. также

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


