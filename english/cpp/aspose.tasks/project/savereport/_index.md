---
title: "Aspose::Tasks::Project::SaveReport method"
linktitle: "SaveReport"
articleTitle: "SaveReport"
second_title: "Aspose.Tasks for C++"
description: "Saves the project overview report to the stream."
type: docs
weight: 1210
url: /cpp/aspose.tasks/project/savereport/
---

## SaveReport (1 of 4) {#savereport_1}

Saves the project overview report to the stream.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream)
```

| Parameter | Description |
| --- | --- |
| stream | The stream to save project report to. |

---

## SaveReport (2 of 4) {#savereport_2}

Saves the project report of the specified type to the specified stream.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream, Visualization::ReportType reportType)
```

| Parameter | Description |
| --- | --- |
| stream | the specified stream to save project report to. |
| reportType | the specified report type. ReportType |

---

## SaveReport (3 of 4) {#savereport_3}

Saves the project overview report to PDF file.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName)
```

| Parameter | Description |
| --- | --- |
| fileName | The file name. |

---

## SaveReport (4 of 4) {#savereport_4}

Saves the project report of the specified type in PDF format to the specified file path.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName, Visualization::ReportType reportType)
```

| Parameter | Description |
| --- | --- |
| fileName | the specified file name. |
| reportType | the specified report type. ReportType |

