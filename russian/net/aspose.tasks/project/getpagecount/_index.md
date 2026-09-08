---
title: "Project.GetPageCount"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает количество страниц проекта, которое будет отрисовано с использованием заданных SaveOptions."
type: docs
weight: 1110
url: /ru/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Возвращает количество страниц проекта, которое будет отрисовано с использованием заданных [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveOptions | SaveOptions | Параметры сохранения, для которых требуется получить количество страниц. |

### Возвращаемое значение

количество страниц для отрисовки.

## Примеры

В этом примере экземпляр HtmlSaveOptions и количество страниц в полученном HTML выводятся в консоль.

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

Показывает, как получить количество страниц для конкретных параметров сохранения.

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

### См. также

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Возвращает количество страниц проекта, которое будет отрисовано с использованием значения по умолчанию [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Дни).

```csharp
public int GetPageCount()
```

### Возвращаемое значение

Количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц для разных шкал времени.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Получить количество страниц, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Возвращает количество страниц проекта, которое будет отрисовано с использованием заданного [`Timescale`](../../../aspose.tasks.visualization/timescale/).

```csharp
public int GetPageCount(Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| масштаб | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц для разных шкал времени.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Получить количество страниц, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### См. также

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Возвращает количество страниц проекта, которое будет отрисовано с использованием значения по умолчанию [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Дни) и заданного [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формат | PresentationFormat | Формат, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц по формату представления и шкале времени.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Получить количество страниц для Days (по умолчанию), Months и ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### См. также

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Возвращает количество страниц проекта, которое будет отрисовано с использованием заданных [`Timescale`](../../../aspose.tasks.visualization/timescale/) и [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формат | PresentationFormat | Формат, для которого нужно получить количество страниц. |
| масштаб | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц по формату представления и шкале времени.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Получить количество страниц для Days (по умолчанию), Months и ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### См. также

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Возвращает количество страниц проекта, которое будет отрисовано с использованием заданных [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) и диапазона дат.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageSize | PageSize | Размер, для которого нужно получить количество страниц. |
| масштаб | Timescale | Масштаб, для которого нужно получить количество страниц. |
| startDate | DateTime | Дата начала, для которой нужно получить количество страниц. |
| endDate | DateTime | Дата окончания, для которой нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц по размеру страницы, шкале времени, дате начала и дате завершения.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### См. также

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Возвращает количество страниц проекта, которое будет отрисовано с использованием заданных [`Timescale`](../../../aspose.tasks.visualization/timescale/) и [`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageSize | PageSize | Размер, для которого нужно получить количество страниц. |
| масштаб | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отрисовки.

## Примеры

Показывает, как получить количество страниц по размеру страницы и шкале времени.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### См. также

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


