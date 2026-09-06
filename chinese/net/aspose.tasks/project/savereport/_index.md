---
title: "Project.SaveReport"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。将项目概览报告保存到流中"
type: docs
weight: 1220
url: /zh/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

将项目概览报告保存到流中。

```csharp
public void SaveReport(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于保存项目报告的流。 |

## 示例

展示如何将项目概览报告保存为 PDF 文件。

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 将概览报告保存为 PDF 文件到指定的流。
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

将项目概览报告保存为 PDF 文件。

```csharp
public void SaveReport(string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | 字符串 | 文件名。 |

## 示例

展示如何将项目概览报告保存为 PDF 文件到流中。

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 可以将概览报告保存为 PDF 文件到指定路径
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

将指定类型的项目报告保存到指定的流中。

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 指定的用于保存项目报告的流。 |
| reportType | ReportType | 指定的报告类型。[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## 示例

展示如何针对特定报告类型将项目报告保存为 PDF 文件。

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// 将概览报告保存为 PDF 文件到指定的流。
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### 另见

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

将指定类型的项目报告以 PDF 格式保存到指定的文件路径。

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | 字符串 | 指定的文件名。 |
| reportType | ReportType | 指定的报告类型。[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## 示例

展示如何以 PDF 格式保存项目报告。

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### 另见

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


