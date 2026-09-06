---
title: "Project.GetPageCount"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تُرجع عدد الصفحات للمشروع ليتم عرضها باستخدام SaveOptions المحددة"
type: docs
weight: 1110
url: /ar/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

تُرجع عدد الصفحات للمشروع ليتم عرضها باستخدام [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| saveOptions | SaveOptions | خيارات الحفظ للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد صفحات ليتم عرضها.

## الأمثلة

في هذا المثال، يتم كتابة نسخة HtmlSaveOptions وعدد الصفحات في HTML الناتج إلى وحدة التحكم.

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

يوضح كيفية الحصول على عدد الصفحات لخيارات الحفظ المحددة.

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

### انظر أيضًا

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) الافتراضي (الأيام).

```csharp
public int GetPageCount()
```

### قيمة الإرجاع

عدد الصفحات للعرض.

## الأمثلة

يوضح كيفية الحصول على عدد الصفحات لمقاييس زمنية مختلفة.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// احصل على عدد الصفحات، Timescale.Months، Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) المحدد.

```csharp
public int GetPageCount(Timescale scale)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| scale | Timescale | المقياس للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات للعرض.

## الأمثلة

يوضح كيفية الحصول على عدد الصفحات لمقاييس زمنية مختلفة.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// احصل على عدد الصفحات، Timescale.Months، Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### انظر أيضًا

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) الافتراضي (الأيام) و[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| format | PresentationFormat | الصيغة للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات للعرض.

## الأمثلة

يوضح كيفية الحصول على عدد الصفحات حسب PresentationFormat وTimescale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// احصل على عدد الصفحات للأيام (افتراضيًا)، الأشهر وThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### انظر أيضًا

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| format | PresentationFormat | الصيغة للحصول على عدد الصفحات. |
| scale | Timescale | المقياس للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد صفحات ليتم عرضها.

## الأمثلة

يوضح كيفية الحصول على عدد الصفحات حسب PresentationFormat وTimescale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// احصل على عدد الصفحات للأيام (افتراضيًا)، الأشهر وThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### انظر أيضًا

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) ونطاق التاريخ.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| pageSize | PageSize | الحجم للحصول على عدد الصفحات. |
| scale | Timescale | المقياس للحصول على عدد الصفحات. |
| startDate | DateTime | تاريخ البدء للحصول على عدد الصفحات. |
| endDate | DateTime | تاريخ الانتهاء للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات للعرض.

## الأمثلة

يوضح كيفية الحصول على عدد الصفحات حسب pageSize وTimescale وتواريخ startDate وendDate.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### انظر أيضًا

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

يعيد عدد الصفحات للمشروع الذي سيتم عرضه باستخدام [`Timescale`](../../../aspose.tasks.visualization/timescale/) و[`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| pageSize | PageSize | الحجم للحصول على عدد الصفحات. |
| scale | Timescale | المقياس للحصول على عدد الصفحات. |

### قيمة الإرجاع

عدد الصفحات للعرض.

## الأمثلة

يعرض كيفية الحصول على عدد الصفحات حسب حجم الصفحة والجدول الزمني.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### انظر أيضًا

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


