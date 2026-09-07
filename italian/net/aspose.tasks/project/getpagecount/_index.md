---
title: "Project.GetPageCount"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Restituisce il conteggio delle pagine per il progetto da renderizzare usando le SaveOptions fornite"
type: docs
weight: 1110
url: /it/net/aspose.tasks/project/getpagecount/
---
## GetPageCount(SaveOptions) {#getpagecount_1}

Restituisce il conteggio delle pagine per il progetto da renderizzare usando le [`SaveOptions`](../../../aspose.tasks.saving/saveoptions/).

```csharp
public int GetPageCount(SaveOptions saveOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveOptions | SaveOptions | Le opzioni di salvataggio per le quali ottenere il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da renderizzare.

## Esempi

In questo esempio l'istanza di HtmlSaveOptions e il numero di pagine nell'HTML risultante vengono scritti sulla console.

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

Mostra come ottenere il conteggio delle pagine per opzioni di salvataggio specifiche.

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

### Vedi anche

* class [SaveOptions](../../../aspose.tasks.saving/saveoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount() {#getpagecount}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/) predefinito (Giorni).

```csharp
public int GetPageCount()
```

### Valore di ritorno

Conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine per diverse scale temporali.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Ottieni il numero di pagine, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Vedi anche

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(Timescale) {#getpagecount_6}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/) fornito.

```csharp
public int GetPageCount(Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| scala | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine per diverse scale temporali.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");

// Ottieni il numero di pagine, Timescale.Months, Timescale.ThirdsOfMonths
var pageCount = project.GetPageCount();
Console.WriteLine("Page count: " + pageCount);
pageCount = project.GetPageCount(Timescale.Months);
Console.WriteLine("Page count (Month): " + pageCount);
pageCount = project.GetPageCount(Timescale.ThirdsOfMonths);
Console.WriteLine("Page count (Thirds of Months): " + pageCount);
```

### Vedi anche

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat) {#getpagecount_4}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/) predefinito (Giorni) e il [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) fornito.

```csharp
public int GetPageCount(PresentationFormat format)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formato | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine per formato di presentazione e scala temporale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Ottieni il numero di pagine per Days (per impostazione predefinita), Months e ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Vedi anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PresentationFormat, Timescale) {#getpagecount_5}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/) e il [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) forniti.

```csharp
public int GetPageCount(PresentationFormat format, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formato | PresentationFormat | Il formato per cui ottenere il conteggio delle pagine. |
| scala | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

un conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine per formato di presentazione e scala temporale.

```csharp
var project = new Project(DataDir + "GetNumberOfPagesForViews.mpp");

// Ottieni il numero di pagine per Days (per impostazione predefinita), Months e ThirdsOfMonths
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Days));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.Months));
Console.WriteLine("Number of Pages = '{0}'", project.GetPageCount(PresentationFormat.ResourceUsage, Timescale.ThirdsOfMonths));
```

### Vedi anche

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale, DateTime, DateTime) {#getpagecount_3}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/), il [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) e l'intervallo di date.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale, DateTime startDate, DateTime endDate)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | PageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scala | Timescale | La scala per cui ottenere il conteggio delle pagine. |
| startDate | DateTime | La data di inizio per cui ottenere il conteggio delle pagine. |
| endDate | DateTime | La data di fine per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine per dimensione della pagina, scala temporale, date di inizio e fine.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(
    PageSize.A3,
    Timescale.Months,
    project.Get(Prj.StartDate) - TimeSpan.FromDays(10),
    project.Get(Prj.FinishDate) + TimeSpan.FromDays(30));

Console.WriteLine(pageCount);
```

### Vedi anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetPageCount(PageSize, Timescale) {#getpagecount_2}

Restituisce il conteggio delle pagine per il progetto da renderizzare utilizzando il [`Timescale`](../../../aspose.tasks.visualization/timescale/) e il [`PageSize`](../../../aspose.tasks.visualization/pagesize/) forniti.

```csharp
public int GetPageCount(PageSize pageSize, Timescale scale)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageSize | PageSize | La dimensione per cui ottenere il conteggio delle pagine. |
| scala | Timescale | La scala per cui ottenere il conteggio delle pagine. |

### Valore di ritorno

Conteggio delle pagine da renderizzare.

## Esempi

Mostra come ottenere il conteggio delle pagine in base a una dimensione di pagina e a una scala temporale.

```csharp
var project = new Project(DataDir + "GetNumberOfPages.mpp");
var pageCount = project.GetPageCount(PageSize.A3, Timescale.Months);

Console.WriteLine(pageCount);
```

### Vedi anche

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


