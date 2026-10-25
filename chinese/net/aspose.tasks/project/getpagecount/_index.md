---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。返回使用给定 SaveOptions 渲染项目的页数。"
type: docs
weight: 1110
url: /zh/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

返回使用给定 [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) 渲染项目的页数。

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveOptions | SaveOptions | 获取页数的保存选项。 |

### 返回值

要渲染的页数。

## 示例

在此示例中，HtmlSaveOptions 的实例以及生成的 HTML 中的页数会写入控制台。

```csharp
[C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
    IncludeProjectNameInPageHeader = false,
    IncludeProjectNameInTitle = false,
    PageSize = PageSize.A4,
    Timescale = Timescale.Days,
    StartDate = project.Get(Prj.StartDate).Date,
    EndDate = project.Get(Prj.FinishDate).Date
};

Console.WriteLine(project.GetPageCount(saveOptions));
```

展示如何获取特定保存选项的页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var options = new HtmlSaveOptions
                  {
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A4,
                      Timescale = Timescale.Days,
                      StartDate = project.Get(Prj.StartDate).Date,
                      EndDate = project.Get(Prj.FinishDate).Date
                  };

Console.WriteLine(project.GetPageCount(options));
```

### 另见

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

返回使用默认[`Timescale`](../../../aspose.tasks.visualization/timescale/)(天)渲染的项目的页面计数。

```csharp
public int GetPageCount()
```

### 返回值

要渲染的页面计数。

## 示例

展示如何获取不同时间尺度的页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// 获取页面数量，Timescale.Months，Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

返回使用给定[`Timescale`](../../../aspose.tasks.visualization/timescale/)渲染的项目的页面计数。

```csharp
public int GetPageCount(Timescale scale)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 比例 | 时间尺度 | 用于获取页面计数的比例。 |

### 返回值

要渲染的页面计数。

## 示例

展示如何获取不同时间尺度的页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// 获取页面数量，Timescale.Months，Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### 另见

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

返回使用默认[`Timescale`](../../../aspose.tasks.visualization/timescale/)(天)和给定[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)渲染的项目的页面计数。

```csharp
public int GetPageCount(PresentationFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 格式 | 展示格式 | 用于获取页面计数的格式。 |

### 返回值

要渲染的页面计数。

## 示例

展示如何通过展示格式和时间尺度获取页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// 获取天（默认）、Months 和 ThirdsOfMonths 的页面数量。
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### 另见

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

返回使用给定[`Timescale`](../../../aspose.tasks.visualization/timescale/)和[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)渲染的项目的页面计数。

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 格式 | 展示格式 | 用于获取页面计数的格式。 |
| 比例 | 时间尺度 | 用于获取页面计数的比例。 |

### 返回值

要渲染的页数。

## 示例

展示如何通过展示格式和时间尺度获取页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// 获取天（默认）、Months 和 ThirdsOfMonths 的页面数量。
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### 另见

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

返回使用给定[`Timescale`](../../../aspose.tasks.visualization/timescale/)、[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)和日期范围渲染的项目的页面计数。

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 页面大小 | 页面大小 | 用于获取页面计数的大小。 |
| 比例 | 时间尺度 | 用于获取页面计数的比例。 |
| 开始日期 | DateTime | 用于获取页面计数的开始日期。 |
| 结束日期 | DateTime | 用于获取页面计数的结束日期。 |

### 返回值

要渲染的页面计数。

## 示例

展示如何通过页面大小、时间尺度、开始和结束日期获取页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### 另见

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

返回使用给定[`Timescale`](../../../aspose.tasks.visualization/timescale/)和[`PageSize`](../../../aspose.tasks.visualization/pagesize/)渲染的项目的页面计数。

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 页面大小 | 页面大小 | 用于获取页面计数的大小。 |
| 比例 | 时间尺度 | 用于获取页面计数的比例。 |

### 返回值

要渲染的页面计数。

## 示例

展示如何通过页面大小和时间尺度获取页面计数。

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### 另见

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


