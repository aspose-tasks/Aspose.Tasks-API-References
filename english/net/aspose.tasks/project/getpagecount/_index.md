---
title: Project.GetPageCount
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Returns page count for the project to be rendered using given SaveOptions
type: docs
weight: 1110
url: /net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Returns page count for the project to be rendered using given [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | SaveOptions | The save options to get page count for. |

### Return Value

a page count to be rendered.

## Examples

In this example instance of HtmlSaveOptions and the number of pages in resulting HTML is written to the console.

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

Shows how to get page count for specific save options.

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

### See Also

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Returns page count for the project to be rendered using default [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days).

```csharp
public int GetPageCount()
```

### Return Value

Page count to be rendered.

## Examples

Shows how to get page count for different timescales.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Get number of pages, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale/).

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| scale | Timescale | The scale to get page count for. |

### Return Value

Page count to be rendered.

## Examples

Shows how to get page count for different timescales.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Get number of pages, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### See Also

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Returns page count for the project to be rendered using default [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) and given [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | The format to get page count for. |

### Return Value

Page count to be rendered.

## Examples

Shows how to get count of pages by presentation format and timescale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Get number of pages for Days (by default), Months and ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### See Also

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale/) and [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | The format to get page count for. |
| scale | Timescale | The scale to get page count for. |

### Return Value

a page count to be rendered.

## Examples

Shows how to get count of pages by presentation format and timescale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Get number of pages for Days (by default), Months and ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### See Also

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) and date range.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | PageSize | The size to get page count for. |
| scale | Timescale | The scale to get page count for. |
| startDate | DateTime | The start date to get page count for. |
| endDate | DateTime | The end date to get page count for. |

### Return Value

Page count to be rendered.

## Examples

Shows how to get count of pages by page size, timescale, start and finish dates.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### See Also

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale/) and [`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | PageSize | The size to get page count for. |
| scale | Timescale | The scale to get page count for. |

### Return Value

Page count to be rendered.

## Examples

Shows how to get count of pages by a page size and a timescale.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### See Also

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


