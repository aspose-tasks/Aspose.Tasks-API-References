---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project yöntemi. Verilen SaveOptions kullanılarak oluşturulacak projenin sayfa sayısını döndürür"
type: docs
weight: 1110
url: /tr/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Verilen [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) kullanılarak oluşturulacak projenin sayfa sayısını döndürür.

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveOptions | SaveOptions | Sayfa sayısını almak için kullanılan kaydetme seçenekleri. |

### Dönüş Değeri

oluşturulacak bir sayfa sayısı.

## Örnekler

Bu örnekte HtmlSaveOptions örneği ve ortaya çıkan HTML'deki sayfa sayısı konsola yazdırılır.

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

Belirli kaydetme seçenekleri için sayfa sayısının nasıl alınacağını gösterir.

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

### Ayrıca Bakınız

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Varsayılan [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Gün) kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount()
```

### Dönüş Değeri

Oluşturulacak sayfa sayısı.

## Örnekler

Farklı zaman ölçekleri için sayfa sayısının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Sayfa sayısını al, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Ayrıca Bakınız

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Verilen [`Timescale`](../../../aspose.tasks.visualization/timescale/) kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount(Timescale scale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ölçek | Timescale | Sayfa sayısını almak için ölçek. |

### Dönüş Değeri

Oluşturulacak sayfa sayısı.

## Örnekler

Farklı zaman ölçekleri için sayfa sayısının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Sayfa sayısını al, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Ayrıca Bakınız

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Varsayılan [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Gün) ve verilen [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| biçim | PresentationFormat | Sayfa sayısını almak için format. |

### Dönüş Değeri

Oluşturulacak sayfa sayısı.

## Örnekler

Sunum formatı ve zaman ölçeğine göre sayfa sayısının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Günler (varsayılan), Aylar ve ThirdsOfMonths için sayfa sayısını al.
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Ayrıca Bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Verilen [`Timescale`](../../../aspose.tasks.visualization/timescale/) ve [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| biçim | PresentationFormat | Sayfa sayısını almak için format. |
| ölçek | Timescale | Sayfa sayısını almak için ölçek. |

### Dönüş Değeri

oluşturulacak bir sayfa sayısı.

## Örnekler

Sunum formatı ve zaman ölçeğine göre sayfa sayısının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Günler (varsayılan), Aylar ve ThirdsOfMonths için sayfa sayısını al.
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Ayrıca Bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Verilen [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) ve tarih aralığı kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısını almak için boyut. |
| ölçek | Timescale | Sayfa sayısını almak için ölçek. |
| startDate | DateTime | Sayfa sayısını almak için başlangıç tarihi. |
| endDate | DateTime | Sayfa sayısını almak için bitiş tarihi. |

### Dönüş Değeri

Oluşturulacak sayfa sayısı.

## Örnekler

Sayfa boyutu, zaman ölçeği, başlangıç ve bitiş tarihine göre sayfa sayısının nasıl alınacağını gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Ayrıca Bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Verilen [`Timescale`](../../../aspose.tasks.visualization/timescale/) ve [`PageSize`](../../../aspose.tasks.visualization/pagesize/) kullanılarak oluşturulacak proje için sayfa sayısını döndürür.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısını almak için boyut. |
| ölçek | Timescale | Sayfa sayısını almak için ölçek. |

### Dönüş Değeri

Oluşturulacak sayfa sayısı.

## Örnekler

Sayfa sayısını sayfa boyutu ve zaman ölçeğine göre nasıl alacağınızı gösterir.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Ayrıca Bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


