---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 지정된 SaveOptions를 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다."
type: docs
weight: 1110
url: /ko/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

지정된 [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/)를 사용하여 렌더링될 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| saveOptions | SaveOptions | 페이지 수를 가져오기 위한 저장 옵션입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

이 예제에서는 HtmlSaveOptions 인스턴스와 결과 HTML의 페이지 수가 콘솔에 출력됩니다.

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

특정 저장 옵션에 대한 페이지 수를 가져오는 방법을 보여줍니다.

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

### 또 보기

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

기본 [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount()
```

### 반환 값

렌더링될 페이지 수.

## 예제

다양한 시간 척도에 대한 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// 페이지 수 가져오기, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

주어진 [`Timescale`](../../../aspose.tasks.visualization/timescale/)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(Timescale scale)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스케일 | Timescale | 페이지 수를 가져올 스케일입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

다양한 시간 척도에 대한 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// 페이지 수 가져오기, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### 또 보기

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

기본 [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Days) 및 지정된 [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(PresentationFormat format)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 형식 | PresentationFormat | 페이지 수를 가져올 형식입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

프레젠테이션 형식 및 시간 척도별 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Days(기본값), Months 및 ThirdsOfMonths에 대한 페이지 수 가져오기
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### 또 보기

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

주어진 [`Timescale`](../../../aspose.tasks.visualization/timescale/) 및 [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 형식 | PresentationFormat | 페이지 수를 가져올 형식입니다. |
| 스케일 | Timescale | 페이지 수를 가져올 스케일입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

프레젠테이션 형식 및 시간 척도별 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Days(기본값), Months 및 ThirdsOfMonths에 대한 페이지 수 가져오기
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### 또 보기

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

주어진 [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) 및 날짜 범위를 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageSize | PageSize | 페이지 수를 가져올 크기입니다. |
| 스케일 | Timescale | 페이지 수를 가져올 스케일입니다. |
| startDate | DateTime | 페이지 수를 가져올 시작 날짜입니다. |
| endDate | DateTime | 페이지 수를 가져올 종료 날짜입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

페이지 크기, 시간 척도, 시작 및 종료 날짜별 페이지 수를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### 또 보기

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

주어진 [`Timescale`](../../../aspose.tasks.visualization/timescale/) 및 [`PageSize`](../../../aspose.tasks.visualization/pagesize/)을 사용하여 렌더링되는 프로젝트의 페이지 수를 반환합니다.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| pageSize | PageSize | 페이지 수를 가져올 크기입니다. |
| 스케일 | Timescale | 페이지 수를 가져올 스케일입니다. |

### 반환 값

렌더링될 페이지 수.

## 예제

페이지 크기와 시간 척도를 사용하여 페이지 수를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### 또 보기

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


