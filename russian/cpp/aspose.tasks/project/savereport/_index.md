---
title: "Aspose::Tasks::Project::SaveReport метод"
linktitle: "SaveReport"
articleTitle: "SaveReport"
second_title: "Aspose.Tasks для C++"
description: "Сохраняет обзорный отчёт проекта в поток."
type: docs
weight: 1210
url: /ru/cpp/aspose.tasks/project/savereport/
---

## SaveReport (1 of 4) {#savereport_1}

Сохраняет обзорный отчёт проекта в поток.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream)
```

| Параметр | Описание |
| --- | --- |
| stream | Поток, в который сохраняется отчёт проекта. |

---

## SaveReport (2 of 4) {#savereport_2}

Сохраняет отчёт проекта указанного типа в указанный поток.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream, Visualization::ReportType reportType)
```

| Параметр | Описание |
| --- | --- |
| stream | указанный поток, в который сохраняется отчёт проекта. |
| reportType | указанный тип отчёта. ReportType |

---

## SaveReport (3 of 4) {#savereport_3}

Сохраняет обзорный отчёт проекта в PDF‑файл.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName)
```

| Параметр | Описание |
| --- | --- |
| fileName | Имя файла. |

---

## SaveReport (4 of 4) {#savereport_4}

Сохраняет отчёт проекта указанного типа в формате PDF по указанному пути к файлу.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName, Visualization::ReportType reportType)
```

| Параметр | Описание |
| --- | --- |
| fileName | указанное имя файла. |
| reportType | указанный тип отчёта. ReportType |

