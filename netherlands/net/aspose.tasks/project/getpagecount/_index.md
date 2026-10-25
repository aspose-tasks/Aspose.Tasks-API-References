---
title: "Project.GetPageCount"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven SaveOptions"
type: docs
weight: 1110
url: /nl/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| saveOptions | SaveOptions | De save-opties om het aantal pagina's voor te krijgen. |

### Retourwaarde

een aantal pagina's om te renderen.

## Voorbeelden

In dit voorbeeld wordt de instantie van HtmlSaveOptions en het aantal pagina's in de resulterende HTML naar de console geschreven.

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

Toont hoe je het aantal pagina's krijgt voor specifieke opslagopties.

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

### Zie ook

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Dagen).

```csharp
public int GetPageCount()
```

### Retourwaarde

Aantal pagina's om te renderen.

## Voorbeelden

Toont hoe je het aantal pagina's krijgt voor verschillende tijdschalen.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Haal het aantal pagina's op, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../../aspose.tasks.visualization/timescale/).

```csharp
public int GetPageCount(Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| schaal | Timescale | De schaal waarvoor het aantal pagina's wordt opgehaald. |

### Retourwaarde

Aantal pagina's om te renderen.

## Voorbeelden

Toont hoe je het aantal pagina's krijgt voor verschillende tijdschalen.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Haal het aantal pagina's op, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Zie ook

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de standaard [`Timescale`](../../../aspose.tasks.visualization/timescale/)(Dagen) en de opgegeven [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| formaat | PresentationFormat | Het formaat waarvoor het aantal pagina's wordt opgehaald. |

### Retourwaarde

Aantal pagina's om te renderen.

## Voorbeelden

Toont hoe je het aantal pagina's krijgt op basis van presentatieformaat en tijdschaal.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Haal het aantal pagina's op voor Dagen (standaard), Maanden en ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Zie ook

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../../aspose.tasks.visualization/timescale/) en [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/).

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| formaat | PresentationFormat | Het formaat waarvoor het aantal pagina's wordt opgehaald. |
| schaal | Timescale | De schaal waarvoor het aantal pagina's wordt opgehaald. |

### Retourwaarde

een aantal pagina's om te renderen.

## Voorbeelden

Toont hoe je het aantal pagina's krijgt op basis van presentatieformaat en tijdschaal.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Haal het aantal pagina's op voor Dagen (standaard), Maanden en ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Zie ook

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) en datumbereik.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageSize | PageSize | De grootte waarvoor het aantal pagina's wordt opgehaald. |
| schaal | Timescale | De schaal waarvoor het aantal pagina's wordt opgehaald. |
| startDate | DateTime | De startdatum waarvoor het aantal pagina's wordt opgehaald. |
| endDate | DateTime | De einddatum waarvoor het aantal pagina's wordt opgehaald. |

### Retourwaarde

Aantal pagina's om te renderen.

## Voorbeelden

Toont hoe je het aantal pagina's krijgt op basis van paginagrootte, tijdschaal, start- en einddatums.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Zie ook

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Retourneert het aantal pagina's voor het project dat wordt gerenderd met de opgegeven [`Timescale`](../../../aspose.tasks.visualization/timescale/) en [`PageSize`](../../../aspose.tasks.visualization/pagesize/).

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pageSize | PageSize | De grootte waarvoor het aantal pagina's wordt opgehaald. |
| schaal | Timescale | De schaal waarvoor het aantal pagina's wordt opgehaald. |

### Retourwaarde

Aantal pagina's om te renderen.

## Voorbeelden

Toont hoe het aantal pagina's te verkrijgen op basis van een paginagrootte en een tijdschaal.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Zie ook

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


