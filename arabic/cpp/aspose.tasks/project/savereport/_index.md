---
title: "Aspose::Tasks::Project::SaveReport طريقة"
linktitle: "SaveReport"
articleTitle: "SaveReport"
second_title: "Aspose.Tasks لـ C++"
description: "يحفظ تقرير نظرة عامة على المشروع إلى الدفق."
type: docs
weight: 1210
url: /ar/cpp/aspose.tasks/project/savereport/
---

## SaveReport (1 of 4) {#savereport_1}

يحفظ تقرير نظرة عامة على المشروع إلى الدفق.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream)
```

| معامل | الوصف |
| --- | --- |
| stream | دفق حفظ تقرير المشروع إليه. |

---

## SaveReport (2 of 4) {#savereport_2}

يحفظ تقرير المشروع من النوع المحدد إلى الدفق المحدد.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::SharedPtr< System::IO::Stream > & stream, Visualization::ReportType reportType)
```

| معامل | الوصف |
| --- | --- |
| stream | الدفق المحدد لحفظ تقرير المشروع إليه. |
| reportType | نوع التقرير المحدد. ReportType |

---

## SaveReport (3 of 4) {#savereport_3}

يحفظ تقرير نظرة المشروع إلى ملف PDF.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName)
```

| معامل | الوصف |
| --- | --- |
| fileName | اسم الملف. |

---

## SaveReport (4 of 4) {#savereport_4}

يحفظ تقرير المشروع من النوع المحدد بصيغة PDF إلى مسار الملف المحدد.

**Returns:** void Aspose::Tasks::

```cpp
SaveReport(const System::String & fileName, Visualization::ReportType reportType)
```

| معامل | الوصف |
| --- | --- |
| fileName | اسم الملف المحدد. |
| reportType | نوع التقرير المحدد. ReportType |

