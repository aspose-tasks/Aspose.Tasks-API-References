---
title: Project.GetPageCount
second_title: Aspose.Tasks för .NET API-referens
description: Project metod. Returnerar antalet sidor för projektet som ska renderas med givenSaveOptions .
type: docs
weight: 1080
url: /sv/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Returnerar antalet sidor för projektet som ska renderas med given[`SaveOptions`](../../../aspose.tasks.saving/saveoptions/) .

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveOptions | SaveOptions | Spara alternativ för att få sidräkning för. |

### Returvärde

ett sidantal som ska återges.

### Exempel

I det här exemplet skrivs HtmlSaveOptions och antalet sidor i resulterande HTML till konsolen.

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

### Se även

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Returnerar sidantal för projektet som ska renderas med standard[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Dagar).

```csharp
public int GetPageCount()
```

### Returvärde

Antal sidor som ska återges.

### Se även

* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../../aspose.tasks.visualization/timescale/) .

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| scale | Timescale | Skalan för att få sidantal för. |

### Returvärde

Antal sidor som ska återges.

### Se även

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Returnerar sidantal för projektet som ska renderas med standard[`Timescale`](../../../aspose.tasks.visualization/timescale/) (Dagar) och givet[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/)

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | PresentationFormat | Formatet att få sidantal för. |

### Returvärde

Antal sidor som ska återges.

### Se även

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../../aspose.tasks.visualization/timescale/) och[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) .

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| format | PresentationFormat | Formatet att få sidantal för. |
| scale | Timescale | Skalan för att få sidantal för. |

### Returvärde

ett sidantal som ska återges.

### Se även

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../../aspose.tasks.visualization/timescale/) ,[`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) och datumintervall.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageSize | PageSize | Storleken att få sidantal för. |
| scale | Timescale | Skalan för att få sidantal för. |
| startDate | DateTime | Startdatum för att få sidräkning för. |
| endDate | DateTime | Slutdatum för att få sidantal för. |

### Returvärde

Antal sidor som ska återges.

### Se även

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Returnerar antalet sidor för projektet som ska renderas med given[`Timescale`](../../../aspose.tasks.visualization/timescale/) och[`PageSize`](../../../aspose.tasks.visualization/pagesize/) .

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageSize | PageSize | Storleken att få sidantal för. |
| scale | Timescale | Skalan för att få sidantal för. |

### Returvärde

Antal sidor som ska återges.

### Se även

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namnutrymme [Aspose.Tasks](../../project/)
* hopsättning [Aspose.Tasks](../../../)


