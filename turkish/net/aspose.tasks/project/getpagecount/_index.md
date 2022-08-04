---
title: GetPageCount
second_title: Aspose.Tasks for .NET API Referansı
description: Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürürSaveOptionsaspose.tasks.saving/saveoptions .
type: docs
weight: 300
url: /tr/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`SaveOptions`](../../../aspose.tasks.saving/saveoptions) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| saveOptions | SaveOptions | Sayfa sayısını almak için kaydetme seçenekleri. |

### Geri dönüş değeri

işlenecek bir sayfa sayısı.

### Örnekler

Bu örnekte HtmlSaveOptions örneği ve sonuçta elde edilen HTML'deki sayfa sayısı konsola yazılır.

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

### Ayrıca bakınız

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Varsayılan kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) (Gün).

```csharp
public int GetPageCount()
```

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| scale | Timescale | Sayfa sayısının alınacağı ölçek. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Varsayılan kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) (Günler) ve verilen[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| format | PresentationFormat | Sayfa sayısının alınacağı biçim. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) ve[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| format | PresentationFormat | Sayfa sayısının alınacağı biçim. |
| scale | Timescale | Sayfa sayısının alınacağı ölçek. |

### Geri dönüş değeri

işlenecek bir sayfa sayısı.

### Ayrıca bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat) ve tarih aralığı.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısının alınacağı boyut. |
| scale | Timescale | Sayfa sayısının alınacağı ölçek. |
| startDate | DateTime | Sayfa sayısının alınacağı başlangıç tarihi. |
| endDate | DateTime | Sayfa sayısının alınacağı bitiş tarihi. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Verilen kullanılarak oluşturulacak proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale) ve[`PageSize`](../../../aspose.tasks.visualization/pagesize) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısının alınacağı boyut. |
| scale | Timescale | Sayfa sayısının alınacağı ölçek. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize)
* enum [Timescale](../../../aspose.tasks.visualization/timescale)
* class [Project](../../project)
* ad alanı [Aspose.Tasks](../../project)
* toplantı [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
