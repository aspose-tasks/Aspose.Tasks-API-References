---
title: "Project.SaveReport"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تحفظ تقرير نظرة المشروع إلى التدفق."
type: docs
weight: 1220
url: /ar/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

يحفظ تقرير نظرة عامة على المشروع إلى الدفق.

```csharp
public void SaveReport(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | التدفق لحفظ تقرير المشروع إليه. |

## الأمثلة

يعرض كيفية حفظ تقرير نظرة المشروع إلى ملف PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// احفظ تقرير النظرة إلى ملف PDF إلى التدفق المحدد.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

يحفظ تقرير نظرة عامة على المشروع إلى ملف PDF.

```csharp
public void SaveReport(string fileName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fileName | سلسلة | اسم الملف. |

## الأمثلة

يعرض كيفية حفظ تقرير نظرة المشروع إلى ملف PDF داخل تدفق.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// يمكن حفظ تقرير النظرة إلى ملف PDF إلى المسار المحدد
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

يحفظ تقرير المشروع من النوع المحدد إلى الدفق المحدد.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | التدفق المحدد لحفظ تقرير المشروع إليه. |
| reportType | ReportType | نوع التقرير المحدد.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## الأمثلة

يعرض كيفية حفظ تقرير المشروع إلى ملف PDF لنوع تقرير محدد.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// احفظ تقرير النظرة إلى ملف PDF إلى التدفق المحدد.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### انظر أيضًا

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

يحفظ تقرير المشروع من النوع المحدد بصيغة PDF إلى مسار الملف المحدد.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| fileName | سلسلة | اسم الملف المحدد. |
| reportType | ReportType | نوع التقرير المحدد.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## الأمثلة

يعرض كيفية حفظ تقرير مشروع المشروع بتنسيق PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### انظر أيضًا

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


