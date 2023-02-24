---
title: Project.GetPageCount
second_title: Aspose.Tasks for .NET API Referansı
description: Project yöntem. Verilen kullanılarak işlenecek proje için sayfa sayısını döndürürSaveOptions .
type: docs
weight: 1080
url: /tr/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Verilen kullanılarak işlenecek proje için sayfa sayısını döndürür[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| saveOptions | SaveOptions | Sayfa sayısını almak için kaydetme seçenekleri. |

### Geri dönüş değeri

işlenecek bir sayfa sayısı.

### Örnekler

Bu örnekte HtmlSaveOptions örneği ve ortaya çıkan HTML'deki sayfa sayısı konsola yazılır.

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

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Varsayılan kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Gün).

```csharp
public int GetPageCount()
```

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Verilen kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| scale | Timescale | Sayfa sayısı alınacak ölçek. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Varsayılan kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Günler) ve verilen[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| format | PresentationFormat | Sayfa sayısı alınacak biçim. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Verilen kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) Ve[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| format | PresentationFormat | Sayfa sayısı alınacak biçim. |
| scale | Timescale | Sayfa sayısı alınacak ölçek. |

### Geri dönüş değeri

işlenecek bir sayfa sayısı.

### Ayrıca bakınız

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Verilen kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) ve tarih aralığı.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısı alınacak boyut. |
| scale | Timescale | Sayfa sayısı alınacak ölçek. |
| startDate | DateTime | Sayfa sayısını almak için başlangıç tarihi. |
| endDate | DateTime | Sayfa sayısını almak için bitiş tarihi. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Verilen kullanılarak işlenecek proje için sayfa sayısını döndürür[`Timescale`](../../../aspose.tasks.visualization/timescale/) Ve[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageSize | PageSize | Sayfa sayısı alınacak boyut. |
| scale | Timescale | Sayfa sayısı alınacak ölçek. |

### Geri dönüş değeri

Oluşturulacak sayfa sayısı.

### Ayrıca bakınız

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* ad alanı [Aspose.Tasks](../../project/)
* toplantı [Aspose.Tasks](../../../)


