---
title: "Project.SaveReport"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 프로젝트 개요 보고서를 스트림에 저장합니다."
type: docs
weight: 1220
url: /ko/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

프로젝트 개요 보고서를 스트림에 저장합니다.

```csharp
public void SaveReport(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 프로젝트 보고서를 저장할 스트림. |

## 예제

프로젝트 개요 보고서를 PDF 파일에 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 지정된 스트림에 개요 보고서를 PDF 파일로 저장합니다.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

프로젝트 개요 보고서를 PDF 파일에 저장합니다.

```csharp
public void SaveReport(string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileName | 문자열 | 파일 이름. |

## 예제

스트림에 프로젝트 개요 보고서를 PDF 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 지정된 경로에 개요 보고서를 PDF 파일로 저장할 수 있습니다.
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

지정된 유형의 프로젝트 보고서를 지정된 스트림에 저장합니다.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 프로젝트 보고서를 저장할 지정된 스트림. |
| reportType | ReportType | 지정된 보고서 유형.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## 예제

특정 보고서 유형에 대해 프로젝트 보고서를 PDF 파일로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 지정된 스트림에 개요 보고서를 PDF 파일로 저장합니다.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### 또 보기

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

지정된 유형의 프로젝트 보고서를 PDF 형식으로 지정된 파일 경로에 저장합니다.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileName | 문자열 | 지정된 파일 이름. |
| reportType | ReportType | 지정된 보고서 유형.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## 예제

프로젝트 보고서를 PDF 형식으로 저장하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### 또 보기

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


