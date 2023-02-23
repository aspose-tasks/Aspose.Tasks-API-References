---
title: Project.GetPageCount
second_title: Справочник по Aspose.Tasks для .NET API
description: Project метод. Возвращает количество страниц для проекта который будет отображаться с использованием заданногоSaveOptions .
type: docs
weight: 1080
url: /ru/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveOptions | SaveOptions | Параметры сохранения, для которых нужно получить количество страниц. |

### Возвращаемое значение

количество отображаемых страниц.

### Примеры

В этом примере экземпляр HtmlSaveOptions и количество страниц в результирующем HTML записывается в консоль.

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

### Смотрите также

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Возвращает количество страниц для проекта, который будет отображаться по умолчанию.[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Дней).

```csharp
public int GetPageCount()
```

### Возвращаемое значение

Количество страниц для отображения.

### Смотрите также

* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| scale | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отображения.

### Смотрите также

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Возвращает количество страниц для проекта, который будет отображаться по умолчанию.[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Дней) и дано[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| format | PresentationFormat | Формат, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отображения.

### Смотрите также

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../../aspose.tasks.visualization/timescale/) и[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| format | PresentationFormat | Формат, для которого нужно получить количество страниц. |
| scale | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

количество отображаемых страниц.

### Смотрите также

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) и диапазон дат.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageSize | PageSize | Размер, для которого нужно получить количество страниц. |
| scale | Timescale | Масштаб, для которого нужно получить количество страниц. |
| startDate | DateTime | Дата начала, для которой нужно получить количество страниц. |
| endDate | DateTime | Дата окончания, для которой нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отображения.

### Смотрите также

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../../aspose.tasks.visualization/timescale/) и[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageSize | PageSize | Размер, для которого нужно получить количество страниц. |
| scale | Timescale | Масштаб, для которого нужно получить количество страниц. |

### Возвращаемое значение

Количество страниц для отображения.

### Смотрите также

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* пространство имен [Aspose.Tasks](../../project/)
* сборка [Aspose.Tasks](../../../)


