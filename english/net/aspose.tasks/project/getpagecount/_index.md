---
title: GetPageCount
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 300
url: /net/aspose.tasks/project/getpagecount/
---
## Project.GetPageCount method (1 of 7)

Returns page count for the project to be rendered using given [`SaveOptions`](../../../aspose.tasks.saving/saveoptions).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | SaveOptions | The save options to get page count for. |

### Return Value

a page count to be rendered.

### Examples

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

### See Also

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (2 of 7)

Returns page count for the project to be rendered using default [`Timescale`](../../../aspose.tasks.visualization/timescale)(Days).

```csharp
public int GetPageCount()
```

### Return Value

Page count to be rendered.

### See Also

* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (3 of 7)

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale).

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| scale | Timescale | The scale to get page count for. |

### Return Value

Page count to be rendered.

### See Also

* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (4 of 7)

Returns page count for the project to be rendered using default [`Timescale`](../../../aspose.tasks.visualization/timescale)(Days) and given [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | The format to get page count for. |

### Return Value

Page count to be rendered.

### See Also

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (5 of 7)

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale) and [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| format | PresentationFormat | The format to get page count for. |
| scale | Timescale | The scale to get page count for. |

### Return Value

a page count to be rendered.

### See Also

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (6 of 7)

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) and date range.

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

### See Also

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

---

## Project.GetPageCount method (7 of 7)

Returns page count for the project to be rendered using given [`Timescale`](../../../aspose.tasks.visualization/timescale) and [`PageSize`](../../../aspose.tasks.visualization/pagesize).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | PageSize | The size to get page count for. |
| scale | Timescale | The scale to get page count for. |

### Return Value

Page count to be rendered.

### See Also

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* namespace [Aspose.Tasks](../../project)
* assembly [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
